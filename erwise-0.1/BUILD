#!/bin/sh
#
echo "****** Building erwise"

(cd Xl ; xmkmf -DHasGcc3=YES)
(cd erwise ; xmkmf -DHasGcc3=YES)
(cd HText ; xmkmf -DHasGcc3=YES)
(cd Ui ; xmkmf -DHasGcc3=YES)
(cd Cl/WWWLibrary ; xmkmf -DHasGcc3=YES)
(cd Cl ; xmkmf -DHasGcc3=YES)

xmkmf -DHasGcc3=YES

make CDEBUGFLAGS=-fcommon

echo "****** Done."
