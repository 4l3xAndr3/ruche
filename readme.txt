Animation d abeilles autour d une ruche (code pour le fun)----------------------------------------------------------
Url     : http://codes-sources.commentcamarche.net/source/54636-animation-d-abeilles-autour-d-une-ruche-code-pour-le-funAuteur  : cs_crisdiDate    : 07/08/2013
Licence :
=========

Ce document intitulé « Animation d abeilles autour d une ruche (code pour le fun) » issu de CommentCaMarche
(codes-sources.commentcamarche.net) est mis à disposition sous les termes de
la licence Creative Commons. Vous pouvez copier, modifier des copies de cette
source, dans les conditions fixées par la licence, tant que cette note
apparaît clairement.

Description :
=============

Pour le plaisir des yeux uniquement : Animation d abeilles autour d une ruche.

<br />C est principalement pour le plaisir de coder de l animation en JavaScript
.
<br /><a name='source-exemple'></a><h2> Source / Exemple : </h2>
<br /><pre
 class='code' data-mode='basic'>
&lt;!DOCTYPE HTML PUBLIC &quot;-//W3C//DTD HTM
L 4.01 Transitional//EN&quot;&gt;
&lt;html&gt;
&lt;head&gt;
&lt;SCRIPT LANGUA
GE=&quot;JavaScript&quot;&gt; 
var Xpos = 2;
var Ypos = 2;
var FlagChoix = 0;

var vara=&quot;DIV ID&quot;;
var varb=&quot;/DIV&quot;;
var m = 0 ;
var n =
 0 ;
var Leader = 0;
var styl='style=&quot;position:absolute;left:0px;top:0px;
width:32px;height:32px;visibility:hidden;&quot;'
chaine='&lt;'+vara+'=&quot;obj
0&quot; '+styl+'&gt;'
+'&lt;img src=&quot;Abeille2.gif&quot; border=0 &gt;'
+'
&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quot;obj15&quot; '+styl+'&gt;'
+'&lt;img src
=&quot;Fleur66.gif&quot; border=0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&qu
ot;obj21&quot; '+styl+'&gt;'
+'&lt;img src=&quot;Fleur32.gif&quot; border=0 &gt
;'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quot;obj16&quot; '+styl+'&gt;'
+'&lt;i
mg src=&quot;Fleurs168.gif&quot; border=0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'+va
ra+'=&quot;obj17&quot; '+styl+'&gt;'
+'&lt;img src=&quot;FleursJonquilles1.gif&
quot; border=0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quot;obj18&quot; '+st
yl+'&gt;'
+'&lt;img src=&quot;Fleur35.gif&quot; border=0 &gt;'
+'&lt;'+varb+'&
gt;'
+'&lt;'+vara+'=&quot;obj19&quot; '+styl+'&gt;'
+'&lt;img src=&quot;Fleur3
7.gif&quot; border=0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quot;obj20&quot
; '+styl+'&gt;'
+'&lt;img src=&quot;Fleur31.gif&quot; border=0 &gt;'
+'&lt;'+v
arb+'&gt;'
+'&lt;'+vara+'=&quot;obj14&quot; '+styl+'&gt;'
+'&lt;img src=&quot;
FleursRoses32.gif&quot; border=0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quo
t;obj1&quot; '+styl+'&gt;'
+'&lt;img src=&quot;Abeille2.gif&quot; border=0 &gt;
'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quot;obj2&quot; '+styl+'&gt;'
+'&lt;img
 src=&quot;Abeille2.gif&quot; border=0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+
'=&quot;obj3&quot; '+styl+'&gt;'
+'&lt;img src=&quot;Abeille2.gif&quot; border=
0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quot;obj4&quot; '+styl+'&gt;'
+'&
lt;img src=&quot;Abeille2.gif&quot; border=0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'
+vara+'=&quot;obj5&quot; '+styl+'&gt;'
+'&lt;img src=&quot;Abeille2.gif&quot; b
order=0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quot;obj6&quot; '+styl+'&gt;
'
+'&lt;img src=&quot;Abeille2.gif&quot; border=0 &gt;'
+'&lt;'+varb+'&gt;'
+
'&lt;'+vara+'=&quot;obj7&quot; '+styl+'&gt;'
+'&lt;img src=&quot;Abeille1.gif&q
uot; border=0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quot;obj8&quot; '+styl
+'&gt;'
+'&lt;img src=&quot;Abeille1.gif&quot; border=0&gt;'
+'&lt;'+varb+'&gt
;'
+'&lt;'+vara+'=&quot;obj9&quot; '+styl+'&gt;'
+'&lt;img src=&quot;Abeille1.
gif&quot; border=0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quot;obj10&quot; 
'+styl+'&gt;'
+'&lt;img src=&quot;Abeille1.gif&quot; border=0 &gt;'
+'&lt;'+va
rb+'&gt;'
+'&lt;'+vara+'=&quot;obj11&quot; '+styl+'&gt;'
+'&lt;img src=&quot;A
beille1.gif&quot; border=0 &gt;'
+'&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quot;obj1
2&quot; '+styl+'&gt;'
+'&lt;img src=&quot;Abeille1.gif&quot; border=0 &gt;'
+'
&lt;'+varb+'&gt;'
+'&lt;'+vara+'=&quot;obj13&quot; '+styl+'&gt;'
+'&lt;img src
=&quot;Ruche2.gif&quot; border=0 &gt;'
+'&lt;'+varb+'&gt;'

document.write(ch
aine);
var div0 = document.getElementById(&quot;obj0&quot;).style;
var div1 = 
document.getElementById(&quot;obj1&quot;).style;
var div2 = document.getElement
ById(&quot;obj2&quot;).style;
var div3 = document.getElementById(&quot;obj3&quo
t;).style;
var div4 = document.getElementById(&quot;obj4&quot;).style;
var div
5 = document.getElementById(&quot;obj5&quot;).style;
var div6 = document.getEle
mentById(&quot;obj6&quot;).style;
var div7 = document.getElementById(&quot;obj7
&quot;).style;
var div8 = document.getElementById(&quot;obj8&quot;).style;
var
 div9 = document.getElementById(&quot;obj9&quot;).style;
var div10 = document.g
etElementById(&quot;obj10&quot;).style;
var div11 = document.getElementById(&qu
ot;obj11&quot;).style;
var div12 = document.getElementById(&quot;obj12&quot;).s
tyle;
var div13 = document.getElementById(&quot;obj13&quot;).style;
var div14 
= document.getElementById(&quot;obj14&quot;).style;
var div15 = document.getEle
mentById(&quot;obj15&quot;).style;
var div16 = document.getElementById(&quot;ob
j16&quot;).style;
var div17 = document.getElementById(&quot;obj17&quot;).style;

var div18 = document.getElementById(&quot;obj18&quot;).style;
var div19 = doc
ument.getElementById(&quot;obj19&quot;).style;
var div20 = document.getElementB
yId(&quot;obj20&quot;).style;
var div21 = document.getElementById(&quot;obj21&q
uot;).style;
var objet;var coordx;var coordy;
objet = new Array(div0,div1,div2
,div3,div4,div5,div6,div7,div8,div9,div10,div11,div12,div13,div14,div15,div16,di
v17,div18,div19,div20,div21);
coordx = new Array(20,410,30,524,27,22,316,40,744
,30,764,80,920,500,1,1,1,1,1,1,1,1);
coordy = new Array(50,115,130,170,210,250,
290,230,250,203,190,100,50,333,1,1,1,1,1,1,1,1);
mouvx = new Array(7.2,10.1,12.
2,11.2,15,14.2,16,-12.1,-14.2,-11.5,-8.2,-10.3,-13,0,0,0,0,0,0,0,0,0);
mouvy = 
new Array(-1.2,2.1,-3.3,4,-2.7,4.1,-2.3,5.4,-3.6,2.6,-1.3,4.1,-3.4,0,0,0,0,0,0,0
,0,0);
var Xruche=1;
var Yruche=1;
var Liberte=-3;
for (var i = 0; i &lt; 22
; i++) {
   objet[i].visibility=&quot;visible&quot;;
}
function placeObj(i,px
,py) {
 objet[i].left=px;
 objet[i].top=py;
}
if (document.getElementById)  
{
   if(navigator.appName.substring(0,3) == &quot;Net&quot;)
      document.ca
ptureEvents(Event.MOUSEMOVE);
   document.onmousemove = Pos_Souris;
   }
func
tion Pos_Souris(e) {
   Xpos = (navigator.appName.substring(0,3) == &quot;Net&q
uot;) ? e.pageX : event.x+document.body.scrollLeft;
   Ypos = (navigator.appNam
e.substring(0,3) == &quot;Net&quot;) ? e.pageY : event.y+document.body.scrollTop
;
   Xpos = Xpos - 10;
}
function mouvement() {
 if (window.innerWidth) { Ec
ranlargeur = window.innerWidth-70; Ecranhauteur = window.innerHeight-100;}
 els
e if (document.documentElement &amp;&amp; document.documentElement.clientWidth){

 Ecranlargeur = document.documentElement.clientWidth-70; Ecranhauteur = docume
nt.documentElement.clientHeight-100;
 } else if (document.body) { Ecranlargeur 
= document.body.clientWidth-70; Ecranhauteur = document.body.clientHeight-10;}

 Ecranhauteur = Ecranhauteur + 0;
 Ecranlargeur = Ecranlargeur + 0;
//===[ pos
ition de la Ruche et des fleurs ]=========//
  Xruche=(Ecranlargeur/2) ;
  Yru
che=(Ecranhauteur- 120);  
  coordx[13] = (Xruche-70);
  coordy[13] = (Yruche-
30); 
  coordx[14] = 2;
  coordx[15] = (Ecranlargeur/8);
  coordx[16] = (Ecra
nlargeur/5);
  coordx[17] = (Ecranlargeur/3);
  coordx[18] = (Ecranlargeur/1.5
);
  coordx[19] = (Ecranlargeur/1.3);
  coordx[20] = (Ecranlargeur/1.16);
  c
oordx[21] = (Ecranlargeur-50);
  coordy[14] = (Yruche+30);
  coordy[15] = (Yru
che+30);
  coordy[16] = (Yruche+30);
  coordy[17] = (Yruche+80);
  coordy[18]
 = (Yruche+90);
  coordy[19] = (Yruche+30);
  coordy[20] = (Yruche+80);
  coo
rdy[21] = (Yruche+30);
//===[ init Abeilles dans ruche ]=========//
if (Libert
e == -3) {
   for (var i = 0; i &lt; 13; i++) {
	coordy[i] = (Yruche+ mouvy[i]
+ 30);
        coordx[i] = Xruche;	
   }
   Liberte=250;
   coordx[9] = Ecra
nlargeur-50;
   coordx[2] = 10;
}
//===[ Liberation des Abeilles de la ruche 
a 300 et reset a 400 ]=========// 
Liberte=Liberte+1; 
if (Liberte &gt; 400) L
iberte = 0 ;
  //===if (Liberte &lt; 300) objet[13].visibility=&quot;visible&qu
ot;; ==// 
  //===if (Liberte &gt; 300) objet[13].visibility=&quot;hidden&quot;
; ==// 
//===[ début boucle principale par Abeille ]=========//
for (var i = 0
; i &lt; 13; i++) {
   FlagChoix=0;
   //===[ stoppe les Abeilles proches de l
a souris ]=========// 
   if ( FlagChoix ==0) { 
      if ( coordy[i] &gt; ( Y
pos - 70) ) {
      if ( coordy[i] &lt; ( Ypos + 70) ) {
      if ( coordx[i] 
&gt; ( Xpos - 50) ) {
      if ( coordx[i] &lt; ( Xpos + 50) ) {
          Fla
gChoix=1; 
          if ( coordy[i] &gt; Ypos ) {     
              coordy[i]
 = coordy[i] -11; 
          }         
          if ( coordy[i] &lt; Ypos ) {
     
              coordy[i] = coordy[i] +14;
          }
          if ( coo
rdx[i] &lt; Xpos ) {     
              coordx[i] = coordx[i] -16;
          }

          if ( coordx[i] &gt; Xpos ) {     
              coordx[i] = coordx[
i] +12;
          }    
       }}}}
   }
   //===[ stoppe les Abeilles proch
es de la ruche ]=========// 
   if ( FlagChoix ==0) { 
      if ( coordy[i] &g
t; ( Yruche - 30) ) {
      if ( coordy[i] &lt; ( Yruche + 90) ) {
      if ( 
coordx[i] &gt; ( Xruche - 40) ) {
      if ( coordx[i] &lt; ( Xruche + 40) ) {

          FlagChoix=1;
          if ( coordx[i] &lt; Xruche ) {     
        
     coordx[i] = coordx[i] -16;
          }
          if ( coordx[i] &gt; Xruc
he ) {     
             coordx[i] = coordx[i] +12;
          }
          if 
(Liberte &lt; 300) { 
             if ( coordy[i] &gt; Yruche ) {     
       
          coordy[i] = coordy[i] -11; 
             }         
             if 
( coordy[i] &lt; Yruche) {     
                 coordy[i] = coordy[i] +14;
  
           }
          }else{
             coordy[i] = coordy[i] +14;
       
   }
       }}}}
   }

   //===[ Les Abeilles butinentle bouquet de Roses ro
ses Obj 14 - position 1 ]=========// 
   if ( FlagChoix ==0) { 
      if ( coo
rdy[i] &gt; ( (Yruche+40) - 20) ) {
      if ( coordy[i] &lt; ( (Yruche+40) + 4
0) ) {
      if ( coordx[i] &gt; 2) {
      if ( coordx[i] &lt; 52) {
       
   if ( coordx[i] &lt; 20) {     
             coordx[i] = coordx[i] -1;       
    
          }
          if ( coordx[i] &gt; 20) {     
             coordx
[i] = coordx[i] +1;
          }
          if (Liberte &lt; 300) {
           
  FlagChoix=1; 
             coordy[i] = coordy[i] -1;
          }
       }}}
}
   }

   //===[ Les Abeilles butinentle tournesol jaune  Obj 15 - position 
2 ]=========// 
   if ( FlagChoix ==0) { 
      if ( coordy[i] &gt; ( (Yruche+
40) - 20) ) {
      if ( coordy[i] &lt; ( (Yruche+40) + 40) ) {
      if ( coo
rdx[i] &gt; ( (Ecranlargeur/8) - 20) ) {
      if ( coordx[i] &lt; ( (Ecranlarg
eur/8) + 50) ) {
          if ( coordx[i] &lt; (Ecranlargeur/8) ) {     
     
        coordx[i] = coordx[i] -1;           
          }
          if ( coordx
[i] &gt; (Ecranlargeur/8) ) {     
             coordx[i] = coordx[i] +1;
    
      }
          if (Liberte &lt; 370) {
             FlagChoix=1; 
        
     coordy[i] = coordy[i] -1;
          }
       }}}}
   }

   //===[ Les 
Abeilles butinentla Tulipes violettes  Obj 16 - position 3 ]=========// 
   if 
( FlagChoix ==0) { 
      if ( coordy[i] &gt; ( (Yruche+40) - 20) ) {
      if
 ( coordy[i] &lt; ( (Yruche+40) + 40) ) {
      if ( coordx[i] &gt; ( (Ecranlar
geur/5) - 20) ) {
      if ( coordx[i] &lt; ( (Ecranlargeur/5) + 50) ) {
     
     if ( coordx[i] &lt; (Ecranlargeur/5) ) {     
             coordx[i] = coo
rdx[i] -1;           
          }
          if ( coordx[i] &gt; (Ecranlargeur/
5) ) {     
             coordx[i] = coordx[i] +1;
          }
          if (
Liberte &lt; 380) {
             FlagChoix=1; 
             coordy[i] = coordy
[i] -1;
          }
       }}}}
   }

   //===[ Les Abeilles butinent les J
onquilles  Obj 17 - position 4 ]=========// 
   if ( FlagChoix ==0) { 
      i
f ( coordy[i] &gt; ( (Yruche+70) - 20) ) {
      if ( coordy[i] &lt; ( (Yruche+
70) + 40) ) {
      if ( coordx[i] &gt; ( (Ecranlargeur/3) - 20) ) {
      if 
( coordx[i] &lt; ( (Ecranlargeur/3) + 50) ) {
          if ( coordx[i] &lt; (Ec
ranlargeur/3) ) {     
             coordx[i] = coordx[i] -1;           
     
     }
          if ( coordx[i] &gt; (Ecranlargeur/3) ) {     
             co
ordx[i] = coordx[i] +1;
          }
          if (Liberte &lt; 380) {
       
      FlagChoix=1; 
             coordy[i] = coordy[i] -1;
          }
      
 }}}}
   }

   //===[ Les Abeilles butinentla Rose Rose Obj 18 - position 5 ]
=========// 
   if ( FlagChoix ==0) { 
      if ( coordy[i] &gt; ( (Yruche+60)
 - 10) ) {
      if ( coordy[i] &lt; ( (Yruche+60) + 40) ) {
      if ( coordx
[i] &gt; ( (Ecranlargeur/1.5) - 30) ) {
      if ( coordx[i] &lt; ( (Ecranlarge
ur/1.5) + 40) ) {
          if ( coordx[i] &lt; (Ecranlargeur/1.5) ) {     
  
           coordx[i] = coordx[i] -1;           
          }
          if ( coo
rdx[i] &gt; (Ecranlargeur/1.5) ) {     
             coordx[i] = coordx[i] +1;

          }
          if (Liberte &lt; 320) {
             FlagChoix=1; 
   
          coordy[i] = coordy[i] -1;
          }
       }}}}
   }

   //===[
 Les Abeilles butinent la tulipe jaune Obj 19 - position 6 ]=========// 
   if 
( FlagChoix ==0) { 
      if ( coordy[i] &gt; ( (Yruche+40) - 10) ) {
      if
 ( coordy[i] &lt; ( (Yruche+40) + 30) ) {
      if ( coordx[i] &gt; ( (Ecranlar
geur/1.3) - 20) ) {
      if ( coordx[i] &lt; ( (Ecranlargeur/1.3) + 50) ) {
 
         if ( coordx[i] &lt; (Ecranlargeur/1.3) ) {     
             coordx[i]
 = coordx[i] -1;           
          }
          if ( coordx[i] &gt; (Ecranla
rgeur/1.3) ) {     
             coordx[i] = coordx[i] +1;
          }
      
    if (Liberte &lt; 260) {
             FlagChoix=1; 
             coordy[i] 
= coordy[i] -1;
          }
       }}}}
   }

   //===[ Les Abeilles butine
nt la Rose rouge  Obj 20 -  position 7 ]=========// 
   if ( FlagChoix ==0) { 

      if ( coordy[i] &gt; ( (Yruche+70) - 20) ) {
      if ( coordy[i] &lt; ( 
(Yruche+70) + 40) ) {
      if ( coordx[i] &gt; ( (Ecranlargeur/1.16) - 20) ) {

      if ( coordx[i] &lt; ( (Ecranlargeur/1.16) + 50) ) {
          if ( coor
dx[i] &lt; (Ecranlargeur/1.16) ) {     
             coordx[i] = coordx[i] -1; 
          
          }
          if ( coordx[i] &gt; (Ecranlargeur/1.16) ) {  
   
             coordx[i] = coordx[i] +1;
          }
          if (Liberte 
&gt; 50) {
             FlagChoix=1; 
             coordy[i] = coordy[i] -1;

          }
       }}}}
   }

   //===[ Les Abeilles butinent  la Rose blanc
e  Obj 21  - position 8 ]=========// 
   if ( FlagChoix ==0) { 
      if ( coo
rdy[i] &gt; ( (Yruche+40)-20 ) ) {
      if ( coordy[i] &lt; ( (Yruche+40)+40 )
 ) {
      if ( coordx[i] &gt; ( (Ecranlargeur-50) - 20 ) ) {
      if ( coord
x[i] &lt; ( (Ecranlargeur-50) + 50 ) ) {
          if ( coordx[i] &lt; (Ecranla
rgeur-50) ) {     
             coordx[i] = coordx[i] -1;           
         
 }
          if ( coordx[i] &gt; (Ecranlargeur-50) ) {     
             coord
x[i] = coordx[i] +1;
          }
          if (Liberte &lt; 370) {
          
   FlagChoix=1; 
             coordy[i] = coordy[i] -1;
          }
       }}
}}
   }

   //===[ deplacement des Abeilles libres ]=========//
   if ( Flag
Choix ==0) { 
      coordx[i] = coordx[i] + mouvx[i] ;
      coordy[i] = coord
y[i] + mouvy[i] ;
   }
   //===[ mouvement aux limites de l ecran ]==========/
/    
   if (coordx[i] &gt; Ecranlargeur) coordx[i] = 11 ;
   if (coordx[i] &l
t; 3 ) coordx[i] = Ecranlargeur ;
   if (coordy[i] &gt; (Yruche+110) ) mouvy[i]
 = - mouvy[i]  ;
   if (coordy[i] &lt; (Yruche-260) ) mouvy[i] = - mouvy[i] ;

//===[ fin boucle principale des abeilles ]=========//
}
 
//===[ affichage ]
=========//
for (var i = 0; i &lt; 22; i++) {
     placeObj(i,coordx[i] ,coord
y[i] );
}
setTimeout(&quot;mouvement()&quot;,100)
}
if(document.getElementBy
Id) window.onload = mouvement;
&lt;/script&gt;
&lt;/head&gt;
&lt;body style=&
quot;background-color: rgb(255, 255, 255); background-image: url(Ciel053.jpg);&q
uot;&gt;

&lt;br&gt;&lt;br&gt;&lt;br&gt; 
Ici page web qui dans mon cas est d
e parler de la vie des abeilles des ruches installées dans les Batignolles.
&lt
;br&gt;&lt;br&gt;&lt;br&gt; 

&lt;/body&gt;
</pre>
