<div align="center">

## Playing Music with Microsoft Direct X 9


</div>

### Description

This tutorial will give you the knowledge to use Microsoft Direct X 9 to play music in your applications. We will do this by using the Direct X 9 Audio class.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[EJ T](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/ej-t.md)
**Level**          |Beginner
**User Rating**    |3.5 (14 globes from 4 users)
**Compatibility**  |VB\.NET
**Category**       |[Graphics/ Sound](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/graphics-sound__10-15.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/ej-t-playing-music-with-microsoft-direct-x-9__10-913/archive/master.zip)





### Source Code

```
<style>
<!--
 /* Style Definitions */
 p.MsoNormal, li.MsoNormal, div.MsoNormal
	{mso-style-parent:"";
	margin:0in;
	margin-bottom:.0001pt;
	mso-pagination:widow-orphan;
	font-size:12.0pt;
	font-family:"Times New Roman";
	mso-fareast-font-family:"Times New Roman";}
a:link, span.MsoHyperlink
	{color:blue;
	text-decoration:underline;
	text-underline:single;}
a:visited, span.MsoHyperlinkFollowed
	{color:purple;
	text-decoration:underline;
	text-underline:single;}
span.SpellE
	{mso-style-name:"";
	mso-spl-e:yes;}
span.GramE
	{mso-style-name:"";
	mso-gram-e:yes;}
@page Section1
	{size:8.5in 11.0in;
	margin:1.0in 1.25in 1.0in 1.25in;
	mso-header-margin:.5in;
	mso-footer-margin:.5in;
	mso-paper-source:0;}
div.Section1
	{page:Section1;}
 /* List Definitions */
 @list l0
	{mso-list-id:5794755;
	mso-list-type:hybrid;
	mso-list-template-ids:-1140787024 67698705 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
@list l0:level1
	{mso-level-text:"%1\)";
	mso-level-tab-stop:.5in;
	mso-level-number-position:left;
	text-indent:-.25in;}
@list l1
	{mso-list-id:393624013;
	mso-list-type:hybrid;
	mso-list-template-ids:1229748470 67698705 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
@list l1:level1
	{mso-level-text:"%1\)";
	mso-level-tab-stop:.5in;
	mso-level-number-position:left;
	text-indent:-.25in;}
@list l2
	{mso-list-id:2108428849;
	mso-list-type:hybrid;
	mso-list-template-ids:136226568 67698705 67698713 67698715 67698703 67698713 67698715 67698703 67698713 67698715;}
@list l2:level1
	{mso-level-text:"%1\)";
	mso-level-tab-stop:.25in;
	mso-level-number-position:left;
	margin-left:.25in;
	text-indent:-.25in;}
ol
	{margin-bottom:0in;}
ul
	{margin-bottom:0in;}
-->
</style>
<!--[if gte mso 10]>
<style>
 /* Style Definitions */
 table.MsoNormalTable
	{mso-style-name:"Table Normal";
	mso-tstyle-rowband-size:0;
	mso-tstyle-colband-size:0;
	mso-style-noshow:yes;
	mso-style-parent:"";
	mso-padding-alt:0in 5.4pt 0in 5.4pt;
	mso-para-margin:0in;
	mso-para-margin-bottom:.0001pt;
	mso-pagination:widow-orphan;
	font-size:10.0pt;
	font-family:"Times New Roman";}
</style>
<![endif]-->
</head>
<body lang=EN-US link=blue vlink=purple style='tab-interval:.5in'>
<div class=Section1>
<p class=MsoNormal align=center style='text-align:center'>Microsoft Direct X 9
Audio</p>
<p class=MsoNormal align=center style='text-align:center'><o:p>&nbsp;</o:p></p>
<p class=MsoNormal>Overview:</p>
<p class=MsoNormal>This tutorial will give you the knowledge to use Microsoft
Direct X 9 to play music in your applications. We will do this by using the
Direct X 9 Audio class.</p>
<p class=MsoNormal><o:p>&nbsp;</o:p></p>
<p class=MsoNormal>Prerequisites:</p>
<p class=MsoNormal>You will need Microsoft Direct X 9 SDK and Microsoft Direct
X 9 Componentized VB</p>
<p class=MsoNormal>You can download them from: <b style='mso-bidi-font-weight:
normal'><o:p></o:p></b></p>
<p class=MsoNormal><b style='mso-bidi-font-weight:normal'><a
href="http://www.msdn.microsoft.com/library/default.asp?url=/downloads/list/directx.asp">http://www.msdn.microsoft.com/library/default.asp?url=/downloads/list/directx.asp</a><o:p></o:p></b></p>
<p class=MsoNormal><b style='mso-bidi-font-weight:normal'><o:p>&nbsp;</o:p></b></p>
<p class=MsoNormal>Start:</p>
<p class=MsoNormal style='margin-left:.5in;text-indent:-.25in;mso-list:l0 level1 lfo1;
tab-stops:list .5in'><![if !supportLists]><span style='mso-list:Ignore'>1)<span
style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span></span><![endif]>Open
Visual Basic.NET and create a new windows application</p>
<p class=MsoNormal style='margin-left:.5in;text-indent:-.25in;mso-list:l0 level1 lfo1;
tab-stops:list .5in'><![if !supportLists]><span style='mso-list:Ignore'>2)<span
style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span></span><![endif]><span
style='mso-spacerun:yes'> </span>The right click on references and click Add</p>
<p class=MsoNormal style='margin-left:.5in;text-indent:-.25in;mso-list:l0 level1 lfo1;
tab-stops:list .5in'><![if !supportLists]><span style='mso-list:Ignore'>3)<span
style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span></span><![endif]>Under
the .Net panel double click on <span style='mso-spacerun:yes'> </span><span
class=SpellE>Microsoft.DirectX</span> and <span class=SpellE>Microsoft.DirectX.AudioVidioPlayback</span></p>
<p class=MsoNormal style='margin-left:.5in;text-indent:-.25in;mso-list:l0 level1 lfo1;
tab-stops:list .5in'><![if !supportLists]><span style='mso-list:Ignore'>4)<span
style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span></span><![endif]>Now
click OK</p>
<p class=MsoNormal style='margin-left:.5in;text-indent:-.25in;mso-list:l0 level1 lfo1;
tab-stops:list .5in'><![if !supportLists]><span style='mso-list:Ignore'>5)<span
style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span></span><![endif]>Open
Form1 in code view and at the top, before the class declaration, type:</p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-size:10.0pt;font-family:"Courier New";color:blue'>Imports</span><span
style='font-size:10.0pt;font-family:"Courier New"'> <span class=SpellE>Microsoft.DirectX</span><o:p></o:p></span></p>
<p class=MsoNormal><span style='font-size:10.0pt;font-family:"Courier New";
color:blue'>Imports</span><span style='font-size:10.0pt;font-family:"Courier New"'>
<span class=SpellE>Microsoft.DirectX.AudioVideoPlayback</span><o:p></o:p></span></p>
<p class=MsoNormal style='margin-left:.5in;text-indent:-.25in;mso-list:l0 level1 lfo1;
tab-stops:list .5in'><![if !supportLists]><span style='mso-list:Ignore'>6)<span
style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span></span><![endif]>Then
go back to design view and add a button onto the form</p>
<p class=MsoNormal style='margin-left:.5in;text-indent:-.25in;mso-list:l0 level1 lfo1;
tab-stops:list .5in'><![if !supportLists]><span style='mso-list:Ignore'>7)<span
style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span></span><![endif]>Double
click the button and add the fowling code</p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-size:10.0pt;font-family:"Courier New"'><span
style='mso-spacerun:yes'>        </span><span style='color:blue'>Dim</span> <span
class=SpellE>OpenFile</span> <span style='color:blue'>As</span> <span
style='color:blue'>New</span> <span class=SpellE><span class=GramE>System.Windows.Forms.OpenFileDialog</span></span><span
class=GramE>(</span>) <span style='color:green'>'Create a dialog<o:p></o:p></span></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-size:10.0pt;font-family:"Courier New"'><span
style='mso-spacerun:yes'>        </span><span class=SpellE><span class=GramE>OpenFile.ShowDialog</span></span><span
class=GramE>(</span>) <span style='color:green'>'Shows the Dialog so the user
can select the file<o:p></o:p></span></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-size:10.0pt;font-family:"Courier New"'><span
style='mso-spacerun:yes'>        </span><span style='color:blue'>Dim</span> <span
class=SpellE>AudioFile</span> <span class=GramE><span style='color:blue'>As</span></span>
Audio <span style='color:green'>'Create a new audio object that can play audio
files<o:p></o:p></span></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-size:10.0pt;font-family:"Courier New"'><span
style='mso-spacerun:yes'>        </span><span class=SpellE>AudioFile</span> = <span
style='color:blue'>New</span> <span class=GramE>Audio(</span><span
class=SpellE>OpenFile.FileName</span>) <span style='color:green'>'Lodes the
file into the <span class=SpellE>AudioFile</span> Object<o:p></o:p></span></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-size:10.0pt;font-family:"Courier New";color:green'><o:p>&nbsp;</o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><o:p>&nbsp;</o:p></p>
<p class=MsoNormal style='margin-left:.5in;text-indent:-.25in;mso-list:l0 level1 lfo1;
tab-stops:list .5in'><![if !supportLists]><span style='mso-list:Ignore'>8)<span
style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span></span><![endif]>Click
play and enjoy</p>
<p class=MsoNormal>NOTE: When the file dialog comes up, only select an audio
file</p>
<p class=MsoNormal>(Another) NOTE: I know that this code could use some error
handling, and a better interface, but I just wanted to proved a way to play
music in Microsoft DirectX 9</p>
<p class=MsoNormal><o:p>&nbsp;</o:p></p>
<p class=MsoNormal>Please Vote and Comment<o:p></o:p></p>
</div>
```

