---
title: "What&#39;s New in BizTalk Server 2013 and 2013 R2 | Microsoft Docs"
ms.custom: ""
ms.date: "2016-03-29"
ms.prod: "biztalk-server-2013"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: bdb841f7-4aa9-45c9-a6f1-d527089fcc09
caps.latest.revision: 67
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# What&#39;s New in BizTalk Server 2013 and 2013 R2
See what's new and what is deprecated in [!INCLUDE[bts2013r2_md](../includes/bts2013r2-md.md)] and [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] 2013.
  
##  <a name="BKMK_NewR2"></a> What’s New in BizTalk Server 2013 R2?  
  
|Feature|Description|  
|-------------|-----------------|  
|Support for new versions of Windows OS, SQL Server, and Visual Studio|See [Hardware and Software Requirements for BizTalk Server 2013 and 2013 R2](../install-and-config-guides/hardware-and-software-requirements-for-biztalk-server-2013-and-2013-r2.md).|  
|Support for JSON|[!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] now supports sending and receiving JSON messages. [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] includes a wizard to generate XSD schema from a JSON instance, and an Encoder and Decoder component to use with custom pipelines. For more information, see [Processing JSON messages using BizTalk Server](../core/processing-json-messages-using-biztalk-server.md).|  
|Updates to the SB-Messaging adapter|SB Messaging adapter is enhanced to support SAS (Shared Access signature) based authentication, in addition to ACS.  With this new improvement, BizTalk Server can now also interact with the on-prem edition of Service Bus. For more information, see [SB-Messaging Adapter](../core/sb-messaging-adapter.md).|  
|Updates to the SFTP adapter|SFTP adapter now supports two-factor authentication and provides an option to specify a temporary folder while uploading/downloading large files. You can also select the Encryption cipher value specific to your target server. For more information, see [SFTP Adapter](../core/sftp-adapter.md).|  
|Updates to HL7 Accelerator|HL7 Accelerator now supports the following:<br /><br /> - Provides capability to include free-text data as part of the message that can be processed by the HL7 pipelines.<br /><br /> - 64-bit support for hosting Hl7 adapter.<br /><br /> See [What's New in BizTalk Accelerator for HL7](http://msdn.microsoft.com/library/ee409458\(v=bts.80\).aspx).|  
|BizTalk Health Monitor|BizTalk Health Monitor is a new BizTalk snap-in that helps monitor the health of your [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] environment. This snap-in can be added to the existing BizTalk Administration Console or can be run individually. Following are the features of BizTalk Health Monitor:<br /><br /> - Generate and view a health report<br /><br /> - Dashboard view for overall health of BizTalk environment<br /><br /> - Send e-mail notifications<br /><br /> - Schedule report collection<br /><br /> - Performance monitor integration with pre-loaded scenario-based performance counters<br /><br /> - Monitor multiple BizTalk environments<br /><br /> - Report management<br /><br /> For more information on BizTalk Health Monitor, see [Getting Started with BizTalk Health Monitor](http://go.microsoft.com/fwlink/?LinkId=403315) and [Overview of BizTalk Health Monitor](http://go.microsoft.com/fwlink/?LinkId=403316).|  
  
### Deprecated List  
  
|Program|Status|Replacement|  
|-------------|------------|-----------------|  
|RFID Mobile|Removed|None|  
|RFID Server|Deprecated|None|  
|SharePoint SSOM/Web Service adapter|Deprecated|Use the CSOM (Client Side Object Model) option.<br /><br /> [Windows SharePoint Services Adapter](../core/windows-sharepoint-services-adapter.md)<br /><br /> [Appendix B: Install the Microsoft SharePoint Adapter](../install-and-config-guides/appendix-b-install-the-microsoft-sharepoint-adapter.md)|  
|SOAP adapter|Deprecated|[WCF-BasicHttp Adapter](../core/wcf-basichttp-adapter.md)|  
|Old SQL adapter|Deprecated|WCF-based SQL adapter in the [!INCLUDE[adapterpacknoversion](../includes/adapterpacknoversion-md.md)]|  
|UDDI|Deprecated|None|  
  
> [!IMPORTANT]
>  Some of these deprecated features may be found in newer versions of BizTalk. In these scenarios, consider the following:  
>   
>  -   The feature may be used internally within BizTalk and is not meant to be used by customer solutions. It is not supported in customer solutions.  
> -   The interfaces may have been modified by Microsoft and may not be publicly available.  
  
##  <a name="BKMK_New"></a> What’s New in BizTalk Server 2013?  
 The following features are added in BizTalk Server 2013.  
  
 **[!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] on Azure IaaS**  
  
|Feature|Description|  
|-------------|-----------------|  
|Configure [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] on a [!INCLUDE[winazure](../includes/winazure-md.md)][!INCLUDE[vm](../includes/vm-md.md)]|See [Create a BizTalk Virtual Machine in Windows Azure](http://msdn.microsoft.com/library/jj572843.aspx).|  
|Create a [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] Group on a [!INCLUDE[winazure](../includes/winazure-md.md)][!INCLUDE[vm](../includes/vm-md.md)]|See [Create the BizTalk Group Prerequisites](http://msdn.microsoft.com/library/jj248711.aspx) and [Configure the BizTalk Group](http://msdn.microsoft.com/library/jj572845.aspx).|  
  
 **[!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] on Premises**  
  
|Feature|Description|  
|-------------|-----------------|  
|Per Core License Model|BizTalk Server 2013 is per core. SQL Server 2012 is also per core. [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] 2010 and previous versions are per-processor.<br /><br /> When running [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] on processors with four cores or less, the license cost remains consistent with [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] 2010. Core licenses are priced at one quarter the cost of a processor license. When running servers with higher capacity processors, licensing cost are increased due to the increased power of the hardware.<br /><br /> To help determine the number of licenses you may need, a PowerShell cmdlet in *C:\Program Files (x86)\Microsoft BizTalk Server 20xx\SDK\Utilities\LicenseUsageTracking* is available.<br /><br /> Helpful links:<br /><br /> [BizTalk Server 2013 Pricing & Editions](http://www.microsoft.com/biztalk/pricing.aspx)<br /><br /> [Understand BizTalk Server 2013 Licensing](http://blogs.biztalk360.com/understand-biztalk-server-2013-licensing/)|  
|Support for new Adapters|[!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] provides new adapters to extend connectivity of [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] applications to [!INCLUDE[winazure](../includes/winazure-md.md)]. [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] also provides updates to SharePoint adapter that gives users the option of choosing between using the client-side or server-side object model for connecting to a SharePoint server. [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] includes a new adapter to send and receive messages from an SFTP server.|  
|Tracking dependencies between artifacts|[!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] updates the [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] Administraton console to provide a UI-driven experience to see how different [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] artifacts such as orchestrations, send ports, receive locations, etc. are dependent on each other. For more information, see [Tracking Dependencies Between Artifacts in a BizTalk Server Application](../core/tracking-dependencies-between-artifacts-in-a-biztalk-server-application.md)|  
|Integrated ESB Toolkit|ESB Toolkit is now integrated as part of the [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] setup. Also, the ESB Toolkit configuration experience is simplified to facilitate quick start time for users. For more information, see [Install and Configure the Microsoft BizTalk ESB Toolkit](../install-and-config-guides/install-and-configure-the-microsoft-biztalk-esb-toolkit.md)|  
|Support for new versions of Windows OS, SQL Server, and Visual Studio|See [Hardware and Software Requirements for BizTalk Server 2013 and 2013 R2](../install-and-config-guides/hardware-and-software-requirements-for-biztalk-server-2013-and-2013-r2.md)|  
|Updates to the supported EDI schemas|[!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] introduces support for the following EDI schemas:<br /><br /> -                     **X12** – 5040, 5050, 6020, 6030<br /><br /> - **EDIFACT** – D06A, D06B, D07A, D07B, D08A, D08B, D09A, D09B, D10A, D10B<br /><br /> -                     **HL7** – 2.51 message support added<br /><br /> -                     **SWIFT** – 2012 Message Pack<br /><br /> The schemas are included in the [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] installation package. You can download the installation package from [http://go.microsoft.com/fwlink/p/?LinkId=258228](http://go.microsoft.com/fwlink/p/?LinkId=258228).|  
|Mapper uses XSLCompiledTransform|The Mapper uses the XSLCompiledTransform class. Previous [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] versions used the XslTransform class, which is obsolete. The XSLCompiledTransform class provides performance enhancements, including:<br /><br /> - Once the Load method completes successfully, the Transform method can be called simultaneously from multiple threads.<br /><br /> - The new XSLT processor compiles the XSLT style sheet to a common intermediate format. Once the style sheet is compiled, it can be cached and reused.<br /><br /> More information at [What the Mapper Updates Mean for You](http://www.quicklearn.com/blog/2013/05/24/what-the-biztalk-server-2013-mapper-updates-mean-for-you/) and [XslCompiledTransform Class](https://msdn.microsoft.com/library/system.xml.xsl.xslcompiledtransform.aspx).|  
|Configurable Dynamic Send Port Handler|When creating a Dynamic Send Port, an adapter Send Handler is configurable for *every* installed adapter. Includes both One-Way and Solicit-Response Dynamic Ports. In previous BizTalk versions, a dynamic send port uses the adapter’s default host.<br /><br /> [Dynamic Send Port Handler is Configurable](../core/dynamic-send-port-handler-is-configurable.md) provides more information.|  
|Ordered Delivery|In previous BizTalk versions with scenarios where ordered delivery uses multiple endpoints, the slowest adapter type is the maximum speed. This behavior directly impacts HL7 solutions. When using the MLLP adapter, acknowledgements (ACK) are required. Delays can occur because an ACK must be received before the next message is sent.<br /><br /> In [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)], the next message can be sent without waiting for an ACK from the previous message. When the ACK arrives, it is internally correlated/connected with its message.|  
|Support Tools|Support Tools is automatically installed with BizTalk: *C:\Program Files (x86)\Microsoft BizTalk Server 20xx\SDK\Utilities\Support Tools*.<br /><br /> Tools include:<br /><br /> - BizTalk Assembly Checker<br /><br /> - MsgBox Viewer<br /><br /> - PSSDiagForBizTalk<br /><br /> - Internet shortcut to BizTalk Terminator download|  
|PowerShell Provider|The [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] PowerShell Provider is in *C:\Program Files (x86)\Microsoft BizTalk Server 2013\SDK\Utilities\PowerShell*.<br /><br /> For previous BizTalk versions, there’s a CodePlex PowerShell Provider at [http://psbiztalk.codeplex.com/](http://psbiztalk.codeplex.com/).|  
|BAM Alerts|If BizTalk Server 2013 uses [!INCLUDE[sqlserver2012](../includes/sqlserver2012-md.md)], Database Mail is needed to use BAM Alerts. If BizTalk Server uses SQL Server 2008 R2, SQL Server Notification Services is needed to use BAM Alerts.<br /><br /> [BAM Alerts](../install-and-config-guides/prepare-your-computer-for-installation.md#BKMK_BAMAlerts) provides more information.|  
  
> [!IMPORTANT]
>  When [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] and [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] are installed on separate computers, Distributed Transaction Coordinator (MS DTC) handles the transactions between the computers. As a result, the [!INCLUDE[btsSQLServerNoVersion](../includes/btssqlservernoversion-md.md)] AlwaysOn feature is not supported with [!INCLUDE[bts2013r2](../includes/bts2013r2-md.md)] and 2013. Starting with [!INCLUDE[bts2016](../includes/bts2016-md.md)], the AlwaysOn feature **is** supported. See [What's New in BizTalk Server 2016](../install-and-config-guides/what-s-new-in-biztalk-server-2016.md) for the details.  
  
### Known Issues  
 [Known issues in BizTalk Server 2013](http://support.microsoft.com/kb/2954101)