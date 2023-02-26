
# Welcome to the one and only original, universal SystemRW / SuperRW featuring MakeRW / ro2rw by lebigmac for Android 10+
# Also known as: read-only-2-read/write super partition converter (ro2rw), MOUNT-RW, FORCE-RW, THE-REAL-RW, FULL-RW, EXT4-RW, EROFS-RW, EROFS-2-RW, F2FS-RW, F2FS-2-RW, EROFS-2-EXT4-CONVERTER, F2FS-2-EXT4-CONVERTER, Super Partition Resizer / Flasher / Patcher, SYSTEM-RW / PRODUCT-RW / VENDOR-RW / ODM-RW, REAL ROOT, FULL ROOT, ROOT ENHANCER, BRUTE FORCE RW, Auto-Debloater and many more aliases!​

# NOTE: Full F2FS-RW patch for Samsung devices scheduled release date: 1. quartal 2023
# Samsung users get your next-gen Galaxy devices ready! 2023 will be a very good year for ALL RW enthousiasts :D

# ------------------------------------------------------------------------------------------------------------

# The prophecy has finally been fullfilled!
# Making Android ten years younger!
# Inspiring a whole generation of talented developers and empowering the open source community.
# The Pandora's Box has been fully unlocked at last!
# The genie has been unleashed from within the bottle!
# Sesame! Open up now!
# Let the Olympic Android System Modding Games (OASMG) begin!
# The power is now in YOUR hands! And don't forget:
# With great power comes great responsibility!

# --------------------------------------------------------------------------------------------------------------

# If you like this project then please feel free to donate to the original developer lebigmac by visiting the official link below and clicking the [ DONATE ] button. Thank you very much! Your support is very much appreciated and it will help me to pay my horrendous electricity bills so I can continue working on this project (and adding new features) + keep it ad-free & create many more amazing new projects like this! :D

# *** OFFICIAL SYSTEM RW / SUPER RW FEAT. MAKERW / RO2RW BY LEBIGMAC HOMEPAGE *** @ 
# ==================================================================================================

#                   http://www.systemrw.com

# ==================================================================================================

# DISCLAIMER: This proprietary software is donationware (it can only exist thanks to donations by people like YOU) and was provided for free as-is only for personal, educational and non-commercial purposes without any kind of implied warranty or support whatsoever. By viewing and using this software you agree to the following terms:
# Under no circumstances shall the original author be held responsible for any damages (such as data loss for example) that may arrise from the (inappropriate) use of this software.
# All responsibility, liability and risk lies with the end-user. You hereby agree not to abuse this software (or parts thereof) for illegal or immoral purposes.
# The end-user is allowed to use this software for free for his/her own personal, educational, non-commercial, legal purposes.
# If the end-user wishes to use this software (or parts thereof) for commercial purposes then please rent a commercial usage license at the official link above. Thank you very much! Your generous donations are very much appreciated and will help me to pay my horrendous electricity bills so I can continue working on this project (adding new features) + keep it ad-free & create many more amazing new projects like this! :D
# This software can be re-uploaded to 3rd party websites indefinitely as long as this software itself (or parts thereof) are not modified by the end-user.
# The end-user is NOT allowed to steal, imitate, hack, crack, hex-edit, modify, decompile and/or abuse this software (or any parts thereof) in any way.
# This readme file shall not be deleted or modified under any circumstances!

# --------------------------------------------------------------------------------------------------------------

# WARNING! NEVER TRUST THE SOFTWARE OF THIEVES!
# This whole project (or parts thereof) was stolen, hacked and/or abused by brigudav, leegarchat & co!
# [ insert name of other shameless thief here ]
# Always download unmodified & original SystemRW / SuperRW feat. MakeRW / ro2rw by the original author lebigmac from OFFICIAL DOWNLOAD LINK ABOVE!

# --------------------------------------------------------------------------------------------------------------

# Original author: lebigmac
# Creation date: February 2021
# Last updated: January 2023

# Requirements: rooted Android 10 or newer & at least 10+ GB free space on device for dumping data

# Description: A program for all Android power users that wish to make their read-only Android 10+ device fully read/write-able in order to debloat & further customize their device.

# IMPORTANT INFO: Make sure /data partition is decrypted and mounted properly before launching program!
# Automatic installation from recovery: Simply boot device into recovery and swipe to install the flashable zip file (do NOT check zip signature verification)!
# Manual installation: extract sysrw_[VERSION]_flashable.zip and copy sysrw_[VERSION] folder into /data/local/tmp/
#  run this command to make the program executable: chmod +x /data/local/tmp/sysrw_[VERSION]/sysrw (replace [VERSION] with the actual version)

# OPTIONAL PROGRAM ARGUMENTS: (replace x with your custom value)
#  in=x : Specify existing super image as input [OPTIONAL]
#  Omitting this parameter is equivalent to using in=@auto

#  out=x : Specify patched super image output file path [OPTIONAL]
#  If omitted, default output value is ./img/super_patched.bin (path is relative to program)

#  size=x : Specify extra size (in MB) to be added to each sub-partition of super image or use size=@auto for auto-resizing all sub-partitions inside new super image! [OPTIONAL]
#  If omitted, default size value is @auto and all sub-partitions will be auto-resized.

# -r : Specify whether or not the patched super image should be output in raw file format [OPTIONAL]
#  Omitting this parameter will create a sparse patched super image by default

# USAGE EXAMPLES:
#  adb shell
#  su
#  cd /data/local/tmp/sysrw_1.36
#  chmod +x ./sysrw

#  ./sysrw
#  ./sysrw -r
#  ./sysrw in=@auto
#  ./sysrw in=@auto -r
#  ./sysrw in=@auto out=@auto
#  ./sysrw in=@auto out=@auto -r
#  ./sysrw in=@auto out=@auto size=@auto
#  ./sysrw in=@auto out=@auto size=@auto -r
#  ./sysrw in=./img/super_original.bin
#  ./sysrw in=./img/super_original.bin size=15
#  ./sysrw in=./img/super_original.bin out=./img/super_patched.bin
#  ./sysrw in=./img/super_original.bin out=./img/super_patched.bin size=@auto
# EXPERT EXAMPLE: (WARNING! This will flash the raw patched super.img directly to your super block device! Do this at your own risk in recovery mode only!)
#  ./sysrw in=../path/to/super.img out=`realpath /dev/block/by-name/super` -r

# --------------------------------------------------------------------------------------------------------------

# Please post your feedback, suggestions and your Olympic Android System Mods (OASMG) @ the official SystemRW/SuperRW feat. MakeRW/ro2rw links below :

# *** OFFICIAL SYSTEM RW / SUPER RW FEAT. MAKERW / RO2RW BY LEBIGMAC HOMEPAGE *** @ 
# ==================================================================================================

#                   http://www.systemrw.com

# ==================================================================================================

# TROUBLESHOOTING:
# If you experience error 73 or bootloop you can try the included sysrw_repair or undo_bootloop scripts in the ./repair subfolder! Good luck!

# --------------------------------------------------------------------------------------------------------------

# Hello and shout-outs goes out to all the people that contributed positively to the creation of this amazing project from scratch (you know who you are). A huge thank you to every single one of you!
# Without your enthousiastic support we would still be stuck in read-only mode forever! How boring! Full R/W mode is much more fun ;) Enjoy fully debloating and further customizing your fully read/write-able next-gen Android device! <3

# Shout-outs to : @Yuki1001 @foxhackerr @Mr Hassan @frxhb @HemanthJabalpuri @012345678 @2mkl @abhinav453 @abs_khafan_19 @abszy @abuzar_uzair @a.dibacco @ahk31 @amurec @aiecxs @anatolii-orsk @andarxapi @andyyan @angel495 @Anhlatuananh @anubarak @arifn @arik80 @articul8madness @assasinx54 @aungthay.plastic @ayoub @b4minee @barryviper @bear263 @bienvanhoang @bingdiancn @blazingkahn35 @brepro1 @bseosbseos @captianxlab @chairman011 @chintocool @chron0s @condor323 @d4ylight @danmann @dbx13 @deathshot9 @deltaquarti @Devill2014 @diogen78 @dragonfire1024 @drdani @email44841 @erickesquia @everyyest @f1^ter @facebooook @fgacko @fire7ly @flashfire5606 @flypatriot @francescohub @gammarayxda @gearmaker @gentisz @gessler2244 @gimmyy @greenspoof @gsser @harpreet @hippie459mn @hippoman @ianmansant @isitolo @jazonx @jc-b @jesuschrist @jhayprince @kafeinsiz @kalhiro @Keven11 @kolibass @kostmatyj @kpykpy @kratos574 @krissrmx @liam_l @m3nty @magnificent_y @masricky @mclaude774 @megiss @minhdat_vo @mions_lv @mishak750 @miustone @mrsergey @munchy_cool @munjeni @nad4 @newdwarf @ninjaperv @islam @nissegura @nttuan @oneironaut2002 @overlimit1 @pandavova @peach-pit @peter1212 @vadlamani @pouya_rezaei @quazero @r00tme @rahamatulla @rakoncwy @rayman95 @rbdomgam @revokke @reynaldio19 @rhewins @ricardo_cruz @rmx3370 @romkazor @sampei @samy2015 @sarbazg @sarychev.rescue @simich007 @simonfoxcoon @simora.lesha @staljin @svoc @swedishforenger @tha_mechanic @thelavip @the_magnificent_y @the_tablet @tids2k @toreton @ufanet @uvs @uvzen @version-x @vishal @vulcany @warhawk971 @xatornet @general @xen423 @xiaoleng @x-root @yasfatft @yoshijulas @zachariahpope @Евгений1 and many more!

# Thanks to all project supporters! You are simply the best! <3

# And thank you God for sending me this angel from above and for giving me the strength to reclaim my original and unique RW project for Android from the claws of these ruthless cyber pirates!

