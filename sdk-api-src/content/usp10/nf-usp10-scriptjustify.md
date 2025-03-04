---
UID: NF:usp10.ScriptJustify
title: ScriptJustify function (usp10.h)
description: Creates an advance widths table to allow text justification when passed to the ScriptTextOut function.
helpviewer_keywords: ["ScriptJustify","ScriptJustify function [Internationalization for Windows Applications]","_win32_ScriptJustify","intl.scriptjustify","usp10/ScriptJustify"]
old-location: intl\scriptjustify.htm
tech.root: Intl
ms.assetid: 9419eb80-cd33-4974-a1f1-d43276cb7a91
ms.date: 12/05/2018
ms.keywords: ScriptJustify, ScriptJustify function [Internationalization for Windows Applications], _win32_ScriptJustify, intl.scriptjustify, usp10/ScriptJustify
f1_keywords:
- usp10/ScriptJustify
dev_langs:
- c++
req.header: usp10.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Usp10.lib
req.dll: Usp10.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Usp10.dll
- Ext-MS-Win-GDI-Internal-Desktop-L1-1-0.dll
- GDI32.dll
- GDI32Full.dll
api_name:
- ScriptJustify
targetos: Windows
req.typenames: 
req.redist: Internet Explorer 5 or later on Windows Me/98/95
ms.custom: 19H1
---

# ScriptJustify function


## -description


Creates an advance widths table to allow text justification when passed to the <a href="https://docs.microsoft.com/windows/desktop/api/usp10/nf-usp10-scripttextout">ScriptTextOut</a> function.


## -parameters




### -param psva [in]

Pointer to an array, of length indicated by <i>cGlyphs</i>, containing <a href="/windows/win32/api/usp10/ns-usp10-script_visattr">SCRIPT_VISATTR</a> structures. Each structure contains visual attributes for a glyph in the line to process.


### -param piAdvance [in]

Pointer to an advance widths array, of length indicated by <i>cGlyphs</i>, obtained from a previous call to <a href="https://docs.microsoft.com/windows/desktop/api/usp10/nf-usp10-scriptplace">ScriptPlace</a>.


### -param cGlyphs [in]

Count of glyphs for the arrays indicated by <i>psva</i> and <i>piAdvance</i>. This parameter also indicates the count of glyphs for the output parameter <i>piJustify</i>.


### -param iDx [in]

Width, in pixels, of the desired change, either an increase of decrease.


### -param iMinKashida [in]

Minimum width of a kashida glyph to generate.


### -param piJustify [out]

Pointer to a buffer in which this function retrieves an array, of length indicated by <i>cGlyphs</i>, containing justified advance widths. The justified widths are sometimes called "cell widths" to distinguish them from unjustified advance widths.


## -returns



Returns 0 if successful. The function returns a nonzero HRESULT value if it does not succeed. The application can test the return value with the <b>SUCCEEDED</b> and <b>FAILED</b> macros.




## -remarks



See <a href="https://docs.microsoft.com/windows/desktop/Intl/displaying-text-with-uniscribe">Displaying Text with Uniscribe</a> for a discussion of the context in which this function is normally called.

This function provides a simple implementation of multilingual justification. It establishes the amount of adjustment to make at each glyph position on the line. It interprets the <a href="/windows/win32/api/usp10/ns-usp10-script_visattr">SCRIPT_VISATTR</a> array generated by a call to <a href="https://docs.microsoft.com/windows/desktop/api/usp10/nf-usp10-scriptshape">ScriptShape</a>, giving top priority to kashida. The function uses interword spacing if no kashida points are available. It uses intercharacter spacing if no interword points are available.

<div class="alert"><b>Note</b>  Sophisticated text formatters might generate their own delta dx array by combining formatter-specific features with the information retrieved by <a href="https://docs.microsoft.com/windows/desktop/api/usp10/nf-usp10-scriptshape">ScriptShape</a> in the <a href="/windows/win32/api/usp10/ns-usp10-script_visattr">SCRIPT_VISATTR</a> array.</div>
<div> </div>
The application should pass the justified advance widths generated by <b>ScriptJustify</b> to <a href="https://docs.microsoft.com/windows/desktop/api/usp10/nf-usp10-scripttextout">ScriptTextOut</a> in the <i>piJustify</i> parameter.

<b>ScriptJustify</b> creates a justified array containing updated advance widths for each glyph. When an advance width for a glyph is increased, the extra width is rendered to the right of the glyph, with a white space or, for Arabic text, a kashida.

<div class="alert"><b>Note</b>  Kashida insertion occurs to the right of the glyph to justify visually. Microsoft Word and Microsoft PowerPoint use this concept. Any change in the kashida placement algorithm should accompany a change in the corresponding <a href="https://docs.microsoft.com/windows/desktop/api/usp10/nf-usp10-scripttextout">ScriptTextOut</a> handler for a particular script, for example, the Arabic TextOut justification handler.</div>
<div> </div>
Sometimes the application tries to handle glyphs that cannot be justified, in which case the <b>uJustification</b> member of <a href="/windows/win32/api/usp10/ns-usp10-script_visattr">SCRIPT_VISATTR</a> is set to SCRIPT_JUSTIFY_NONE. In this case, <b>ScriptJustify</b> copies the input array indicated by <i>piAdvance</i> to the output array indicated by <i>piJustify</i> and returns S_FALSE to the application.

<div class="alert"><b>Important</b>  Starting with Windows 8: To maintain the ability to run on Windows 7, a module that uses Uniscribe must specify Usp10.lib before gdi32.lib in its library list.</div>
<div> </div>



## -see-also




<a href="https://docs.microsoft.com/windows/desktop/Intl/displaying-text-with-uniscribe">Displaying Text with Uniscribe</a>



<a href="/windows/win32/api/usp10/ns-usp10-script_visattr">SCRIPT_VISATTR</a>



<a href="https://docs.microsoft.com/windows/desktop/api/usp10/nf-usp10-scriptplace">ScriptPlace</a>



<a href="https://docs.microsoft.com/windows/desktop/api/usp10/nf-usp10-scriptshape">ScriptShape</a>



<a href="https://docs.microsoft.com/windows/desktop/api/usp10/nf-usp10-scripttextout">ScriptTextOut</a>



<a href="https://docs.microsoft.com/windows/desktop/Intl/uniscribe">Uniscribe</a>



<a href="https://docs.microsoft.com/windows/desktop/Intl/uniscribe-functions">Uniscribe Functions</a>
 

 

