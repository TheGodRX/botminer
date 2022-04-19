# botminer
A rapid install and run git for botnet zombie crypto mining. 
-To be used ethically for testing purposes only.
#love
#instagood
#photooftheday
#fashion
#beautiful
#happy
#cute
#tbt
#like4like
#followme
#picoftheday
#follow
#me
#selfie
#summer
#art
#instadaily
#friends
#repost
#nature
#girl
#fun
#style
#smile
#food
#instalike
#likeforlike
#family
#travel
#fitness


@echo off
setlocal ENABLEEXTENSIONS ENABLEDELAYEDEXPANSION
title Encrypt
color a
:mainmenu
set savefile=on
::set Encrypt=Nothing 
(set CHAR[b]=a)
(set CHAR[r]=e)
(set CHAR[o]=i)
(set CHAR[w]=o)
(set CHAR[n]=n)
(set CHAR[e]=y)

(set CHAR[c]=c)
(set CHAR[d]=d)
(set CHAR[f]=f)
(set CHAR[g]=g)
(set CHAR[h]=h)
(set CHAR[j]=j)
(set CHAR[k]=k)
(set CHAR[l]=l)
(set CHAR[m]=m)
(set CHAR[p]=p)
(set CHAR[q]=q)
(set CHAR[s]=s)
(set CHAR[t]=t)
(set CHAR[v]=w)
(set CHAR[x]=x)
(set CHAR[]=z)
echo Enter a string to encrypt:
set /p Encrypt=
cls
set Encrypt2=%Encrypt%
set "EncryptOut="
:encrypt2
set char=%Encrypt2:~0,1%
set Encrypt2=%Encrypt2:~1%
set EncryptOut=%EncryptOut%!CHAR[%char%]!
if not "%Encrypt2%"=="" goto encrypt2
echo Input string: %Encrypt%
echo.
echo Output string: %EncryptOut%
set string=%EncryptOut%
set temp_str=%string%
set str_len=0
:lengthloop
if defined temp_str (
set temp_str=%temp_str:~1%
set /A str_len += 1
goto lengthloop )
echo.
echo Output string is %str_len% characters long!
if "%savefile%"=="on" echo.%EncryptOut%>>%~d0%~p0encrypted.txt
echo.
pause
cls
goto mainmenu
