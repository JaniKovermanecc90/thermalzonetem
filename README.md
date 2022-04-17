# thermalzonetem
= ObjGet("winmgmts:\\" &amp; @ComputerName &amp; "\root\wmi") $aClasses = $WMI.SubclassesOf()      For $class In $aClasses         If StringInStr($class.Path_.Path, "thermalzonetemp") Then ConsoleWrite($class.Path_.Path &amp; @CRLF)     Next
