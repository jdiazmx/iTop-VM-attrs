# iTop-VM-attrs
some complementry fields for Virtual Machines

# Goal
We use a lot of complementary attributes for our Virtual Machines. Probably useless in another context.

The fields added are :
* Location (as for a physical device, we want to know in wich datacenter the virtul machine resides)
* S_UUID (kind of a serial number, helps in data consolidation -two VM can have the same name, but normally not the same UUID)
* S_FUNCTION, S_Contact_1, S_Contact_2,S_Usage,S_Comment, S_Project are all business informations
* S_CREATOR is the name of the person who deployed the VM
* S_EndOfLife is the date we supposely could destroy the VM (after a validation !)
* S_Template is the name of the Source Template used for the deployment
* S_Backup are some informations for our Backup Tool
* S_LastBootDate and S_CurentHypervisor are informations collected dynamically and not tracked in the history of the VM
* S_OS_Version and S_OS_Distributor are informations about the OS version but from the Linux perspective (again from a Data Synchronisation)

# Installation
As for all my extentions, just download the zip file, and copy the 'schirrms-...' directory in your extensions directory, then rerun the setup as usual.
