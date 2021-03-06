<img src="http://www.cytoscape.org/images/logo/cy3logoOrange.svg" height=50>

# Gun-scape 
[GunDB](https://github.com/amark/gun) Cytoscape Graph Visualizer + Live Editor

#### [Try the Live Demo](http://rawgit.com/lmangani/gun-scape/master/index.html)
Execute your own _"Shot-GunDB Wedding"_ and test all Gun [commands](http://gun.js.org/docs/get.html) in a snap:
![ezgif com-optimize 30](https://user-images.githubusercontent.com/1423657/31863000-bdd31120-b747-11e7-8b7c-b2586aa7cae8.gif)
<!-- ![ezgif com-optimize 29](https://user-images.githubusercontent.com/1423657/31855811-136fc9e2-b6b3-11e7-9b40-0b6e1a57ad29.gif) -->

###### Flow Example
```
g.get('ua').put({name: 'SIP User-Agent'});
g.get('opensips').put({name: 'OpenSIPS'});
g.get('asterisk').put({name: 'Asterisk'});
g.get('rtpengine').put({name: 'RTP:Engine'});
g.get('homer').put({name: 'HOMER'});
g.get('ua').get('sip').put(g.get('opensips')); 
g.get('ua').get('rtp').put(g.get('rtpengine')); 
g.get('opensips').get('sip').put(g.get('asterisk')); 
g.get('rtpengine').get('rtp').put(g.get('asterisk')); 
g.get('opensips').get('hep-sip').put(g.get('homer')); 
g.get('asterisk').get('hep-sip').put(g.get('homer')); 
g.get('rtpengine').get('hep-rtcp').put(g.get('homer')); 
```
<img src="https://user-images.githubusercontent.com/1423657/31861056-e283d9f4-b725-11e7-8e77-faddca3bbaf8.png" width=500/>

### Credit
This Demo is based on [serve-gun](https://github.com/JosePedroDias/serve-gundb)
