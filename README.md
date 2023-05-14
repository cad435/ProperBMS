# ProperBMS
Proper "slim" BMS, based around the S-8254

As I was tinkering around a lot with Li-Ion cells (not LiPo yet) the last year I did quite a few hours research protecting me and my cells. I looked for (an bought) one of those "simple" protection circuits. It seems there are only quite two versions of them available:

First: "chained DW01" style BMS's. Although they will be working 99% of the time it is just... bad... (1% failure is just too much if a possible failure involves lithium fire). DW01 is really only meant to be used on one single cell - not on a 3S to 12S (I saw it as high as 17S) pack. They often come with a passive balancing circuitry, wich is desirable. Cells generally should be matched (thus, decreasing the need for balancing), but they always drift ever so slightly. Having a little passive balancing to bring them back together from time to time therefore seems to be a good option.

Second: BMS wich use actual pack protection IC's like the S-8254, BQ7790500 or the BM3451, wich is decent and should generally be prefered. Sadly though, they don't offer any balancing at all. I tried to source some, but really only found some 100A 4S, wich for most of my projects is too much Amps and often I only use 3S Packs.

So I finally threw a board together, building a circuitry around the ABLIC S-8254AAVFT-TB-S (Ablic), with a passive bleedof balancing around the HY2213-BB3A
