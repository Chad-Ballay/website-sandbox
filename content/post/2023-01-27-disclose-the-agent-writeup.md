---
title: Disclose The Agent - Writeup
date: 2023-01-27T11:51:35.497Z
description: Letsdefend.io Challenge Solution
---


D﻿ecided to start back up with some basic training after someone mentioned LetsDefend.io.  The site impressed me.  Here is a writeup on one of their public facing challenges that kind of shows what to expect.

[D﻿isclose the Agent](https://app.letsdefend.io/challenge/disclose-the-agent)

Premise is that you've got a PCAP file and you need to identify who the secret agent is, what they are doing, and who they are communicating with.  

1. G﻿rab the PCAP file. [https://api.letsdefend.io/download/downloadfile/smtpchallenge.zip](<1. https://api.letsdefend.io/download/downloadfile/smtpchallenge.zip>) Pass: 321
2. L﻿oad it into WireShark.  

   ![](/img/screenshot-from-2023-01-27-05-57-30.png)

   1. What is the email address of Ann's secret boyfriend?

      L﻿ooked through the pcap file for all the From: and To: SMTP packets.  From there I was able to see this.  [mistersecretx@aol.com](mailto:mistersecretx@aol.com)

      ![](/img/screenshot-from-2023-01-31-22-41-35.png)