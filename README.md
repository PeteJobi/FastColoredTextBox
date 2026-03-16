FastColoredTextBox - FIXED
==================

This fork fixes a lot of bugs in the original repo, and adds some nice-to-have features. This was necessitated by my use of this component in [Regexer](https://github.com/PeteJobi/Regexer).

- Double-click + drag can now select multiple words, just like it works in notepad. Thanks to this [stackoverflow answer](https://stackoverflow.com/a/25708621/5920922).
- If AllowSeveralTextStyleDrawing is true, applying a style to characters will stack over whatever style was there before (as intended by original author), but if false, applying a style will override whatever style was there before. This fixes styling bugs I encountered.
- The auto-complete menu can now wrap around when navigating i.e if you press down when you're on the last item, you go to the first item. If you press up when you're on the first item, you go to last item.
- You can now set ToolTipDuration to 0 to show a tooltip indefinitely.
- You can choose to use a solid brush for the selected auto-complete item instead of the default gradient brush.
- You can remove the spacing for icons in the auto-complete menu by setting NoSpacingForIcons to true.
- If you want the auto-complete menu to show up again automatically after the user selects an item, set ReShowMenuAfterSelected to true.
- Fixed bug where tooltip shows up for items that don't have tooltips specified.
- If AutoWidth is set to true, the auto-complete menu will automatically resize its width to fit the items. Use AutoWidthExtraPadding to put some spacing between the right edge of the menu and the widest item. If any tooltip is shown while the menu resizes, it is reshown to adjust its position.
- Fixed bug with MaxToolTipSize. Before now, the MaxToolTipSize actually sets the width and height of the tooltip, even when the tooltip size is smaller than MaxToolTipSize. Now, MaxToolTipSize only limits the size of the tooltip when it would otherwise exceed it, and the tooltip text wraps around as expected.

Fast Colored TextBox is text editor component for .NET.
Allows you to create custom text editor with syntax highlighting.
It works well with small, medium, large and very-very large files.

It has such settings as foreground color, font style, background color which can be adjusted for arbitrarily selected text symbols. One can easily gain access to a text with the use of regular expressions. WordWrap, Find/Replace, Code folding and multilevel Undo/Redo are supported as well. 

![Fast Colored TextBox](http://www.codeproject.com/KB/edit/FastColoredTextBox_/fastcoloredtextbox2.png)

More details http://www.codeproject.com/Articles/161871/Fast-Colored-TextBox-for-syntax-highlighting

Nuget package https://www.nuget.org/packages/FCTB/
