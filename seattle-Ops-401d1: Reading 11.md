How to Use Wireshark to Steal Passwords

Wireshark is a great tool to capture network packets, and we all know that people use the network to login to websites like Facebook, Twitter or Amazon. So there must be passwords or other authorization data being transported in those packets, and they may be obtained by using wireshark.
To gain access to someone’s password, you have to capture the network packets that contain the passwords or other credentials. And to capture the password you need to enable the promiscuous mode on the network card to be able to capture packets that are not meant to be received by your PC. This may sound complicated, but it basically works like this:
1.	All the packets on the network that actually arrive at your PCs (or Mac) will be inspected to check if they have a destination that matches the network card
2.	if the destination address is a match, the packets are destined for your PC and will be passed up to the CPU and processed
3.	if the destination address in the packet does not match the address of the network card the packets will simply be ignored and discarded
The third option shows that if your network card sees packets that are sent from other PCs to other servers (without your PC being involved at all), your card will not even really look at them except to find out that it doesn’t care. So if you want to grab stuff that others are sending to each other, you’ve got a problem.

Now, if you want to tell your network card “hey, accept everything. Forget the destination thing filtering, you need to enable a special mode on the network card. That mode is called “Promiscuous Mode”, and Wireshark does it automatically by default:

The bottom line is, you can’t get easy access to packets of other users, and you can’t decrypt the sessions that hold the things you want to see most. If at all, you can only look at unencrypted stuff, and only on networks you have administrative access to. 

