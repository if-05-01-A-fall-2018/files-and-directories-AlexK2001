1. **FAT Main Memory Requirements**
* Disk = 2.684*10^(11) B, Block Size = 1024 B; => 262.144.000 Blöcke
* 262.144.000
* 2^(16) = 65536 B; 2^(32) = 4,3 Mrd. B => The table entry has a size of 32 Bit.
* 262.144.000 Blöcke * 32 Bit / 8 Bit = 1.048.576.000 => The finally size is 1000 MB.

2. **Random Access of Files**
* a
* 107.834.590 Position; Block size = 1024 => 107.834.590 / 1024 ~ 105.308 You have to skip to the block 105.308

3. **UFS (i-node) File Size**
* 32 Bit block numbers = 4Bytes
###1KB
  Block size = 1024B
  1024B / 4 = 256
  Direct = 10 * 1024B = 10.240
  Single = 256 * 1024B = 262.144B
  Double = 256^2 * 1024B = 67.108.864B
  Triple = 256^3 * 1024B = 17.179.869.184B
  Max size = Direct + Single + Double + Triple = 17.247.250.432B ~ 16GB

###4KB
  Block size = 4096B
  32 / 8 = 4
  4096B / 4 = 1024B
  Direct = 10 * 4096B = 40960B
  Single = 1024B * 4096B = 4194304B
  Double = 1024B^2 * 4096B = 4294967296B
  Triple = 1024B^3 * 4096B =
  Max size = Direct + Single + Double + Triple = 4.402.345.713.664B ~ 4GB

4. **UFS File Size**
  disk Block size 512B
  512 / 4 = 128
  FileSize = 5GB

  * Direct = 10 * 512B = 5.120B
  Single = 1024B * 512B = 65.536B
  Double = 1024B^2 * 512B = 8.388.608
  Triple = 1024B^3 * 512B = 1.073.741.824
  Max size = Direct + Single + Double + Triple = 1.082.201.088 ~ 1GB

  Weil Max size kleiner als ein File ist. => A Block size of 1024 wäre besser da hätten wir 16GB.

  * Man braucht eine Block size of 1024. Dann ist alles Gut.
