FinamTicksDownloader
====================

Ticks Downloader for Finam.ru
Limited to FORTS market only.

Description
-----------

[Standard download form][1] has several limitations like: period restrictions, file size restriction, user sometimes must wait too long for the file being prepared. In this repository you'll find my implementation of ticks downloader.

Usage
-----

    FinamTicksDownloader.exe <ticker> <timeframe> <from> <to>

Parameters:

* *ticker* - valid FORTS ticker (RTS, SBRF, Si, etc.)
* *timeframe* - valid timeframe. Supported timeframes are:
    * M5 - 5 minute timeframe
    * M1 - 1 minute timeframe 
    * ticks - tick data
* *from* - date to start from
* *to* - final date


Example 1:

    FinamTicksDownloader.exe RTS M5 2013.01.01 2013.12.31

Will download 5 minute candle series for RTS ticker since 1 January till 31 December 2013.

FAQ
---
Q: How can I merge all of .txt files into one?
A: Put a file named "*!all-to-one.bat*" to directory with .txt files. Run the bat-file, output result will be placed to "*!data.txt*". 

Like it?
--------

Please contribute!


  [1]: http://www.finam.ru/analysis/profile041CA00007/default.asp


