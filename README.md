# DiskDoubler Test Files

This repository contains a collection of minimal, legally redistributable
DiskDoubler archives suitable for inclusion in test suites for programs that
incorporate DiskDoubler extraction functionality.

**See Also:**
[StuffIt Test Files](https://github.com/ssokolow/stuffit-test-files/),
[RAR Test Files](https://github.com/ssokolow/rar-test-files)

## Explain

Since there are no free tools I know of for creating
[DiskDoubler](https://en.wikipedia.org/wiki/DiskDoubler) archives, and it's
important to be able to integration-test systems that use `lsar` and `unar` from
The Unarchiver's open-source
[command-line tools](https://theunarchiver.com/command-line) to process legacy
archives, I decided to step up and create some legally redistributable
DiskDoubler archives.

## Contents

The loose files are DiskDoubler-compressed data forks, as should be extractable
using a non-Macintosh tool such as the The Unarchiver's CLI tools.

The `.dd` files are archives created using DiskDoubler's "Combine" option and
are created directly from the uncompressed source files, not from the
DiskDoubler-compressed individual files.

`sources.dd377.ad.dd.1` and `sources.dd377.ad.dd.2` are a copy of
`sources.dd377.ad.dd`, split into pieces using DiskDoubler's apparently
proprietary "Split" option which The Unarchiver CLI tools v1.10.1 can't make
heads or tails of either directly or when manually `cat`ed together.

The StuffIt archives are complete (data fork, resource fork, HFS creator and
type codes) representations of the individually DiskDoubler-compressed files in
the following formats, compressed using the copy of StuffIt Deluxe 4.5 which I
purchased for my
[StuffIt Test Files](https://github.com/ssokolow/stuffit-test-files/) repository
and confirmed to be extractable using The Unarchiver's CLI tools as built from
source for the Ubuntu Linux 20.04 LTS package repository.

The meaning of the folder and archive names are as follows:

- `sources.dd377.ad`: DiskDoubler 3.7.7 configured to use AutoDoubler A
  compression mode.
- `sources.dd377.ads`: DiskDoubler 3.7.7 configured to use AutoDoubler B
  compression mode.
- `sources.dd377.dda`: DiskDoubler 3.7.7 configured to use DiskDoubler A
  compression mode.
- `sources.dd377.ddb`: DiskDoubler 3.7.7 configured to use DiskDoubler B
  compression mode.

The source files are the same public domain ones created for my StuffIt Test
Files repository, with a fresh set being extracted from `sources.sit` on my
Power Mac G4 for each variant of DiskDoubler compression.

## "How Do I Know These Are Legal?"

First, the contents are the same test files I created from scratch and released
into the public domain for my
[RAR test files](https://github.com/ssokolow/rar-test-files) and
[StuffIt Test Files](https://github.com/ssokolow/stuffit-test-files/)
repositories, plus a TIFF file converted from the PNG file using a copy of
GraphicConverter 5.9.5 for Classic MacOS that has been registered using a
license key
[now given away for free](https://www.lemkesoft.de/en/products/graphicconverter/download/download-old-versions/)
by the original developer.

**My copy of DiskDoubler was purchased as sealed New Old Stock** on eBay, and my
used copy of StuffIt Deluxe 4.5, purchased on eBay, has a passage in its license
that allows for the transfer of the license:

> 3. OTHER RESTRICTIONS. You may not rent or lease the SOFTWARE, but **you may
>    transfer the SOFTWARE and accompanying written materials on a permanent
>    basis provided you retain no copies and the recipient agrees to the terms
>    of this agreement**. [...]

Since I don't have a BinHex encoder on the drive I use for StuffIt Deluxe 4.5, I
had to swap to my StuffIt Deluxe 6.5 drive to BinHex-encode the `.dd` "Bundled"
archives. (Big thanks to whoever invented IDE-to-SD Card adapters.)

That version of StuffIt doesn't _explicitly_ say the license is transferable,
but it should be implicit in the passage I've bolded here:

> The Software is owned by Aladdin Systems and is protected by United States
> copyright laws and international treaty provisions. **Therefore, you must
> treat the Software like any other copyrighted material (e.g., a book or
> musical recording).** Paying the license fee allows you the right to use one
> copy of the Software on a single computer. You may not network the Software or
> otherwise use it or make it available for use on more than one computer at the
> same time. You may not rent or lease the Software, nor may you modify, adapt,
> translate, reverse engineer, decompile, or disassemble the Software. If you
> violate any part of this agreement, your right to use this Software terminates
> automatically and you must then destroy all copies of the Software in your
> possession.

All are running on a genuine Power Mac G4 Quicksilver 2002 which I own:

![Order Info for DiskDoubler 3.7.7](photos/dd377_order_info.jpg)

![Picture of DiskDoubler 3.7.7](photos/dd377.jpg)

![Picture of StuffIt 4.5 Deluxe](photos/stuffit45mac.jpg)

![Picture of StuffIt 6.5 Deluxe](photos/stuffit65mac.jpg)

![Picture of Power Mac G4](photos/powermacg4.jpg)

---

## Future Plans

The option to create a self-extracting archive seems to only be available via
the INIT which crashes Finder under MacOS 9. Revisit this when I have a
Macintosh capable of running System 6 or 7.

I also do not currently know whether newer versions of DiskDoubler implemented
different and incompatible file formats as has been the case several times with
StuffIt. I _do_ know that I don't have any older copies of DiskDoubler which
implement the "Old B" compression listed in DiskDoubler 3.7.7's Convert dialog
and that "Sigma" is greyed out... apparently because it had something to do with
the
[DoubleUp](https://archive.org/details/TNM_DiskDoubler_data_compression_card_for_Macinto_20171214_0204)
NuBus hardware accelerator.

(Given how rare that NuBus card must be, and how I don't currently even _have_ a
NuBus-based Macintosh, I don't anticipate creating test files for those any time
soon.)

## License

By design, the files within the archives have been created from scratch and are
minimally novel in the hope that they will be ineligible for copyright.

I hereby release anything in these archives that I _do_ hold copyright to into
the public domain using the Creative Commons
[CC0](http://creativecommons.org/publicdomain/zero/1.0/) public domain
dedication.

<p xmlns:dct="http://purl.org/dc/terms/" xmlns:vcard="http://www.w3.org/2001/vcard-rdf/3.0#">
  <a rel="license"
     href="http://creativecommons.org/publicdomain/zero/1.0/">
    <img src="http://i.creativecommons.org/p/zero/1.0/88x31.png" style="border-style: none;" alt="CC0" />
  </a>
  <br />
  To the extent possible under law,
  <span resource="[_:publisher]" rel="dct:publisher">
    <span property="dct:title">Stephan Sokolow</span></span>
  has waived all copyright and related or neighboring rights to
  <span property="dct:title">DiskDoubler Test Files</span>.
This work is published from:
<span property="vcard:Country" datatype="dct:ISO3166"
      content="CA" about="[_:publisher]">
  Canada</span>.
</p>
