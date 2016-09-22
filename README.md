Local Manifests
=================================


Instructions
---------------

Initializing:

First, create a folder to hold the source code: 

	mkdir ~/RR

Next..

	cd ~/RR

Initialize local repository:

    repo init -u https://github.com/ResurrectionRemix/platform_manifest.git -b lollipop5.1
    
Sync up:

	repo sync -j16 -f --force-sync --no-clone-bundle

Also add the local manifests:

    git clone https://github.com/DemoniacTeamDevs/local_manifests_hwY635 -b master .repo/local_manifests

Sync up:

	repo sync --force-sync --force-broken
	
-------------
 
_Building_
---------------

First:

	cd ~/RR

Second:

	. build/envsetup.sh

Third:

    brunch codename
    
Example:

    brunch hwY635


