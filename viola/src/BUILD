# If this script dosn't work...
# type:  setenv IMAKECPP /usr/bin/cpp
# before executing BUILD
#
echo "****** Building W3 library"
(cd libWWW; ./BUILD)

echo "****** Building XPA library"
(cd libXPA/src; xmkmf -DHasGcc3=YES; make)

echo "****** Building XPM library"
(cd libXPM; xmkmf -DHasGcc3=YES; make)

#echo "****** Building GIF library"
#(cd libGIF; xmkmf -DHasGcc3=YES; make)

echo "****** Building IMG library"
(cd libIMG; xmkmf -DHasGcc3=YES; make libIMG.a)

echo "****** Building libStyle library"
(cd libStyle; xmkmf -DHasGcc3=YES; make)

echo "****** Building Viola"
(cd viola; xmkmf -DHasGcc3=YES; make)
#(cd viola; xmkmf; make -e 'CC=purify cc' -e 'CDEBUGFLAGS=-g')
#(cd viola; xmkmf; make -e 'CDEBUGFLAGS=-g -ldl')

echo "****** Building ViolaWWW-Motif"
(cd vw; xmkmf -DHasGcc3=YES; make)
#(cd vw; xmkmf; make -e 'CC=purify cc' -e 'CDEBUGFLAGS=-g')
#(cd vw; xmkmf; make -e 'CDEBUGFLAGS=-g -ldl')

echo "****** Done."
