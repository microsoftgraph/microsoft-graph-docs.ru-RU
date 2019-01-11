---
title: Работа с отчетами об использовании Office 365 в Microsoft Graph
description: Microsoft Graph позволяет получить доступ к отчетам Office 365 и узнать, как сотрудники компании используют службы Office 365. Например, вы можете определить, кто использует службу по максимуму, а кому вообще не нужна лицензия Office 365.
localization_priority: Priority
ms.openlocfilehash: 1fcefc9c5fb5ba57551b75b74081ea60a1bcf1b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861336"
---
# <a name="working-with-office-365-usage-reports-in-microsoft-graph"></a>Работа с отчетами об использовании Office 365 в Microsoft Graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Microsoft Graph позволяет получить доступ к отчетам Office 365 и узнать, как сотрудники компании используют службы Office 365. Например, вы можете определить, кто использует службу по максимуму, а кому вообще не нужна лицензия Office 365.

## <a name="authorization"></a>Авторизация

Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения. Укажите разрешения, необходимые для доступа к отчетам, на портале Azure Active Directory (Azure AD). Дополнительные сведения см. в [справочнике по разрешениям Microsoft Graph](/graph/permissions-reference) и разделе [Разрешения для отчетов](/graph/permissions-reference#reports-permissions).

## <a name="changes-to-the-reports-apis"></a>Изменения на API отчетов

Исходный интерфейсы API отчетов были обновлены, можно вызвать API для конкретного представления, который будет вместо передачи параметра представления. Рекомендуется начать с помощью новых интерфейсов API в приложениях как можно скорее. В следующей таблице перечислены интерфейсы API, которые были удалены и новые интерфейсы API, заменены их.

| Исходный API            | Новые API                                  |
| :---------------------- | :--------------------------------------- |
| EmailActivity           | <ul><li>[getEmailActivityUserDetail](../api/reportroot-getemailactivityuserdetail.md);</li><li>[getEmailActivityCounts](../api/reportroot-getemailactivitycounts.md);</li><li>[getEmailActivityUserCounts](../api/reportroot-getemailactivityusercounts.md);</li></ul> |
| EmailAppUsage           | <ul><li>[getEmailAppUsageUserDetail](../api/reportroot-getemailappusageuserdetail.md);</li><li>[getEmailAppUsageAppsUserCounts](../api/reportroot-getemailappusageappsusercounts.md);</li><li>[getEmailAppUsageUserCounts](../api/reportroot-getemailappusageusercounts.md);</li><li>[getEmailAppUsageVersionsUserCounts](../api/reportroot-getemailappusageversionsusercounts.md);</li></ul> |
| MailboxUsage            | <ul><li>[getMailboxUsageDetail](../api/reportroot-getmailboxusagedetail.md);</li><li>[getMailboxUsageMailboxCounts](../api/reportroot-getmailboxusagemailboxcounts.md);</li><li>[getMailboxUsageQuotaStatusMailboxCounts](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md);</li><li>[getMailboxUsageStorage](../api/reportroot-getmailboxusagestorage.md);</li></ul> |
| Office365Activations    | <ul><li>[getOffice365ActivationsUserDetail](../api/reportroot-getoffice365activationsuserdetail.md);</li><li>[getOffice365ActivationCounts](../api/reportroot-getoffice365activationcounts.md);</li><li>[getOffice365ActivationsUserCounts](../api/reportroot-getoffice365activationsusercounts.md);</li></ul> |
| Office365ActiveUser     | <ul><li>[getOffice365ActiveUserDetail](../api/reportroot-getoffice365activeuserdetail.md);</li><li>[getOffice365ActiveUserCounts](../api/reportroot-getoffice365activeusercounts.md);</li><li>[getOffice365ServicesUserCounts](../api/reportroot-getoffice365servicesusercounts.md);</li></ul> |
| Office365GroupsActivity | <ul><li>[getOffice365GroupsActivityDetail](../api/reportroot-getoffice365groupsactivitydetail.md);</li><li>[getOffice365GroupsActivityCounts](../api/reportroot-getoffice365groupsactivitycounts.md);</li><li>[getOffice365GroupsActivityGroupCounts](../api/reportroot-getoffice365groupsactivitygroupcounts.md);</li><li>[getOffice365GroupsActivityStorage](../api/reportroot-getoffice365groupsactivitystorage.md);</li><li>[getOffice365GroupsActivityFileCounts](../api/reportroot-getoffice365groupsactivityfilecounts.md);</li></ul> |
| OneDriveActivity        | <ul><li>[getOneDriveActivityUserDetail](../api/reportroot-getonedriveactivityuserdetail.md);</li><li>[getOneDriveActivityUserCounts](../api/reportroot-getonedriveactivityusercounts.md);</li><li>[getOneDriveActivityFileCounts](../api/reportroot-getonedriveactivityfilecounts.md);</li></ul> |
| OneDriveUsage           | <ul><li>[getOneDriveUsageAccountDetail](../api/reportroot-getonedriveusageaccountdetail.md);</li><li>[getOneDriveUsageAccountCounts](../api/reportroot-getonedriveusageaccountcounts.md);</li><li>[getOneDriveUsageFileCounts](../api/reportroot-getonedriveusagefilecounts.md);</li><li>[getOneDriveUsageStorage](../api/reportroot-getonedriveusagestorage.md);</li></ul> |
| SharePointActivity      | <ul><li>[getSharePointActivityUserDetail](../api/reportroot-getsharepointactivityuserdetail.md);</li><li>[getSharePointActivityFileCounts](../api/reportroot-getsharepointactivityfilecounts.md);</li><li>[getSharePointActivityUserCounts](../api/reportroot-getsharepointactivityusercounts.md);</li><li>[getSharePointActivityPages](../api/reportroot-getsharepointactivitypages.md);</li></ul> |
| SharePointSiteUsage     | <ul><li>[getSharePointSiteUsageDetail](../api/reportroot-getsharepointsiteusagedetail.md);</li><li>[getSharePointSiteUsageFileCounts](../api/reportroot-getsharepointsiteusagefilecounts.md);</li><li>[getSharePointSiteUsageSiteCounts](../api/reportroot-getsharepointsiteusagesitecounts.md);</li><li>[getSharePointSiteUsageStorage](../api/reportroot-getsharepointsiteusagestorage.md);</li><li>[getSharePointSiteUsagePages](../api/reportroot-getsharepointsiteusagepages.md);</li></ul> |
| SfbActivity             | <ul><li>[getSkypeForBusinessActivityUserDetail](../api/reportroot-getskypeforbusinessactivityuserdetail.md);</li><li>[getSkypeForBusinessActivityCounts](../api/reportroot-getskypeforbusinessactivitycounts.md);</li><li>[getSkypeForBusinessActivityUserCounts](../api/reportroot-getskypeforbusinessactivityusercounts.md);</li></ul> |
| SfbDeviceUsage          | <ul><li>[getSkypeForBusinessDeviceUsageUserDetail](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md);</li><li>[getSkypeForBusinessDeviceUsageDistributionUserCounts](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md);</li><li>[getSkypeForBusinessDeviceUsageUserCounts](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md);</li></ul> |
| SfbOrganizerActivity    | <ul><li>[getSkypeForBusinessOrganizerActivityCounts](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md);</li><li>[getSkypeForBusinessOrganizerActivityUserCounts](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md);</li><li>[getSkypeForBusinessOrganizerActivityMinuteCounts](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md);</li></ul> |
| SfbParticipantActivity  | <ul><li>[getSkypeForBusinessParticipantActivityCounts](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md);</li><li>[getSkypeForBusinessParticipantActivityUserCounts](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md);</li><li>[getSkypeForBusinessParticipantActivityMinuteCounts](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md);</li></ul> |
| SfbP2PActivity          | <ul><li>[getSkypeForBusinessPeerToPeerActivityCounts](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md);</li><li>[getSkypeForBusinessPeerToPeerActivityUserCounts](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md);</li><li>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md);</li></ul> |
| YammerActivity          | <ul><li>[getYammerActivityUserDetail](../api/reportroot-getyammeractivityuserdetail.md);</li><li>[getYammerActivityCounts](../api/reportroot-getyammeractivitycounts.md);</li><li>[getYammerActivityUserCounts](../api/reportroot-getyammeractivityusercounts.md);</li></ul> |
| YammerDeviceUsage       | <ul><li>[getYammerDeviceUsageUserDetail](../api/reportroot-getyammerdeviceusageuserdetail.md);</li><li>[getYammerDeviceUsageDistributionUserCounts](../api/reportroot-getyammerdeviceusagedistributionusercounts.md);</li><li>[getYammerDeviceUsageUserCounts](../api/reportroot-getyammerdeviceusageusercounts.md);</li></ul> |
| YammerGroupsActivity    | <ul><li>[getYammerGroupsActivityDetail](../api/reportroot-getyammergroupsactivitydetail.md);</li><li>[getYammerGroupsActivityGroupCounts](../api/reportroot-getyammergroupsactivitygroupcounts.md);</li><li>[getYammerGroupsActivityCounts](../api/reportroot-getyammergroupsactivitycounts.md)</li></ul> |

## <a name="next-steps"></a>Дальнейшие действия

Ресурсы и API Microsoft Graph открывают новые способы взаимодействия с пользователями и контроля их работы. Чтобы узнать больше:

- Изучите подробнее методы и свойства ресурсов, наиболее полезных для вашего сценария.
- Опробуйте API в [песочнице Explorer](https://developer.microsoft.com/graph/graph-explorer).

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).
