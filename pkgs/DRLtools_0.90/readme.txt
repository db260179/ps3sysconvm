
    _   _   __________  _________________                                                
E _| |_| |_ \______   \/   _____/\_____  \ ___.    .__                                   
F|_   _   _| |    |>  /\_____  \    (__  < \_ |__  |  |   __ __ _______ _____   ___.__.
N _| |_| |_  |     __/ _____/   \ ____/   \ | __ \ |  |  |  |  \\_  __ \\__  \ <   |  |
E|_   _   _| |    |   /         //        / | \_\ \|  |__|  |  / |  | \/ / __ \_\___  |
T  |_| |_|   |____|  /_______  //______  /  |___  /|____/|____/  |__|   (____  // ____|  
  __________.____________  ____                                                           
  \         \\           \|    | ___________________   ________   .____       _________    
   \______   \\______     \    | \__    ___/\_____  \  \_____  \  |    |     /   _____/    
    |    |    \|         _/    |   |    |    /   |   \  /   |   \ |    |     \_____  \     
    |    |     \    ,     \    |___|    |   /    |    \/    |    \|    |___  /        \    
   /     `     /    |      \       |____|   \_______  /\_______  /|_______ \/_______  /    
  /_________  /|____|____  /_______  \              \/         \/         \/        \/v0.90
 ===========\/===========\/=========\/=====================================================
Project #PS3bluray
DRLtools v0.90 for PS3 01.01.2011


BACKGROUND
Our quest to restore BD playback for those PS3s that lost it after downgrading continues. Unfortunately our project suffered a serious setback last week when one of our discoveries was prematurely leaked: A potentially harmful and incomplete method to restore BD playback was disclosed by an attention-seeking individual. It should be noted that the fix in question is only a "band-aid" solution to the problem. There is a very real possibility of future drive revocation resulting in PERMANENTLY broken playback! However, to make using it safer for those who wish to apply it, we have created this collection of DRL Tools. In the meantime we are continuing to work on a permanent and simple solution for all PS3s.

The tools in the suite are:
	- DRLbackup v0.90 (PS3 pkg used to backup DRL1 / DRL2 files to a USB drive)
	- DRLgen v0.90 (Windows .net 2.0 application to derive DRL1 / DRL2 files from an MKB_RO.inf file)
	- DRLcopy v0.90 (PS3 pkg to restore previously backed-up DRL1 / DRL2 files or to copy derived DRL1 / DRL2 files from DRLgen)


HOW IT WORKS
Each Blu-Ray movie contains a Media Key Block (MKB) as part of its copy protection scheme. Newer movies feature higher MKBs; the latest one is MKB v20. Addtionally, each BD movie has a unique encrypted title key. Both are stored inside the AACS/MKB_RO.inf file of each disc. Fixing BD playback requires exact knowledge of which was the first instance of the highest MKB played so far. DRLgen can be used to identify the Blu-Ray movie with the highest MKB, and then create replacement DRL1/2 files for your PS3 which then restore BD playback.


REQUIREMENTS
1. A means to access Blu-Ray title discs to gather the AACS/MKB_RO.inf file, a Blu-Ray drive in a Mac / Windows PC makes the process easiest. Alternatively, SAK v1.0 can be installed as an OtherOS on the PS3 with firmware 3.15 or lower to accomplish this task.
2. Explicit knowledge of EVERY blu-ray title the blu-ray drive has played and the MKB versions of those discs. WARNING: While you can safely check every BD's MKB with DRLgen, you should limit the number of attempts of installing DRLs on the PS3, as the full details of the AACS "traitor tracking system" are not well known.
3. A FAT32 USB storage device to store and retrieve MKB_RO.inf and DRL files.


DETAILED INSTRUCTIONS
Full instructions are available on the Project #PS3bluray wiki http://ps3bluray.info/?title=DRLtools


ABOUT THE TOOLS
DRLgen is a new and SAFER utility that uses the MKB_RO.inf from a Blu-Ray disc to derive correctly formatted DRL1 and DRL2 files easily every time. No difficult hex editing or byte-counting is involved.  It is important to note that DRLgen uses the AACS' specification for the MKB format and does not simply assume DRL records start at a specific position and are of a specific length. The previously leaked information makes all these assumptions and is flat out INCORRECT in many situations today, and is NOT future proof and could lead to permanently broken playback.

DRLbackup, previously released, has been updated to work in cooperation with the other two tools.  As a best practice, a backup of the DRL1 / DRL2 files should be made prior to any system downgrade.  Use in conjunction with DRLcopy for a completely recreatable process to downgrade your Large NAND PS3 and restore Blu-Ray playback in the future.
Note: The location of saved files has changed, users of the older version of the tool should place their saved DRL files into a 'PS3bluray' folder in the root of the USB storage device for compatability with the new DRLcopy tool.

DRLcopy is a new PS3 tool that uses the output of the new version of DRLbackup (or properly located DRL backups from the previous version) and/or the derived DRL files from DRLgen to restore your blu-ray functionality after a firmware downgrade.



WHAT YOU CAN DO TO HELP:
We are still in need of a MKB v13 DRL1. If the highest movie you have played on your (non downgraded) PS3 is MKB v13, please create a backup of your DRL1 with DRLbackup v0.90 and email it to projectps3bluray@gmail.com
Thank you!




_________________________________________________________________________________________

ABOUT THIS PROJECT:
Project #PS3bluray was formed on efnet by a group of enthusiasts after the Blu-Ray playback problem was discovered, our goal is to find a permanent solution. This is a group effort; we are neither seeking individual fame nor money.
For serious discussion, join us in our IRC-channel #PS3bluray on efnet.

Thanks to everyone involved!
Your time and hard work is very much appreciated.

