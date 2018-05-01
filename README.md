# atom package install
 git install into `~/.atom`

`apm install --packages-file packages.list`


# fix your home keys on macs
https://damieng.com/blog/2015/04/24/make-home-end-keys-behave-like-windows-on-mac-os-x


Put below in this file `~/Library/KeyBindings/DefaultKeyBinding.dict`
May need a system reset for this to take effect.

```
{
    "\UF729"  = moveToBeginningOfParagraph:; // home
    "\UF72B"  = moveToEndOfParagraph:; // end
    "$\UF729" = moveToBeginningOfParagraphAndModifySelection:; // shift-home
    "$\UF72B" = moveToEndOfParagraphAndModifySelection:; // shift-end
    "^\UF729" = moveToBeginningOfDocument:; // ctrl-home
    "^\UF72B" = moveToEndOfDocument:; // ctrl-end
    "^$\UF729" = moveToBeginningOfDocumentAndModifySelection:; // ctrl-shift-home
    "^$\UF72B" = moveToEndOfDocumentAndModifySelection:; // ctrl-shift-end
}
```
