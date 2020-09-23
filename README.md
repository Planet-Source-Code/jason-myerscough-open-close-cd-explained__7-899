<div align="center">

## Open\_Close\_CD\_Explained


</div>

### Description

This is a break down tutorial explaining how to open and close the Cd rom.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Jason Myerscough](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/jason-myerscough.md)
**Level**          |Intermediate
**User Rating**    |3.6 (18 globes from 5 users)
**Compatibility**  |Delphi 7, Delphi 6, Delphi 5
**Category**       |[Windows API Call/ Explanation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/windows-api-call-explanation__7-39.md)
**World**          |[Delphi](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/delphi.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/jason-myerscough-open-close-cd-explained__7-899/archive/master.zip)





### Source Code

The program is too short to upload so i thought it would be better to create a tutorial :P
<br>
<br>
<font coloe=#0099ff>Before you can make the CD open or close you have to add
 <b>MMSYSTEM</b> to the <b>uses</b> section of the code.
 The function used to open the CD is <b>MciSendString;</b>
 The function takes for arguments which are:
 <b>lpszCommand:</b><i> This command is need to tell the function what to do</i>
 <b>lpszReturnString:</b><i> This holds the string returned by the command</i>
 <b>cchReturn:</b><i> The size argument is the size of the return string.</i>
 <b>hwndCallback:</b><i> is the window that called texecuted the command ie the form.</i>
 Since we dont want the function to return anything we want it to perform a
 task we set "lpszReturnString" to nil and "cchReturn" to 0
 The command to open the CD is <b>"Set CDAudio Door Open"</b>
 The command to close the CD is the same apart from you change 'Open' to
 'Closed'
<br>
<br>
<table align=center border=1 bordercolor=navy cellspacing=0 cellpadding=0>
<tr>
<td bgcolor=navy><font color=white> Open/close CD</font></td>
</tr>
<tr>
<td>  MciSendString('Set CDAudio Door Open', nil, 0, form1.Handle);</td>
</tr>
<tr>
<td> 
 MciSendString('Set CDAudio Door Closed', nil, 0, form1.Handle);</td>
</tr>
</table>
Rate The tutorial, if not for the content then for the se of html tables :D - MyerSoft site comming soon

