<HTML>
<HEAD>
<TITLE>ZOOM-IN AND ZOOM-OUT</TITLE>
</HEAD>
<BODY BGCOLOR="#554477">
<marquee>
       <FONT COLOR="#660000" size="20">Zooming In....Zooming Out Image....</FONT>
</marquee>
<img src="https://www.gimp-forum.net/attachment.php?aid=3820.jpeg" name="slide" height=600 width=675 border=5>
<Script>
var i=300;
var j=50;
var k;
var zoomspeed=500;
function zooming()
{
   if(i==300)
  {
       k=0;
  }
  if(i==0)
  {
       k=1;
  }
  if(k==0)
  {
        document.images.slide.width=i;
        document.images.slide.height=i;
       i=i-j;
  }
  else
  {
       document.images.slide.width=i;
       document.images.slide.height=i;
       i=i+j;
  }
  setTimeout("zooming()", zoomspeed);
}
zooming();
</SCRIPT>
</BODY>
</HTML>
