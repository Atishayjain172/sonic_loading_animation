Center(
                  child: Row(
                    mainAxisAlignment: MainAxisAlignment.start,
                    children: <Widget>[
                      Container(child: TweenAnimationBuilder(
                          duration: Duration(milliseconds: 5000),
                          tween: Tween<double>(begin: 0,end: MediaQuery.of(context).size.width - 150),
                          builder: (_,double value,__){
                            return Padding(
                                padding: EdgeInsets.fromLTRB(value,0,0,0),
                                child: Image.asset('listloading.gif',
                                  height: 100,
                                  width: 100,));
                          }
                      )),
                    ],
                  ),
                );