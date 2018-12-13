---
title: Журнал изменений Microsoft Graph
description: Этот журнал содержит сведения об изменениях Microsoft Graph, в том числе API Microsoft Graph для конечных точек версии 1.0 и бета-версии.
ms.openlocfilehash: e8b4671d527bac65d1855c21d7612077ed18203e
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222662"
---
# <a name="changelog-for-microsoft-graph"></a>Журнал изменений Microsoft Graph

Этот журнал содержит сведения об изменениях Microsoft Graph, в том числе API Microsoft Graph для конечных точек версии 1.0 и бета-версии.

Дополнительные сведения об известных проблемах с API Microsoft Graph см. в статье [Известные проблемы](known-issues.md).

## <a name="december-2018"></a>Декабрь 2018 года

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлен новый тип ресурса [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).|
| Дополнение | бета | Добавлено свойство `createdDateTime` для ресурса [organization](/graph/api/resources/organization?view=graph-rest-beta).|
| Дополнение | 1.0 | Добавлен метод `memberOf` для получения сведений о непосредственном [участии](/graph/api/device-list-memberOf?view=graph-rest-1.0) для [устройств](/graph/api/resources/device?view=graph-rest-1.0). Этот метод был добавлен для получения списка участий, включая вложенные участия.|

### <a name="microsoft-teams-apis"></a>API Microsoft Teams

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |бета| Представлен новый тип ресурса [teamsTemplate](/graph/api/resources/teamstemplate?view=graph-rest-beta).|
|Дополнение |бета| Представлен новый тип ресурса [teamSpecialization](/graph/api/resources/teamspecialization?view=graph-rest-beta).|
|Дополнение |Бета-версия| Добавлены свойства isFavoriteByDefault, mail и webUrl для [канала](/graph/api/resources/channel?view=graph-rest-beta).|
|Дополнение |Бета-версия| Добавлено свойство displayName для [команды](/graph/api/resources/team?view=graph-rest-beta)|
|Дополнение |Бета-версия| Добавлены свойство описание для [команды](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |Бета-версия| Добавлены свойство классификация для [команды](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |Бета-версия| Добавлены свойство [специализация](/graph/api/resources/teamspecialization?view=graph-rest-beta) для [команды](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |Бета-версия| Добавлено свойство [видимость](/graph/api/resources/teamvisibilitytype?view=graph-rest-beta) для [группы](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |Бета-версия| Добавлено свойство [шаблон](/graph/api/resources/teamstemplate?view=graph-rest-beta) для [группы](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |Бета-версия| Добавлено семейство владельцы для [группы](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |Бета-версия| Представлен новый элемент перечисления unknownFutureValue для объекта teamVisibilityType.|
|Дополнение |Бета-версия| Представлен новый элемент перечисления unknownFutureValue для объекта giphyRatingType.|
|Дополнение |Бета-версия| Представлен новый элемент перечисления unknownFutureValue для объекта teamsAsyncOperationType.|
|Дополнение |Бета-версия| Представлен новый элемент перечисления unknownFutureValue для объекта teamsAsyncOperationStatus.|
|Дополнение |Бета-версия| Представлен новый элемент перечисления unknownFutureValue для объекта teamsAppDistributionMethod.|
|Дополнение |Бета-версия| Представлен новый тип ресурса [/teamsTemplates](/graph/api/resources/teamstemplate?view=graph-rest-beta).|
|Дополнение | 1.0 | Добавлена поддержка разрешений администратора для операций c [командами](/graph/api/resources/team?view=graph-rest-1.0), [каналами](/graph/api/resources/channel?view=graph-rest-1.0) и [вкладками](/graph/api/resources/teamstab?view=graph-rest-1.0). |

### <a name="privileged-identity-management-apis"></a>API управления привилегированными пользователями

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета-версия | Добавлено свойство `registeredRoot` для объекта [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta).|
| Изменение | Бета-версия | Переименовано свойство `onboardDateTime` объекта [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) для `registeredDateTime`.|
| Дополнение | Бета-версия | Добавлено новое действие [регистрация ресурсов](/graph/api/governanceresource-register?view=graph-rest-beta).|
| Удаление | Бета-версия | Удалено свойство`isPermanent` для объекта [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta).|
| Удаление | Бета-версия | Удалено свойство `roleAssignmentStartDateTime` для объекта [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta).|
| Удаление | Бета-версия | Удалено свойство `roleAssignmentEndDateTime` для объекта [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta).|

## <a name="november-2018"></a>Ноябрь 2018 г.

### <a name="data-policy-operations-api"></a>API операций с политикой данных

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлено новое свойство **progress** для [dataPolicyOperation](/graph/api/resources/dataPolicyOperation?view=graph-rest-beta). Оно указывает ход выполнения операции.

### <a name="microsoft-teams-apis"></a>API Microsoft Teams

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |1.0| Представлен новый тип ресурса [team](/graph/api/resources/team?view=graph-rest-1.0).|
|Дополнение |1.0| Представлен новый тип ресурса [channel](/graph/api/resources/channel?view=graph-rest-1.0).|
|Дополнение |1.0| Представлен новый тип ресурса [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-1.0).|
|Дополнение |1.0| Представлен новый тип ресурса [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-1.0).|
|Дополнение |1.0| Представлен новый тип ресурса [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-1.0).|
|Дополнение |1.0| Представлен новый тип ресурса [teamsAsyncOperation](/graph/api/resources/teamsasyncoperation?view=graph-rest-1.0). |
|Дополнение |1.0| Представлен новый сложный тип [teamGuestSettings](/graph/api/resources/teamguestsettings?view=graph-rest-1.0). |
|Дополнение |1.0| Представлен новый сложный тип [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-1.0). |
|Дополнение |1.0| Представлен новый сложный тип [teamMessagingSettings](/graph/api/resources/teammessagingsettings?view=graph-rest-1.0). |
|Дополнение |1.0| Представлен новый сложный тип [teamFunSettings](/graph/api/resources/teamfunsettings?view=graph-rest-1.0). |
|Дополнение |1.0| Представлено новое действие [Клонирование объекта команды](/graph/api/team-clone?view=graph-rest-1.0). |
|Дополнение |1.0| Представлено новое действие [Архивация объекта команды](/graph/api/team-archive?view=graph-rest-1.0).|
|Дополнение |1.0| Представлено новое действие [Распаковка объекта команды](/graph/api/team-unarchive?view=graph-rest-1.0). |
|Дополнение         | бета          | Добавлена поддержка разрешений приложений для [клонирования объекта команды](/graph/api/team-clone?view=graph-rest-beta) |
|Дополнение |бета| Представлен объект [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta), заменяющий /teams/{id}/apps с некоторыми отличиями в полезных данных. |
|Дополнение |бета| Представлен объект [/appCatalogs/teamsApps/{id}/appDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta), заменяющий свойство версии в [/appCatalogs/teamsApps/{id}](/graph/api/resources/teamsapp?view=graph-rest-beta). |
|Изменение   |бета| Тип объекта [/appCatalogs/teamsApps](/graph/api/resources/teamsapp?view=graph-rest-beta) переименован с teamsCatalogApp на teamsApp. |
|Изменение   |бета| Тип свойства distributionMethod в [/appCatalogs/teamsApps](/graph/api/resources/teamsapp?view=graph-rest-beta) переименован с teamsCatalogAppDistributionMethod на teamsAppDistributionMethod  |
|Удаление |бета| teamsCatalogAppDistributionMethod переименован на teamsAppDistributionMethod  |
|Дополнение |бета| Представлен объект [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta), заменяющий /teams/{id}/apps с некоторыми отличиями в полезных данных. |
|Дополнение |бета| Добавлено свойство displayName в объект [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) |
|Дополнение |бета| Добавлено свойство messageId в объект [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) |
|Дополнение |бета| Добавлено свойство teamsApp в объект [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) |
|Дополнение |бета| Представлен новый тип ресурса [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta).|
|Дополнение |бета| Представлен новый тип ресурса [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta).|
|Дополнение |бета| Представлен новый тип ресурса [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta).|
|Дополнение |бета| Представлен новый элемент перечисления hiddenMembership для объекта teamVisibilityType.|
|Дополнение |бета| Представлен новый элемент перечисления createTeam для объекта teamsAsyncOperationType.|
|Дополнение |бета| Представлен новый элемент перечисления teamsAppDistributionMethod.|
|Дополнение |бета| Представлено новое действие обновления приложения в [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta). |

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | 1.0 | Добавлено действие [forceDelete](/graph/api/domain-forcedelete?view=graph-rest-1.0) для объекта [domains](/graph/api/resources/domain?view=graph-rest-1.0).|
| Дополнение | бета | Добавлен новый метод transitiveMembers для объекта [groups](/graph/api/group-list-transitivemembers?view=graph-rest-beta). Этот метод возвращает плоский список элементов, включая вложенные элементы.|
| Дополнение | бета | Добавлен новый метод transitiveMemberOf для объектов [users](/graph/api/user-list-transitivemembersof?view=graph-rest-beta), [groups](/graph/api/group-list-transitivemembersof?view=graph-rest-beta), [devices](/graph/api/device-list-transitivemembersof?view=graph-rest-beta) и [service principals](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta).|
| Дополнение | бета | Добавлен метод memberOf, чтобы получить сведения о непосредственном [участии](/graph/api/device-list-members?view=graph-rest-beta) для устройств. Этот метод добавлен для получения списка участий, включая вложенные участия.|
| Дополнение | бета | Добавлены новые свойства в объект [users](/graph/api/resources/user?view=graph-rest-beta): **faxNumber**, **onPremisesDistinguishedName** и **otherMails**.|
| Дополнение | бета | Добавлено свойство **forceChangePasswordNextSignInWithMfa** в сложный тип [passwordProfile](/graph/api/resources/passwordprofile?view=graph-rest-beta).|

### <a name="reports-apis"></a>API отчетов

| Тип изменения | Версия                                    | Описание                              |
| :---------- | :----------------------------------------- | :--------------------------------------- |
| Дополнение    | Бета-версия Microsoft Graph для Китая под управлением 21Vianet | Добавлены следующие API:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta);<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta);<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta);<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta);<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta);<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta);<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta);<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta);<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta);<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta);<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta);<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta);<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta);<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta);<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta);<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta);<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta);<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta);<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta);<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta);<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta);<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta);<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta);<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta);<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta);<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta);<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta);<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta);<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta);<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta);<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta);<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta);<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta);<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta);<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta);<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta);<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta); |

### <a name="directory-apis"></a>API каталогов
| Тип изменения | Версия                                    | Описание                              |
| :---------- | :----------------------------------------- | :--------------------------------------- |
| Дополнение    | бета | Добавлены свойства externalUserState и externalUserStateChangeDateTime в объект [user](/graph/api/resources/user?view=graph-rest-beta).|

## <a name="october-2018"></a>Октябрь 2018 г.

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлен новый метод transitiveMembers для объекта [groups](/graph/api/group-list-transitivemembers?view=graph-rest-beta). Этот метод возвращает плоский список элементов, включая вложенные элементы.|
| Дополнение | бета | Добавлен новый метод transitiveMemberOf для объектов [users](/graph/api/user-list-transitivemembersof?view=graph-rest-beta), [groups](/graph/api/group-list-transitivemembersof?view=graph-rest-beta), [devices](/graph/api/device-list-transitivemembersof?view=graph-rest-beta) и [service principals](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta).|
| Дополнение | бета | Добавлен метод memberOf, чтобы получить сведения о непосредственном [участии](/graph/api/device-list-members?view=graph-rest-beta) для устройств. Этот метод добавлен для получения списка участий, включая вложенные участия.|
| Дополнение | бета | Добавлены новые свойства в объект [users](/graph/api/resources/user?view=graph-rest-beta): **faxNumber**, **onPremisesDistinguishedName** и **otherMails**.|

### <a name="riskyusers-apis"></a>API RiskyUsers

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |бета| Добавлен [API riskyUsers](/graph/api/resources/riskyuser?view=graph-rest-beta), представляющий пользователей Azure AD в состоянии риска, как определено защитой идентификации Azure AD. |


### <a name="signin-apis"></a>API входа

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Изменение   |бета| Свойство `conditionalAccessPolicies` переименовано на `appliedConditionalAccessPolicy`.|
|Дополнение |бета| Представлены дополнительные свойства риска в [API входа](/graph/api/resources/signin?view=graph-rest-beta), в том числе `riskDetail`, `riskLevelAggregated`, `riskLevelDuringSignIn`, `riskEventTypes` и `riskState`.|
|Дополнение |бета| Представлены дополнительные свойства входа в [API входа](/graph/api/resources/signin?view=graph-rest-beta), в том числе `authenticationProcessingDetails`, `originalRequestID`, `isInteractive`, `tokenIssuerName`, `tokenIssuerType`, `correlationId` и `processingTimeinMilliseconds`.|
|Удаление   |бета| Удалено свойство `isRisky`.|

## <a name="october-2018"></a>Октябрь 2018 г.

### <a name="delta-query"></a>Запрос изменений

| **Тип изменения** | **Версия** | **Описание**                  |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | бета   | Добавлена возможность [запроса изменений](delta-query-overview.md) для объекта [directoryObject](/graph/api/directoryobject-delta?view=graph-rest-beta) |
| Изменение      | 1.0 и бета  | Другое поведение при возвращении измененных свойств только в отклике JSON для объектов [users](/graph/api/user-delta?view=graph-rest-1.0) и [groups](/graph/api/group-delta?view=graph-rest-1.0). |
| Дополнение    | 1.0   | Добавлена функция [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) для [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0), чтобы поддерживать [отслеживание изменений с помощью запроса изменений](delta-query-overview.md). |

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлено свойство **licenseAssignmentStates** в объект [User](/graph/api/resources/user?view=graph-rest-beta) для [лицензирования на основе групп](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|
| Дополнение | бета | Добавлен ресурс **licenseAssignmentState** для [лицензирования на основе групп](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|
| Дополнение | бета | Добавлены свойства **assignedLicenses**, **licenseProcessingState**, **hasMembersWithLicenseErrors** и **membersWithLicenseErrors** в объект [Group](/graph/api/resources/group?view=graph-rest-beta) для [лицензирования на основе групп](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|

### <a name="microsoft-intune-apis"></a>API Microsoft Intune

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлено свойство **tenantLockdownRequireNetworkDuringOutOfBoxExperience** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0)|
|Дополнение|1.0|Добавлено свойство **v12_0** для сложного типа [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0)|
|Дополнение|бета|Добавлено свойство **lastReportAggregationDateTime** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены новые объекты:<br/>[intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[deviceAndAppManagementAssignedRoleIds](/graph/api/resources/intune-rbac-deviceandappmanagementassignedroleids?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые типы перечисления:<br/>[applicationGuardEnabledOptions](/graph/api/resources/intune-deviceconfig-applicationguardenabledoptions?view=graph-rest-beta)<br/>[autoRestartNotificationDismissalMethod](/graph/api/resources/intune-deviceconfig-autorestartnotificationdismissalmethod?view=graph-rest-beta)<br/>[meteredConnectionLimitType](/graph/api/resources/intune-deviceconfig-meteredconnectionlimittype?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлено действие [enableLegacyPcManagement](/graph/api/intune-deviceconfig-devicemanagement-enablelegacypcmanagement?view=graph-rest-beta) для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [extendFeatureUpdatesPause](/graph/api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendfeatureupdatespause?view=graph-rest-beta) для объекта [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [extendQualityUpdatesPause](/graph/api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendqualityupdatespause?view=graph-rest-beta) для объекта [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [unassignUserFromDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice?view=graph-rest-beta) для объекта [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [getAssignedRoleIdsForLoggedInUser](/graph/api/intune-rbac-devicemanagement-getassignedroleidsforloggedinuser?view=graph-rest-beta) для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [getManagedDevicesWithAppFailures](/graph/api/intune-troubleshooting-user-getmanageddeviceswithappfailures?view=graph-rest-beta) для объекта [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [managedDeviceEnrollmentAbandonmentSummary](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentabandonmentsummary?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
|Дополнение|бета|Добавлена функция [managedDeviceEnrollmentAbandonmentDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentabandonmentdetails?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
|Удаление|бета|Удалено свойство **subjectAlternativeNameType** из объекта [androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **subjectAlternativeNameType** для объекта [androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **certificateStore**, **customSubjectAlternativeNames** и **subjectAlternativeNameType** для объекта [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **subjectAlternativeNameType** из объекта [androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **subjectAlternativeNameType** для объекта [androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **certificateStore**, **customSubjectAlternativeNames** и **subjectAlternativeNameType** для объекта [androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **legacyPcManangementEnabled** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **pinRequiredOnLaunchInsteadOfBiometric** из объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **roleScopeTagIds** для объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta).|
|Дополнение|бета|Добавлено свойство **applicationGuardEnabledOptions** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **selectedMobileAppIds** для объекта [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **engagedRestartDeadlineInDays**, **engagedRestartSnoozeScheduleInDays**, **engagedRestartTransitionScheduleInDays**, **autoRestartNotificationDismissal**, **scheduleRestartWarningInHours** и **scheduleImminentRestartWarningInMinutes** для объекта [ windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **preSharedKey** и **meteredConnectionLimit** для объекта [windowsWifiConfiguration](/graph/api/resources/intune-deviceconfig-windowswificonfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **intuneBrandingProfiles** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **v6_0**, **v7_0**, **v7_1**, **v8_0**, **v8_1** и **v9_0** для сложного типа [androidMinimumOperatingSystem](/graph/api/resources/intune-apps-androidminimumoperatingsystem?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **v12_0** для сложного типа [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **runAsLoggedOnUser** из сложного типа [win32LobAppPowerShellScriptDetection](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetection?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **lastUpdateDateTime** для сложного типа [osVersionCount](/graph/api/resources/intune-devices-osversioncount?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **lastUpdateDateTime** для сложного типа [windowsMalwareCategoryCount](/graph/api/resources/intune-devices-windowsmalwarecategorycount?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **lastUpdateDateTime** для сложного типа [windowsMalwareExecutionStateCount](/graph/api/resources/intune-devices-windowsmalwareexecutionstatecount?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **lastUpdateDateTime** для сложного типа [windowsMalwareNameCount](/graph/api/resources/intune-devices-windowsmalwarenamecount?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **lastUpdateDateTime** для сложного типа [windowsMalwareStateCount](/graph/api/resources/intune-devices-windowsmalwarestatecount?view=graph-rest-beta)|

### <a name="privileged-identity-management-apis"></a>API управления привилегированными пользователями

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение | бета | Изменен объект [privilegedapproval](/graph/api/resources/privilegedapproval?view=graph-rest-beta).|
| Дополнение | бета | Добавлен объект [privilegedroleassignmentrequest](/graph/api/resources/privilegedroleassignmentrequest?view=graph-rest-beta), а также следующие методы и действия:<br> [List](/graph/api/privilegedroleassignmentrequest-list?view=graph-rest-beta) <br> [Create](/graph/api/privilegedroleassignmentrequest-post?view=graph-rest-beta) <br> [Cancel](/graph/api/privilegedroleassignmentrequest-cancel?view=graph-rest-beta) <br> [My](/graph/api/privilegedroleassignmentrequest-my?view=graph-rest-beta) |
| Дополнение | бета | Добавлено [Update](/graph/api/privilegedrolesettings-update?view=graph-rest-beta) для [privilegedRoleSettings](/graph/api/resources/privilegedrolesettings?view=graph-rest-beta)|
| Удаление |бета| Удалена [самостоятельная активация назначения ролей](/graph/api/privilegedrole_selfactivate?view=graph-rest-beta)|

### <a name="microsoft-teams-apis"></a>API Microsoft Teams

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение|бета|Добавлена поддержка разрешений приложений для API [архивации объекта команды](/graph/api/team-archive?view=graph-rest-beta) и [распаковки объекта команды](/graph/api/team-unarchive?view=graph-rest-beta).|

### <a name="outlook-contacts"></a>Контакты Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Удаление         | 1.0        | Это исправление в документации: удалено свойство **flag** из статьи по объекту [contact](/graph/api/resources/contact?view=graph-rest-1.0). Свойство никогда не было доступным в объекте **contact**.|

### <a name="reports-apis"></a>API отчетов
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | 1.0    | Добавлено свойство **Site ID** для объекта [getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0). |

## <a name="september-2018"></a>Сентябрь 2018 г.

### <a name="calls-and-online-meetings-api"></a>API звонков и собраний по сети

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | бета        | Ресурс [application](/graph/api/resources/application?view=graph-rest-beta) обновлен для добавления коллекции звонков. |
| Изменение          | бета        | Ресурс [operation](/graph/api/resources/operation?view=graph-rest-beta) обновлен для поддержки API продолжительных звонков и собраний по сети. |
| Дополнение        | бета        | Добавлен ресурс [call](/graph/api/resources/call?view=graph-rest-beta) для управления голосовыми и видеозвонками (изначально в Microsoft Teams), включая API для [создания звонков](/graph/api/application-post-calls?view=graph-rest-beta), [получения звонка](/graph/api/call-get?view=graph-rest-beta), [удаления (завершения) звонка](/graph/api/call-delete?view=graph-rest-beta), [ответа на звонок](/graph/api/call-answer?view=graph-rest-beta), [отклонения звонка](/graph/api/call-reject?view=graph-rest-beta), [перенаправления звонка](/graph/api/call-redirect?view=graph-rest-beta) и [ передачи звонка](/graph/api/call-transfer?view=graph-rest-beta). Мы также расширили API для поддержки [сценариев IVR](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta): [воспроизведение запроса](/graph/api/call-playprompt?view=graph-rest-beta), [запись звонка](/graph/api/call-record?view=graph-rest-beta), [отмена обработки мультимедиа](/graph/api/call-cancelmediaprocessing?view=graph-rest-beta) и [подписка на тональные уведомления](/graph/api/call-subscribetotone?view=graph-rest-beta). |
| Дополнение        | бета        | Добавлен ресурс [participant](/graph/api/resources/call?view=graph-rest-beta) и API для управления участниками в голосовых и видеозвонках и собраниях, в том числе [получение объекта participant](/graph/api/participant-get?view=graph-rest-beta), [настройка звукового микшера для участника](/graph/api/participant-configuremixer?view=graph-rest-beta), отключение звука [одного](/graph/api/participant-mute?view=graph-rest-beta) или [всех](/graph/api/participant-muteall?view=graph-rest-beta) участников, [получение списка участников](/graph/api/call-list-participants?view=graph-rest-beta) в звонке или собрании и [приглашение участников](/graph/api/participant-invite?view=graph-rest-beta) в звонок или собрание. |
| Дополнение        | бета        | Добавлены API для приложений по управлению и участию в звонках и собраниях, включая возможность [делиться контентом](/graph/api/call-changescreensharingrole?view=graph-rest-beta), [самостоятельно отключать и включать звук](/graph/api/call-unmute?view=graph-rest-beta) и [обновлять метаданные, связанные со звонком](/graph/api/call-updatemetadata?view=graph-rest-beta). |
| Дополнение        | бета        | Добавлен ресурс [audio routing group](/graph/api/resources/audioroutinggroup?view=graph-rest-beta) и API для управления частными звуковыми маршрутами между участниками многосторонней беседы, включая [создание групп маршрутизации звука](/graph/api/call-post-audioroutinggroups?view=graph-rest-beta), [получение их списка](/graph/api/audioroutinggroup-get?view=graph-rest-beta), а также их [обновление](/graph/api/audioroutinggroup-update?view=graph-rest-beta) и [удаление](/graph/api/audioroutinggroup-delete?view=graph-rest-beta). |
| Дополнение        | бета        | Добавлен ресурс [online meeting](/graph/api/resources/audioroutinggroup?view=graph-rest-beta) и API для управления собраниями по сети Microsoft Teams. Изначально существует только один API для собраний по сети для [получения объекта online meeting](/graph/api/onlinemeeting-get?view=graph-rest-beta). Также был добавлен соответствующий ресурс для [сведений об аудиоконференции](/graph/api/resources/audioconferencing?view=graph-rest-beta), связанный с собранием (например, URL-адрес телефонного подключения, секретные коды и номера телефонов). |
| Дополнение        | бета        | Выполнение многих из API звонков и собраний занимает длительное время, поэтому были добавлены ресурсы для этих продолжительных операций: [операции, предназначенные для звонков](/graph/api/resources/commsoperation?view=graph-rest-beta), [воспроизведение аудио запросов](/graph/api/resources/playpromptoperation?view=graph-rest-beta) и [ запись](/graph/api/resources/recordoperation?view=graph-rest-beta).  |

### <a name="dynamics-365-business-central-api"></a>API Dynamics 365 Business Central

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | бета          | Добавлены API финансовых показателей для Dynamics 365 Business Central. Дополнительные сведения см. в статье [Справочник по API финансовых показателей](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)

### <a name="microsoft-graph-data-connect"></a>Microsoft Graph Data Connect

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение         | Неприменимо| Представлена возможность массового доступа к данным Office 365. Подробные сведения см. в статье [Microsoft Graph Data Connect (предварительная версия)](data-connect-overview.md).|

### <a name="microsoft-intune-apis"></a>API Microsoft Intune
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлено действие [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-1.0) для объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0). |
|Дополнение|Бета|Добавлены новые объекты:<br/>[officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta)<br/>[officeClientConfigurationAssignment](/graph/api/resources/intune-cirrus-officeclientconfigurationassignment?view=graph-rest-beta)<br/>[officeConfiguration](/graph/api/resources/intune-cirrus-officeconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientSecurityConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientsecurityconfiguration?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[officeClientCheckinStatus](/graph/api/resources/intune-cirrus-officeclientcheckinstatus?view=graph-rest-beta)<br/>[officeConfigurationAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationassignmenttarget?view=graph-rest-beta)<br/>[officeConfigurationGroupAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationgroupassignmenttarget?view=graph-rest-beta)<br/>[officeUserCheckinSummary](/graph/api/resources/intune-cirrus-officeusercheckinsummary?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлено действие [assign](/graph/api/intune-cirrus-officeclientconfiguration-assign?view=graph-rest-beta) для объекта [officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие **updatePrioritie** для коллекции [officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta) |
|Дополнение|Бета|Добавлены новые объекты:<br/>[deviceConfigurationConflictSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationconflictsummary?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta)<br/>[win32LobApp](/graph/api/resources/intune-apps-win32lobapp?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[deviceConfigurationTargetedUserAndDevice](/graph/api/resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice?view=graph-rest-beta)<br/>[win32LobAppDetection](/graph/api/resources/intune-apps-win32lobappdetection?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetection](/graph/api/resources/intune-apps-win32lobappfilesystemdetection?view=graph-rest-beta)<br/>[win32LobAppInstallExperience](/graph/api/resources/intune-apps-win32lobappinstallexperience?view=graph-rest-beta)<br/>[win32LobAppMsiInformation](/graph/api/resources/intune-apps-win32lobappmsiinformation?view=graph-rest-beta)<br/>[win32LobAppPowerShellScriptDetection](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetection?view=graph-rest-beta)<br/>[win32LobAppProductCodeDetection](/graph/api/resources/intune-apps-win32lobappproductcodedetection?view=graph-rest-beta)<br/>[win32LobAppRegistryDetection](/graph/api/resources/intune-apps-win32lobappregistrydetection?view=graph-rest-beta)<br/>[win32LobAppReturnCode](/graph/api/resources/intune-apps-win32lobappreturncode?view=graph-rest-beta)<br/>[windows10AppsForceUpdateSchedule](/graph/api/resources/intune-deviceconfig-windows10appsforceupdateschedule?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые типы перечисления:<br/>[administratorConfiguredDeviceComplianceState](/graph/api/resources/intune-deviceconfig-administratorconfigureddevicecompliancestate?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[microsoftStoreForBusinessPortalSelectionOptions](/graph/api/resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions?view=graph-rest-beta)<br/>[win32LobAppDetectionOperator](/graph/api/resources/intune-apps-win32lobappdetectionoperator?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetectionType](/graph/api/resources/intune-apps-win32lobappfilesystemdetectiontype?view=graph-rest-beta)<br/>[win32LobAppMsiPackageType](/graph/api/resources/intune-apps-win32lobappmsipackagetype?view=graph-rest-beta)<br/>[win32LobAppRegistryDetectionType](/graph/api/resources/intune-apps-win32lobappregistrydetectiontype?view=graph-rest-beta)<br/>[win32LobAppReturnCodeType](/graph/api/resources/intune-apps-win32lobappreturncodetype?view=graph-rest-beta)<br/>[windows10AppsUpdateRecurrence](/graph/api/resources/intune-deviceconfig-windows10appsupdaterecurrence?view=graph-rest-beta)<br/>[windowsAppStartLayoutTileSize](/graph/api/resources/intune-deviceconfig-windowsappstartlayouttilesize?view=graph-rest-beta)<br/>[windowsAutopilotProfileAssignmentDetailedStatus](/graph/api/resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлено действие **overrideComplianceState** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие **getTargetedUsersAndDevices** для коллекции [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) для объекта [importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) |
|Дополнение|бета|Добавлено свойство **restrictedApps** для объекта [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta).|
|Дополнение|бета|Добавлено свойство **tokenCreationDateTime** для объекта [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **restrictedApps** из объекта [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **restrictedApps** из объекта [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta)|
|Изменение|бета|Изменены следующие свойства объекта [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta):<br/>свойство **enablePerApp** преобразовано из обязательного в необязательное<br/>|
|Дополнение|бета|Добавлены свойства **disableProtectionOfManagedOutboundOpenInData** и **protectInboundDataFromUnknownSources** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **microsoftStoreForBusinessPortalSelection** для объекта [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **passcodeMinutesOfInactivityBeforeScreenTimeout** для объекта [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **useOAuth** для объекта [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **kioskModeBlockVolumeButtons**, **classroomForceRequestPermissionToLeaveClasses**, **keychainBlockCloudSync**, ** pkiBlockOTAUpdates**, **privacyForceLimitAdTracking**, **enterpriseBookBlockBackup**, **enterpriseBookBlockMetadataSync**, **airPrintBlocked**, **airPrintBlockCredentialsStorage**, **airPrintForceTrustedTLS**, **airPrintBlockiBeaconDiscovery**, **blockSystemAppRemoval** и **vpnBlockCreation** для объекта [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **disableProtectionOfManagedOutboundOpenInData** и **protectInboundDataFromUnknownSources** для объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **gatekeeperAllowedAppSource** для объекта [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **keychainBlockCloudSync**, **airPrintBlocked**, **airPrintForceTrustedTLS** и **airPrintBlockiBeaconDiscovery** для объекта [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **deviceModel** и **deviceManufacturer** для объекта [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **enabledForScopeValidation** для объекта [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **claimTokenManagementFromExternalMdm** для объекта [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **windows10AppsForceUpdateSchedule** для объекта [windows10AppsForceUpdateSchedule](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **deploymentProfileAssignmentDetailedStatus** для объекта [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства навигации **deviceConfigurationConflictSummary** и **importedWindowsAutopilotDeviceIdentityUploads** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **intendedDeploymentProfile** для объекта [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **startLayoutTileSize** и **name** для сложного типа [windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **desktopApplicationId** и **desktopApplicationLinkPath** для сложного типа [windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **name** из сложного типа [windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **disallowDesktopApps** для сложного типа [windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta)|
|Изменение|бета|Изменены следующие свойства сложного типа [windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta):<br/>свойство **startMenuLayoutXml** преобразовано из обязательного в необязательное<br/>|
|Дополнение|бета|Добавлены свойства **v10_1607**, **v10_1703**, **v10_1709** и **v10_1803** для сложного типа [windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **paloAltoGlobalProtect** для типа перечисления [androidWorkProfileVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconnectiontype?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **remoteLock** для типа перечисления [deviceComplianceActionType](/graph/api/resources/intune-deviceconfig-devicecomplianceactiontype?view=graph-rest-beta)|


### <a name="microsoft-teams-apis"></a>API Microsoft Teams

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение|бета|Добавлены API для [вкладок](/graph/api/resources/teamstab?view=graph-rest-beta).|
|Дополнение|бета|Добавлены API для [публикации приложений для организации](/graph/api/resources/teamsapp?view=graph-rest-beta).|
|Дополнение|бета|Добавлена поддержка разрешений приложений для [GET /teams/{id}](/graph/api/team-get?view=graph-rest-beta) |
|Дополнение|бета|Добавлена поддержка разрешений приложений для [GET /teams/{id}/channels](/graph/api/group-list-channels?view=graph-rest-beta) |
|Дополнение|бета|Добавлена поддержка разрешений приложений для [GET /teams/{id}/channels/{id}](/graph/api/channel-get?view=graph-rest-beta) |
|Дополнение|бета|Добавлена поддержка разрешений приложений для [PUT /groups/{id}/team](/graph/api/team-put-teams?view=graph-rest-beta) |
|Дополнение|бета|Добавлена поддержка разрешений приложений для [PATCH /teams/{id}](/graph/api/team-update?view=graph-rest-beta) |
|Дополнение|бета|Добавлена поддержка разрешений приложений для [создания канала](/graph/api/channel-post?view=graph-rest-beta), [обновления канала](/graph/api/channel-patch?view=graph-rest-beta) и [удаления канала](/graph/api/channel-delete?view=graph-rest-beta). |
|Удаление|бета| Удалены свойства isBlocks и installedState из [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta).|
|Изменение| бета | Свойство context в [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta) переименовано на distributionMethod.|

### <a name="outlook-mail"></a>Почта Outlook

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета | Свойство **InternetMessageHeaders** объекта [message](/graph/api/resources/message?view=graph-rest-1.0) теперь доступно для записи при создании сообщения. |


### <a name="project-rome-notifications-api"></a>API уведомлений Project Rome

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение          | бета        | Добавлен тип ресурса [notification](/graph/api/resources/projectrome-notification?view=graph-rest-beta). |
| Дополнение          | бета        | Добавлены API [создания и публикации уведомлений] (/graph/api/projectrome_notification_post?view=graph-rest-beta).|

### <a name="security-apis"></a>API безопасности

| **Тип изменения** | **Версия** | **Описание**              |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета       | Добавлены API оценки безопасности для [API безопасности](/graph/api/resources/securescore-api-overview?view=graph-rest-beta), включающие следующие ресурсы и операции:<br/>[secureScores](/graph/api/resources/securescores?view=graph-rest-beta) (и соответствующие объекты)<br/>[Перечисление объектов secureScores](/graph/api/securescores-list?view=graph-rest-beta)<br/>[secureScoreControlProfiles](/graph/api/resources/securescorecontrolprofiles?view=graph-rest-beta)<br/>[Перечисление объектов secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-list?view=graph-rest-beta)<br/>[Обновление secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-update?view=graph-rest-beta)


### <a name="onedrive-and-sharepoint-apis"></a>API OneDrive и SharePoint

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлен аргумент **deferCommit** для действия [createUploadSession](/graph/api/driveitem-createuploadsession?view=graph-rest-beta) в объекте [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta)|
| Дополнение        | бета        | Добавлен сложный тип [storagePlanInformation](/graph/api/resources/storageplaninformation?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **storagePlanInformation** для сложного типа [quota](/graph/api/resources/quota?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство навигации **following** для объекта [drive](/graph/api/resources/drive?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено действие [follow](/graph/api/driveitem-follow?view=graph-rest-beta) для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено API [отмены подписки](/graph/api/driveitem-unfollow?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **hasPassword** для объекта [permission](/graph/api/resources/permission?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **preventsDownload** для сложного типа [sharingLink](/graph/api/resources/sharinglink?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство навигации **permission** для объекта [sharedDriveItem](/graph/api/resources/shareddriveitem?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **geolocation** для объекта [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлен сложный тип [geolocationColumn](/graph/api/resources/geolocationcolumn?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **analytics** для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **analytics** для объекта [site](/graph/api/resources/site?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **analytics** для объекта [listItem](/graph/api/resources/listitem?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлена функция **getActivitiesByInterval** для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлена функция **getActivitiesByInterval** для объекта [site](/graph/api/resources/site?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлена функция **getActivitiesByInterval** для объекта [listItem](/graph/api/resources/listitem?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлен объект [itemAnalytics](/graph/api/resources/itemanalytics?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлен объект [itemActivityStat](/graph/api/resources/itemactivity?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлен сложный тип [itemActionStat](/graph/api/resources/itemactionstat?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлен сложный тип [accessAction](/graph/api/resources/accessaction?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлен сложный тип [incompleteData](/graph/api/resources/incompletedata?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **access** для сложного типа [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **location** для сложного типа [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) |
| Дополнение        | 1.0        | Добавлено свойство **preview** для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) |
| Дополнение        | 1.0        | Добавлен сложный тип [itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-1.0) |

## <a name="august-2018"></a>Август 2018 г.

### <a name="delta-query"></a>Запрос изменений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлена возможность [запроса изменений](delta-query-overview.md) для следующих объектов в Azure AD:<br/>[application](/graph/api/application-delta?view=graph-rest-beta)<br/>[directoryRole](/graph/api/directoryrole-delta?view=graph-rest-beta)<br/>[servicePrincipal](/graph/api/serviceprincipal-delta?view=graph-rest-beta) |

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | 1.0 | Добавлено свойство isMultipleDataLocationsForServicesEnabled в ресурс [Organization](/graph/api/resources/organization?view=graph-rest-beta), позволяющее приложениям проверять, включена ли для клиента поддержка нескольких регионов. Добавлено свойство preferredDataLocation в ресурсы [user](/graph/api/resources/user?view=graph-rest-beta) и [group](/graph/api/resources/group?view=graph-rest-beta), позволяющее настраивать предпочтительное расположение данных для пользователя и группы.|
| Дополнение | 1.0 | Добавлено свойство [onPremisesProvisioningErrors](/graph/api/resources/onpremisesprovisioningerror?view=graph-rest-1.0) в объекты [User](/graph/api/resources/user?view=graph-rest-1.0) и [Group](/graph/api/resources/group?view=graph-rest-1.0), представляющее ошибки синхронизации службы каталогов при синхронизации локальных каталогов с Azure Active Directory с использованием продукта синхронизации Майкрософт (включая Azure AD Connect, DirSync и MIM + соединитель).|
| Дополнение | 1.0 | Добавлено свойство [onPremisesExtensionAttributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-1.0) в объект [User](/graph/api/resources/user?view=graph-rest-1.0), содержащее 15 свойств атрибутов настраиваемых расширений. Для пользователя onPremisesSyncEnabled этот набор свойств управляется в локальной службе Active Directory, синхронизирован с Azure AD и доступен только для чтения. Для исключительно облачных пользователей (где значением для onPremisesSyncEnabled является false) эти свойства можно задать при создании или обновлении.|
|Дополнение|1.0|Добавлены свойства **onPremisesDomainName**, **onPremisesSamAccountName** и **onPremisesUserPrincipalName** для объекта [User](/graph/api/resources/user?view=graph-rest-1.0)|

### <a name="microsoft-intune-apis"></a>API Microsoft Intune

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлены новые объекты:<br/>[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-1.0)<br/>[androidWorkProfileCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilecustomconfiguration?view=graph-rest-1.0)<br/>[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-1.0)<br/>|
|Дополнение|1.0|Добавлены новые типы перечисления:<br/>[androidWorkProfileCrossProfileDataSharingType](/graph/api/resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype?view=graph-rest-1.0)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](/graph/api/resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype?view=graph-rest-1.0)<br/>[androidWorkProfileRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype?view=graph-rest-1.0)<br/>|
|Дополнение|1.0|Добавлена функция [managedDeviceEnrollmentFailureDetails](/graph/api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-1.0) для ресурса [reportRoot](/graph/api/resources/intune-shared-reportroot?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлена функция [managedDeviceEnrollmentTopFailures](/graph/api/intune-shared-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-1.0) для ресурса [reportRoot](/graph/api/resources/intune-shared-reportroot?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлено свойство **kioskModeBuiltInAppId** для объекта [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-1.0).|
|Дополнение|1.0|Добавлен элемент **notAssigned** для типа перечисления [complianceStatus](/graph/api/resources/intune-shared-compliancestatus?view=graph-rest-1.0)|
|Дополнение|1.0|Добавлен элемент **pushNotification** для типа перечисления [deviceComplianceActionType](/graph/api/resources/intune-deviceconfig-devicecomplianceactiontype?view=graph-rest-1.0)|
|Дополнение|1.0|Добавлен элемент **userAbandonment** для типа перечисления [deviceEnrollmentFailureReason](/graph/api/resources/intune-troubleshooting-deviceenrollmentfailurereason?view=graph-rest-1.0)|
|Дополнение|1.0|Добавлены элементы **compromised** и **misconfigured** для типа перечисления [managedDevicePartnerReportedHealthState](/graph/api/resources/intune-devices-manageddevicepartnerreportedhealthstate?view=graph-rest-1.0)|
|Дополнение|1.0|Добавлен элемент **assignedToExternalMDM** для типа перечисления [vppTokenState](/graph/api/resources/intune-onboarding-vpptokenstate?view=graph-rest-1.0)|
||
|Дополнение|Бета|Добавлены новые объекты:<br/>[advancedThreatProtectionOnboardingDeviceSettingState](/graph/api/resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate?view=graph-rest-beta)<br/>[advancedThreatProtectionOnboardingStateSummary](/graph/api/resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary?view=graph-rest-beta)<br/>[depEnrollmentBaseProfile](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile?view=graph-rest-beta)<br/>[depEnrollmentProfile](/graph/api/resources/intune-enrollment-depenrollmentprofile?view=graph-rest-beta)<br/>[depIOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depiosenrollmentprofile?view=graph-rest-beta)<br/>[depMacOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depmacosenrollmentprofile?view=graph-rest-beta)<br/>[enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta)<br/>[importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta)<br/>[importedAppleDeviceIdentityResult](/graph/api/resources/intune-enrollment-importedappledeviceidentityresult?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta)<br/>[roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta)<br/>[windowsIdentityProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsidentityprotectionconfiguration?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[configurationManagerClientHealthState](/graph/api/resources/intune-devices-configurationmanagerclienthealthstate?view=graph-rest-beta)<br/>[customSubjectAlternativeName](/graph/api/resources/intune-deviceconfig-customsubjectalternativename?view=graph-rest-beta)<br/>[deviceManagementUserRightsLocalUserOrGroup](/graph/api/resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup?view=graph-rest-beta)<br/>[deviceManagementUserRightsSetting](/graph/api/resources/intune-deviceconfig-devicemanagementuserrightssetting?view=graph-rest-beta)<br/>[managementCertificateWithThumbprint](/graph/api/resources/intune-enrollment-managementcertificatewiththumbprint?view=graph-rest-beta)<br/>[mobileAppSupportedDeviceType](/graph/api/resources/intune-troubleshooting-mobileappsupporteddevicetype?view=graph-rest-beta)<br/>[osVersionCount](/graph/api/resources/intune-devices-osversioncount?view=graph-rest-beta)<br/>[windowsMalwareCategoryCount](/graph/api/resources/intune-devices-windowsmalwarecategorycount?view=graph-rest-beta)<br/>[windowsMalwareExecutionStateCount](/graph/api/resources/intune-devices-windowsmalwareexecutionstatecount?view=graph-rest-beta)<br/>[windowsMalwareNameCount](/graph/api/resources/intune-devices-windowsmalwarenamecount?view=graph-rest-beta)<br/>[windowsMalwareOverview](/graph/api/resources/intune-devices-windowsmalwareoverview?view=graph-rest-beta)<br/>[windowsMalwareStateCount](/graph/api/resources/intune-devices-windowsmalwarestatecount?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые типы перечисления:<br/>[configurationManagerClientState](/graph/api/resources/intune-devices-configurationmanagerclientstate?view=graph-rest-beta)<br/>[depTokenType](/graph/api/resources/intune-enrollment-deptokentype?view=graph-rest-beta)<br/>[discoverySource](/graph/api/resources/intune-enrollment-discoverysource?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[iTunesPairingMode](/graph/api/resources/intune-enrollment-itunespairingmode?view=graph-rest-beta)<br/>[lanManagerAuthenticationLevel](/graph/api/resources/intune-deviceconfig-lanmanagerauthenticationlevel?view=graph-rest-beta)<br/>[localSecurityOptionsMinimumSessionSecurity](/graph/api/resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity?view=graph-rest-beta)<br/>[resultantAppStateDetail](/graph/api/resources/intune-apps-resultantappstatedetail?view=graph-rest-beta)<br/>[vpnProviderType](/graph/api/resources/intune-deviceconfig-vpnprovidertype?view=graph-rest-beta)<br/>[windowsMalwareThreatState](/graph/api/resources/intune-devices-windowsmalwarethreatstate?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлено действие [uploadDepToken](/graph/api/intune-enrollment-deponboardingsetting-uploaddeptoken?view=graph-rest-beta) для [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [syncWithAppleDeviceEnrollmentProgram](/graph/api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram?view=graph-rest-beta) для [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [setDefaultProfile](/graph/api/intune-enrollment-enrollmentprofile-setdefaultprofile?view=graph-rest-beta) для объекта [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие **importAppleDeviceIdentityList** для коллекции [importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [updateDeviceProfileAssignment](/graph/api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta) для объекта [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta). |
|Дополнение|бета|Добавлено действие [shareForSchoolDataSyncService](/graph/api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice?view=graph-rest-beta) для объекта [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [unshareForSchoolDataSyncService](/graph/api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice?view=graph-rest-beta) для объекта [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [assignUserToDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice?view=graph-rest-beta) для объекта [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [getRoleScopeTagsByResource](/graph/api/intune-rbac-devicemanagement-getrolescopetagsbyresource?view=graph-rest-beta) для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [getRoleScopeTagsByIds](/graph/api/intune-rbac-devicemanagement-getrolescopetagsbyids?view=graph-rest-beta) для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [getEncryptionPublicKey](/graph/api/intune-enrollment-deponboardingsetting-getencryptionpublickey?view=graph-rest-beta) для [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [exportMobileConfig](/graph/api/intune-enrollment-enrollmentprofile-exportmobileconfig?view=graph-rest-beta) для объекта [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) для объекта [importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) |
|Удаление|бета|Удалена коллекция **uploadDepToken** |
|Удаление|бета|Удалено действие **syncWithAppleDeviceEnrollmentProgram** из коллекции [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Удаление|бета|Удалена функция **getEncryptionPublicKey** из коллекции [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Дополнение|бета|Добавлено свойство **restrictedApps** для объекта [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **vpnAlwaysOnPackageIdentifier** и **vpnEnableAlwaysOnLockdownMode** для объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **packageName** из объекта [androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **restrictedApps** в объект [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **vpnAlwaysOnPackageIdentifier** и **vpnEnableAlwaysOnLockdownMode** для объекта [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **optInToDeviceIdSharing** для объекта [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **tokenType**, **tokenName**, **syncedDeviceCount**, **defaultProfileDisplayName** и ** dataSharingConsentGranted** для объекта [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **roleScopeTagIds** для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **roleScopeTagIds** и **supportsScopeTags** для объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **windowsMalwareOverview** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Изменение|бета|Изменены следующие свойства объекта [iosCertificateProfileBase](/graph/api/resources/intune-deviceconfig-ioscertificateprofilebase?view=graph-rest-beta):<br/>свойство **subjectAlternativeNameType** преобразовано из обязательного в необязательное<br/>|
|Дополнение|бета|Добавлено свойство **restrictedApps** для объекта [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **certificateStore** и **customSubjectAlternativeNames** для объекта [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **enforcedSoftwareUpdateDelayInDays** для объекта [iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **providerType**, **userDomain**, **strictEnforcement**, **cloudName** и **excludeList** для объекта [iosVpnConfiguration](/graph/api/resources/intune-deviceconfig-iosvpnconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **safariBlockAutofill**, **cameraBlocked**, **iTunesBlockMusicService**, **spotlightBlockInternetResults**, **keyboardBlockDictation**, **definitionLookupBlocked**, **appleWatchBlockAutoUnlock**, **iTunesBlockFileSharing**, **iCloudBlockDocumentSync**, **iCloudBlockMail**, **iCloudBlockAddressBook**, **iCloudBlockCalendar**, **iCloudBlockReminders**, **iCloudBlockBookmarks**, **iCloudBlockNotes**, **airDropBlocked**, **passwordBlockModification** и **passwordBlockFingerprintUnlock** для объекта [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **roleScopeTagIds**, **windowsActiveMalwareCount**, **windowsRemediatedMalwareCount**, **notes** и **configurationManagerClientHealthState** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **installStateDetail** для объекта [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **roleScopeTagIds** для объекта [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **targetVersion** и **updateVersion** для объекта [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **resource** для объекта [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **localStorage**, **setPowerPolicies** и **signInOnResume** для объекта [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **configurationManagerComplianceRequired** для объекта [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **userRightsAccessCredentialManagerAsTrustedCaller**, **userRightsAllowAccessFromNetwork**, **userRightsBlockAccessFromNetwork**, **userRightsActAsPartOfTheOperatingSystem**, **userRightsLocalLogOn**, **userRightsBackupData**, **userRightsChangeSystemTime**, **userRightsCreateGlobalObjects**, **userRightsCreatePageFile**, **userRightsCreatePermanentSharedObjects**, **userRightsCreateSymbolicLinks**, **userRightsCreateToken**, **userRightsDebugPrograms**, **userRightsRemoteDesktopServicesLogOn**, **userRightsDelegation**, **userRightsGenerateSecurityAudits**, **userRightsImpersonateClient**, **userRightsIncreaseSchedulingPriority**, **userRightsLoadUnloadDrivers**, **userRightsLockMemory**, **userRightsManageAuditingAndSecurityLogs**, **userRightsManageVolumes**, **userRightsModifyFirmwareEnvironment**, **userRightsModifyObjectLabels**, **userRightsProfileSingleProcess**, **userRightsRemoteShutdown**, **userRightsRestoreData**, **userRightsTakeOwnership**, **userRightsRegisterProcessAsService**, **localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients**, **localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers**, **lanManagerAuthenticationLevel** и **lanManagerWorkstationEnableInsecureGuestLogons** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **passwordMinimumAgeInDays**, **tenantLockdownRequireNetworkDuringOutOfBoxExperience** и **dataProtectionBlockDirectMemoryAccess** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **extendedKeyUsages** для объекта [windows10PkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pkcscertificateprofile?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **enableDnsRegistration** и **dnsSuffixes** для объекта [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **customSubjectAlternativeNames** для объекта [windows81CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows81certificateprofilebase?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **extractHardwareHash** и **deviceNameTemplate** для объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **addressableUserName** и **userPrincipalName** для объекта [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **threatState** для объекта [windowsDeviceMalwareState](/graph/api/resources/intune-devices-windowsdevicemalwarestate?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **qualityUpdatesPauseStartDateTime**, **featureUpdatesPauseStartDateTime**, **featureUpdatesRollbackWindowInDays**, **qualityUpdatesWillBeRolledBack**, **featureUpdatesWillBeRolledBack**, **qualityUpdatesRollbackStartDateTime** и **featureUpdatesRollbackStartDateTime** для объекта [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **trustedServerCertificateNames** для объекта [windowsWifiEnterpriseEAPConfiguration](/graph/api/resources/intune-deviceconfig-windowswifienterpriseeapconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства навигации **defaultIosEnrollmentProfile**, **defaultMacOsEnrollmentProfile**, **enrollmentProfiles** и **importedAppleDeviceIdentities** для объекта [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **roleScopeTags** для объекта [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta).|
|Дополнение|бета|Добавлены свойства навигации **advancedThreatProtectionOnboardingStateSummary**, **roleScopeTags** и **importedWindowsAutopilotDeviceIdentityUploads** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **supportedDeviceTypes** для сложного типа [mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **hideEscapeLink** для сложного типа [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)|
|Дополнение|бета|Добавлены элементы **zscalerPrivateAccess**, **f5Access2018**, **citrixSso** и **paloAltoGlobalProtectV2** для типа перечисления [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **userAbandonment** для типа перечисления [deviceEnrollmentFailureReason](/graph/api/resources/intune-troubleshooting-deviceenrollmentfailurereason?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **blocked** для типа перечисления [enrollmentState](/graph/api/resources/intune-enrollment-enrollmentstate?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **microsoft365ManagedMdm** для типа перечисления [managementAgentType](/graph/api/resources/intune-devices-managementagenttype?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **domainNameService** для типа перечисления [subjectAlternativeNameType](/graph/api/resources/intune-deviceconfig-subjectalternativenametype?view=graph-rest-beta)|
|Дополнение|бета|Добавлены элементы **wpa2Personal** и **wpa2Enterprise** для типа перечисления [wiFiSecurityType](/graph/api/resources/intune-deviceconfig-wifisecuritytype?view=graph-rest-beta)|
|Дополнение|бета|Добавлены элементы **enterpriseUnwantedSoftware**, **ransom** и **hipsRule** для типа перечисления [windowsMalwareCategory](/graph/api/resources/intune-devices-windowsmalwarecategory?view=graph-rest-beta)|

### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлено действие [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) и сложные типы [freeBusyError](/graph/api/resources/freebusyerror?view=graph-rest-beta), [scheduleInformation](/graph/api/resources/scheduleinformation?view=graph-rest-beta) и [scheduleItem](/graph/api/resources/scheduleitem?view=graph-rest-beta) для поддержки [получения сведений о доступности пользователей, списков рассылки и ресурсов для указанного периода времени](outlook-get-free-busy-schedule.md). |

### <a name="outlook-mail"></a>Почта Outlook

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлена поддержка действия [getMailTips](/graph/api/user-getmailtips?view=graph-rest-1.0) для получения подсказок для определенных получателей. Добавлены следующие ресурсы: [automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-1.0), [mailTips](/graph/api/resources/mailtips?view=graph-rest-1.0), [mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-1.0). |

### <a name="reports-apis"></a>API отчетов
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | 1.0    | Добавлено свойство **Activated On Shared Computer** для объекта [getoffice365activationsuserdetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0) |
| Дополнение    | 1.0    | Добавлено свойство **Shared Computer Activation** для объекта [getoffice365activationsusercounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0). |

### <a name="security-apis"></a>API безопасности

| **Тип изменения** | **Версия** | **Описание**              |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета       | Добавлены свойства **activityGroupName**, **cloudAppStates**, **confidence** и **registryKeyStates** для объекта [alert](/graph/api/resources/alert?view=graph-rest-beta ). |
|Удаление|бета| Удалены свойства **activityGroupStates**, **applicationStates**, **malwareWasRunning**, **riskScore** и **type** из объекта [alert](/graph/api/resources/alert?view=graph-rest-beta ). |
|Изменение|бета| Тип **comments** изменен с `String` на `String collection`, а тип **severity** изменен с `String` на перечисление [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta) в объекте [alert](/graph/api/resources/alert?view=graph-rest-beta). |
| Дополнение        | бета       | Добавлены следующие типы ресурсов: <br/> [cloudAppSecurityState](/graph/api/resources/cloudappsecuritystate?view=graph-rest-beta) <br/> [fileHash](/graph/api/resources/filehash?view=graph-rest-beta) <br/> [registryKeyState](/graph/api/resources/registrykeystate?view=graph-rest-beta) |
|Удаление|бета| Удалены следующие типы ресурсов: <br/> **activityGroupState**  <br/> **applicationSecurityState** |
| Дополнение        | бета       | Добавлены следующие перечисления: <br/> [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta) <br/> [connectionDirection](/graph/api/resources/connectiondirectionenumtype?view=graph-rest-beta) <br/> [connectionStatus](/graph/api/resources/connectionstatusenumtype?view=graph-rest-beta) <br/> [emailRole](/graph/api/resources/emailroleenumtype?view=graph-rest-beta) <br/> [fileHashType](/graph/api/resources/filehashtypeenumtype?view=graph-rest-beta) <br/> [registryHive](/graph/api/resources/registryhiveenumtype?view=graph-rest-beta)  <br/> [registryOperation](/graph/api/resources/registryoperationenumtype?view=graph-rest-beta) <br/> [registryValueType](/graph/api/resources/registryvaluetypeenumtype?view=graph-rest-beta)|
|Удаление|Бета| Удалены следующие типы перечисления: <br/> **alertType** <br/> **applicationPermissionsRequired** |
| Дополнение        | бета       | Добавлено свойство **fileHash** для объекта [fileSecurityState](/graph/api/resources/filesecuritystate?view=graph-rest-beta ).|
|Удаление|бета| Удалены свойства **authenticodeHash256** и **sha256** из объекта [fileSecurityState](/graph/api/resources/filesecuritystate?view=graph-rest-beta). |
| Дополнение | бета | Добавлено свойство **os** для объекта [hostSecurityState](/graph/api/resources/hostsecuritystate?view=graph-rest-beta).|
| Дополнение | бета | Добавлены свойства **category**, **family** и **wasRunning** для объекта [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta).|
|Удаление|бета| Удалено свойство **aliases** из объекта [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta). |
|Изменение|бета| Свойство **malwareWasRunning** перемещено из объекта [alert](/graph/api/resources/alert?view=graph-rest-beta ) в [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta) и переименовано в **wasRunning**. |
| Дополнение        | бета       | Добавлены свойства **applicationName**, **destinationDomain**, **direction**, **domainRegisteredDateTime**, **localDnsName **, **natDestinationAddress**, **natDestinationPort**, **natSourceAddress**, **natSourcePort**, **riskScore**, **status** и **urlParameters** для объекта [networkConnection](/graph/api/resources/networkconnection?view=graph-rest-beta ).|
|Изменение|бета| Свойство **uri** изменено на **destinationUrl** в объекте [networkConnection](/graph/api/resources/networkconnection?view=graph-rest-beta ). |
| Дополнение        | бета       | Добавлено свойство **fileHash** для объекта [process](/graph/api/resources/process?view=graph-rest-beta ).|
|Удаление|бета| Удалены свойства **authenticodeHash256** и **sha256** из объекта [process](/graph/api/resources/process?view=graph-rest-beta ). |
| Дополнение        | бета       | Добавлены свойства **aadUserId**, **emailRole**, **isVpn** и **logonIp** для объекта [userSecurityState](/graph/api/resources/usersecuritystate?view=graph-rest-beta).|
|Изменение|бета| Свойство **logonIpAddress** изменено на **logonIp** в объекте [userSecurityState](/graph/api/resources/usersecuritystate?view=graph-rest-beta). |
| Дополнение        | бета       | Добавлено свойство **wasRunning** для объекта [vulnerabilityState](/graph/api/resources/vulnerabilitystate?view=graph-rest-beta).|
|Удаление|бета| Удалено свойство **name** из объекта [vulnerabilityState](/graph/api/resources/vulnerabilitystate?view=graph-rest-beta). |

## <a name="july-2018"></a>Июль 2018 г.

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Изменение|бета|Обновлен ресурс [chatmessage](/graph/api/resources/chatmessage?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлен тип ресурса [вложения для чата](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлен тип ресурса [упоминания для чата](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлен тип ресурса [реакции для чата](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлена возможность [получения всех API сообщений в канале](/graph/api/channel-list-messages?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения API сообщений в канале](/graph/api/channel-get-message?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения всех API ответов на сообщения](/graph/api/channel-list-messagereplies?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения ответа для API сообщений](/graph/api/channel-get-messagereply?view=graph-rest-beta) |

### <a name="synchronization-apis"></a>API синхронизации

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлено свойство **progress** для объекта [sychronizationStatus](/graph/api/resources/synchronization-synchronizationstatus?view=graph-rest-beta), чтобы разрешить клиентам наблюдать за ходом выполнения задания синхронизации.|

### <a name="application-and-serviceprincipal-api-changes"></a>Изменения в API application и servicePrincipal

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | API [application](/graph/api/resources/application?view=graph-rest-beta) и [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) будут обновлены в предварительной (бета) версии. Первый набор изменений будет применен 16 мая 2018 г. Изменения включают в себя переименование и реструктуризацию свойств. Большинство существующих свойств будут доступны только после применения изменений. Будут добавлены новые свойства. Прежде чем выйдет версия 1.0 с изменениями, будет выпущена бета-версия. |

### <a name="microsoft-teams-apis"></a>API Microsoft Teams
| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение|Бета-версия|Добавлена поддержка разрешений приложений для [/users/{id}/joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения всех API сообщений в канале](/graph/api/channel-list-messages?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения API сообщений в канале](/graph/api/channel-get-message?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения всех API ответов на сообщения](/graph/api/channel-list-messagereplies?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения ответа для API сообщений](/graph/api/channel-get-messagereply?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлен тип ресурса [вложения для чата](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлен тип ресурса [упоминания для чата](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлен тип ресурса [реакции для чата](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Изменение|Бета-версия|Обновлен ресурс [chatmessage](/graph/api/resources/chatmessage?view=graph-rest-beta)|
|Удаление|Бета-версия|Удален DELETE /groups/{id}/team/channels/{id}, используйте DELETE /teams/{id}/channels/{id}. |
|Удаление|Бета-версия|Удален GET /groups/{id}/team/channels/{id}, используйте GET /teams/{id}/channels/{id}. |
|Удаление|Бета-версия|Удален PATCH /groups/{id}/team/channels/{id}, используйте PATCH /teams/{id}/channels/{id}. |
|Удаление|Бета-версия|Удален POST /groups/{id}/team/channels/{id}/chatthreads, используйте POST /teams/{id}/channels/{id}/chatthreads. |
|Удаление|Бета-версия|Удален GET /groups/{id}/team/channels, используйте GET /teams/{id}/channels. |
|Удаление|Бета-версия|Удален DELETE /groups/{id}/channels/{id}, используйте DELETE /teams/{id}/channels/{id}. |
|Удаление|Бета|Удален GET /groups/{id}/channels/{id}, используйте GET /teams/{id}/channels/{id}. |
|Удаление|Бета-версия|Удален PATCH /groups/{id}/channels/{id}, используйте PATCH /teams/{id}/channels/{id}. |
|Удаление|Бета-версия|Удален POST /groups/{id}/channels/{id}/chatthreads, используйте POST /teams/{id}/channels/{id}/chatthreads. |
|Удаление|Бета-версия|Удален GET /groups/{id}/channels, используйте GET /teams/{id}/channels. |
|Удаление|Бета-версия|Удален POST /groups/{id}/team/channels, используйте POST /teams/{id}/channels. |
|Удаление|Бета-версия|Удален GET /groups/{id}/team, используйте GET /teams/{id}. |
|Удаление|Бета-версия|Удален PATCH /groups/{id}/team, используйте PATCH /teams/{id}. |
|Дополнение|Бета-версия|Добавлен API для [перечисления всех групп в организации](teams-list-all-teams.md). |

### <a name="outlook-contacts"></a>Контакты Outlook
| **Тип изменения** | **Версия**   | **Описание**                          |
|:--------------- |:------------- |:---------------------------------------- |
|Дополнение |Бета-версия | Добавлен сложный тип [typedEmailAddress](/graph/api/resources/typedemailaddress?view=graph-rest-beta). |
|Изменение | Бета-версия | Изменен тип свойства **emailAddresses** для ресурса [contact](/graph/api/resources/contact?view=graph-rest-beta). Теперь это коллекция экземпляров **typedEmailAddress**.|

### <a name="webhooks"></a>Веб-перехватчики
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Критическое изменение | Бета-версия и версия 1.0 | Сокращен до 3 дней [максимальный период действия подписки](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type) с использованием [веб-перехватчиков](/graph/api/resources/webhooks?view=graph-rest-1.0) для элементов в корне диска. |


## <a name="june-2018"></a>Июнь 2018 г.

### <a name="identity-and-access-apis"></a>API удостоверений и доступа

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлена функция [получения доступа к проверкам](/graph/api/resources/accessreviews-root?view=graph-rest-beta) в [Azure AD](/graph/api/resources/azure-ad-overview?view=graph-rest-beta). |

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Все | Новые разрешения приложений _Application.ReadWrite.All_ и _Application.ReadWrite.OwnedBy_, позволяющие клиентскому приложению создавать, читать, обновлять и удалять приложения и субъекты-службы, как описано в [статье о разрешениях](permissions-reference.md#application-resource-permissions). |
| Дополнение | 1.0 | Добавлены свойства **ageGroup**, **legalAgeGroupClassification** и **ConsentRequiredForMinor** для ресурса [user](/graph/api/resources/user?view=graph-rest-1.0)

### <a name="microsoft-intune-apis"></a>API Microsoft Intune

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Для сущности [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0) добавлено свойство **connectorServerName**.|
|Дополнение|1.0|Для сущности [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0) добавлены свойства **firewallEnabled**, **firewallBlockAllIncoming** и **firewallEnableStealthMode**.|
|Дополнение|1.0|Для типа перечисления [iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-1.0) добавлен элемент **unknown**.|
|Дополнение|Бета|Добавлены новые сущности:<br/>[androidDeviceOwnerWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownerwificonfiguration?view=graph-rest-beta)<br/>[iosVppAppAssignedDeviceLicense](/graph/api/resources/intune-apps-iosvppappassigneddevicelicense?view=graph-rest-beta)<br/>[iosVppAppAssignedLicense](/graph/api/resources/intune-apps-iosvppappassignedlicense?view=graph-rest-beta)<br/>[iosVppAppAssignedUserLicense](/graph/api/resources/intune-apps-iosvppappassigneduserlicense?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationState](/graph/api/resources/intune-deviceconfig-manageddevicemobileappconfigurationstate?view=graph-rest-beta)<br/>[userPFXCertificate](/graph/api/resources/intune-raimportcerts-userpfxcertificate?view=graph-rest-beta)<br/>[vppTokenLicenseSummary](/graph/api/resources/intune-onboarding-vpptokenlicensesummary?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[iosVppAppRevokeLicensesActionResult](/graph/api/resources/intune-apps-iosvppapprevokelicensesactionresult?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые типы перечисления:<br/>[androidDeviceOwnerSystemUpdateInstallType](/graph/api/resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype?view=graph-rest-beta)<br/>[androidDeviceOwnerWiFiSecurityType](/graph/api/resources/intune-deviceconfig-androiddeviceownerwifisecuritytype?view=graph-rest-beta)<br/>[userPfxIntendedPurpose](/graph/api/resources/intune-raimportcerts-userpfxintendedpurpose?view=graph-rest-beta)<br/>[userPfxPaddingScheme](/graph/api/resources/intune-raimportcerts-userpfxpaddingscheme?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Для ресурса [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) добавлено действие [completeSignup](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken?view=graph-rest-beta). |
|Дополнение|Бета|Для ресурса [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) добавлено действие [revokeAllLicenses](/graph/api/intune-apps-iosvppapp-revokealllicenses?view=graph-rest-beta) |
|Дополнение|Бета|Для ресурса [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) добавлено действие [revokeUserLicense](/graph/api/intune-apps-iosvppapp-revokeuserlicense?view=graph-rest-beta) |
|Дополнение|Бета|Для ресурса [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) добавлено действие [revokeDeviceLicense](/graph/api/intune-apps-iosvppapp-revokedevicelicense?view=graph-rest-beta) |
|Дополнение|Бета|Для ресурса [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) добавлено действие [sendCustomNotificationToCompanyPortal](/graph/api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal?view=graph-rest-beta) |
|Дополнение|Бета|Для семейства [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) добавлена функция **getLicensesForApp** |
|Удаление|Бета|Удалены следующие типы перечисления:<br/>**windowsUpdateInsiderBuildControl**<br/>|
|Дополнение|Бета|Для сущности [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta) добавлены свойства **systemUpdateWindowStartMinutesAfterMidnight**, **systemUpdateWindowEndMinutesAfterMidnight** и **systemUpdateInstallType**|
|Изменение|Бета|Изменен тип следующих свойств сущности [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta):<br/>**passwordMinutesOfInactivityBeforeScreenTimeout** из Int64 для Int32<br/>|
|Дополнение|Бета|Для сущности [androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta) добавлено свойство **customKeyValueData**|
|Дополнение|Бета|Для сущности [androidVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidvpnconfiguration?view=graph-rest-beta) добавлено свойство **customKeyValueData**|
|Дополнение|Бета|Для сущности [androidWorkProfileVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconfiguration?view=graph-rest-beta) добавлено свойство **customKeyValueData**|
|Дополнение|Бета|Для сущности [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta) добавлено свойство **customKeyValueData**|
|Дополнение|Бета|Для сущности [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-beta) добавлены свойства **userPrincipalName** и **deviceModel**|
|Дополнение|Бета|Для сущности [deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-beta) добавлены свойства **userId** и **userPrincipalName**|
|Дополнение|Бета|Для сущности [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta) добавлено свойство **connectorServerName**|
|Удаление|Бета|Для сущности [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) удалено свойство **settingXml**|
|Дополнение|Бета|Для сущности [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) добавлены свойства **vppTokenId** и **revokeLicenseActionResults**|
|Дополнение|Бета|Для сущности [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) добавлены свойства **firewallEnabled**, **firewallBlockAllIncoming** и **firewallEnableStealthMode**|
|Удаление|Бета|Для сущности [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) удалено свойство **remoteAssistanceSessionErrorString**|
|Дополнение|Бета|Для сущности [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta) добавлены свойства **antivirusRequired** и **antiSpywareRequired**|
|Дополнение|Бета|Для сущности [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) добавлены свойства **defenderOfficeAppsOtherProcessInjection**, **defenderOfficeAppsExecutableContentCreationOrLaunch**, **defenderOfficeAppsLaunchChildProcess**, **defenderOfficeMacroCodeAllowWin32Imports**, **defenderScriptObfuscatedMacroCode**, **defenderScriptDownloadedPayloadExecution**, **defenderProcessCreation**, **defenderUntrustedUSBProcess**, **defenderUntrustedExecutable** и **defenderEmailContentExecution **|
|Дополнение|Бета|Для сущности [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) добавлены свойства **searchDisableLocation**, **inkWorkspaceAccessState**, **defenderPotentiallyUnwantedAppActionSetting** и ** defenderCloudExtendedTimeoutInSeconds** |
|Дополнение|Бета|Для сущности [windows81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows81generalconfiguration?view=graph-rest-beta) добавлены свойства **updatesMinimumAutoInstallClassification**|
|Удаление|Бета|Для сущности [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) добавлено свойство **previewBuildSetting**|
|Дополнение|Бета|Для сущности [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) добавлено свойство **userPfxCertificates**|
|Дополнение|Бета|Для сущности [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) добавлено свойство навигации **assignedLicenses**|
|Дополнение|Бета|Для сущности [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) добавлено свойство навигации **managedDeviceMobileAppConfigurationStates**|
|Дополнение|Бета|Для сложного типа [iosWebContentFilterSpecificWebsitesAccess](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterspecificwebsitesaccess?view=graph-rest-beta) добавлено свойство **websiteList**|
|Дополнение|Бета|Для типа перечисления [devicePlatformType](/graph/api/resources/intune-deviceconfig-deviceplatformtype?view=graph-rest-beta) добавлен участник **androidWorkProfile**|
|Дополнение|Бета|Для типа перечисления [editionUpgradeLicenseType](/graph/api/resources/intune-deviceconfig-editionupgradelicensetype?view=graph-rest-beta) добавлен участник **notConfigured**|
|Дополнение|Бета|Для типа перечисления [iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-beta) добавлен участник **unknown**|
|Дополнение|Бета|Для типа перечисления [mobileAppActionType](/graph/api/resources/intune-troubleshooting-mobileappactiontype?view=graph-rest-beta) добавлен участник **userRequestedInstall**|
|Дополнение|Бета|Для типа перечисления [windows10EditionType](/graph/api/resources/intune-deviceconfig-windows10editiontype?view=graph-rest-beta) добавлен участник **notConfigured**

### <a name="microsoft-teams-apis"></a>API Microsoft Teams
| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение         | Бета          | Добавлены API [архивирования](/graph/api/team-archive?view=graph-rest-beta) и [разархивирования](/graph/api/team-unarchive?view=graph-rest-beta) команды.|
|Дополнение         | Бета          | Добавлена операция [клонирования](/graph/api/team-clone?view=graph-rest-beta) команды. |
|Дополнение         | Бета          | Добавлены интерфейсы API для добавления [приложений](/graph/api/resources/teamsapp?view=graph-rest-beta) в группы и удаления из них. |
|Изменение|Бета|Обновлен путь к сущности [команды](/graph/api/resources/team?view=graph-rest-beta).|
|Изменение|Бета|Обновлен путь к сущности [канала](/graph/api/resources/channel?view=graph-rest-beta).|


### <a name="privileged-identity-management-apis"></a>API управления привилегированными пользователями

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета | Добавлена сущность [privilegedAccess](/graph/api/resources/privilegedaccess?view=graph-rest-beta).|
| Дополнение | Бета | Добавлен объект [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta), а также следующие методы и действия: <br> [Список](/graph/api/governanceresource-list?view=graph-rest-beta) <br> [Получение](/graph/api/governanceresource-get?view=graph-rest-beta)<br>|
| Дополнение | Бета | Добавлена сущность [governanceSubject](/graph/api/resources/governancesubject?view=graph-rest-beta).|
| Дополнение | Бета | Добавлена сущность [governanceRoleDefinition](/graph/api/resources/governanceroledefinition?view=graph-rest-beta), а также следующие методы и действия:<br> [Список](/graph/api/governanceroledefinition-list?view=graph-rest-beta) <br> [Получение](/graph/api/governanceroledefinition-get?view=graph-rest-beta) |
| Дополнение | Бета | Добавлена сущность [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta), а также следующие методы и действия:<br> [Список](/graph/api/governanceroleassignment-list?view=graph-rest-beta) <br> [Получение](/graph/api/governanceroleassignment-get?view=graph-rest-beta) <br> [Экспорт](/graph/api/governanceroleassignment-export?view=graph-rest-beta) |
| Дополнение | Бета | Добавлена сущность [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta), а также следующие методы и действия:<br> [Список](/graph/api/governanceroleassignmentrequest-list?view=graph-rest-beta) <br> [Получение](/graph/api/governanceroleassignmentrequest-get?view=graph-rest-beta) <br> [Создание](/graph/api/governanceroleassignmentrequest-post?view=graph-rest-beta) <br> [Отмена](/graph/api/governanceroleassignmentrequest-cancel?view=graph-rest-beta) <br> [Обновление](/graph/api/governanceroleassignmentrequest-update?view=graph-rest-beta) |
| Дополнение | Бета | Добавлена сущность [governanceRoleSetting](/graph/api/resources/governancerolesetting?view=graph-rest-beta), а также следующие методы и действия:<br> [Список](/graph/api/governancerolesetting-list?view=graph-rest-beta) <br> [Получение](/graph/api/governancerolesetting-get?view=graph-rest-beta) <br> [Обновление](/graph/api/governancerolesetting-update?view=graph-rest-beta) |
| Дополнение | Бета | Добавлены следующие сложные типы: <br> [governancePermission](/graph/api/resources/governancepermission?view=graph-rest-beta) <br> [governanceRoleAssignmentRequestStatus](/graph/api/resources/governanceroleassignmentrequeststatus?view=graph-rest-beta) <br> [governanceRuleSetting](/graph/api/resources/governancerulesetting?view=graph-rest-beta) <br> [governanceSchedule](/graph/api/resources/governanceschedule?view=graph-rest-beta)|

### <a name="security-apis"></a>API безопасности

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | Бета        | Добавлены новые типы перечисления:<br/>[alertFeedback](/graph/api/resources/alertfeedbackenumtype?view=graph-rest-beta)<br/>[alertStatus](/graph/api/resources/alertstatusenumtype?view=graph-rest-beta)<br/>[alertType](/graph/api/resources/alerttypeenumtype?view=graph-rest-beta)<br/>[applicationPermissionsRequired](/graph/api/resources/applicationpermissionsrequiredenumtype?view=graph-rest-beta)<br/>[logonType](/graph/api/resources/logontypeenumtype?view=graph-rest-beta)<br/>[processIntegrityLevel](/graph/api/resources/processintegritylevelenumtype?view=graph-rest-beta)<br/>[securityNetworkProtocol](/graph/api/resources/securitynetworkprotocolenumtype?view=graph-rest-beta)<br/>[userAccountSecurityType](/graph/api/resources/useraccountsecuritytypeenumtype?view=graph-rest-beta)<br/>

## <a name="may-2018"></a>Май 2018 г.

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | версия 1.0        | Добавлено действие [занесения в список удаленных элементов, принадлежащих пользователю](/graph/api/directory-deleteditems-user-owned?view=graph-rest-1.0) для ресурса [каталога (удаленных элементов)](/graph/api/resources/directory?view=graph-rest-1.0). |
| Дополнение | Бета | В ресурс [directory](/graph/api/resources/directory?view=graph-rest-beta) добавлена функция [getUserOwnedObjects](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta) для перечисления удаленных групп, принадлежащих определенному пользователю. |

### <a name="education-api"></a>API для образования

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета | Разрешение **Members.Read.Hidden** необходимо для чтения или обновления коллекции **Members** в объекте [educationClass](/graph/api/resources/educationclass?view=graph-rest-1.0) с помощью маркеров только для приложения. |
|Изменение           |Бета-версия           |Обновлены возможные значения типа **educationSubmissionStatus** в свойстве status объекта [educationsubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|
|Изменение           |Бета-версия           |Добавлен сложный тип **educationAssignmentIndividualRecipient** к свойству assignTo объекта [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta).|
|Изменение           |Бета-версия           |Добавлены свойства **unsubmittedBy**, **unsubmittedDate**, **returnedBy**, **returnedDate** объекта [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|
|Дополнение         |Бета-версия           |Добавлены действия [return](/graph/api/educationsubmission-return?view=graph-rest-beta) и [unsubmit](/graph/api/educationsubmission-unsubmit?view=graph-rest-beta) для объекта [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|
|Изменение           |Бета-версия           |Удалены действия release и recall для объекта [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|

### <a name="groups"></a>Группы

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета | Добавлено свойство **importance** в объект [post](/graph/api/resources/post?view=graph-rest-1.0). |

### <a name="microsoft-bookings-api"></a>API Microsoft Bookings

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | Бета          | Добавлены объект [bookingBusiness](/graph/api/resources/bookingbusiness?view=graph-rest-beta) и следующие методы и действия CRUD: <br> [перечисление](/graph/api/bookingbusiness-list?view=graph-rest-beta); <br> [создание](/graph/api/bookingbusiness-post-bookingbusinesses?view=graph-rest-beta); <br> [получение](/graph/api/bookingbusiness-get?view=graph-rest-beta); <br> [Обновление](/graph/api/bookingbusiness-update?view=graph-rest-beta) <br> [удаление](/graph/api/bookingbusiness-delete?view=graph-rest-beta); <br> [публикация](/graph/api/bookingbusiness-publish?view=graph-rest-beta); <br> [отмена публикации](/graph/api/bookingbusiness-unpublish?view=graph-rest-beta). <br> Узнайте больше об интеграции с [API Microsoft Bookings](booking-concept-overview.md). |
| Добавление        | Бета          | Добавлены объект [bookingAppointment](/graph/api/resources/bookingappointment?view=graph-rest-beta) и следующие методы и действие CRUD: <br> [перечисление](/graph/api/bookingbusiness-list-appointments?view=graph-rest-beta); <br> [создание](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta); <br> [получение](/graph/api/bookingappointment-get?view=graph-rest-beta); <br> [Обновление](/graph/api/bookingappointment-update?view=graph-rest-beta) <br> [удаление](/graph/api/bookingappointment-delete?view=graph-rest-beta); <br> [отмена](/graph/api/bookingappointment-cancel?view=graph-rest-beta). |
| Добавление        | Бета          | Добавлены объект [bookingCurrency](/graph/api/resources/bookingcurrency?view=graph-rest-beta) и следующие методы: <br> [перечисление](/graph/api/bookingcurrency-list?view=graph-rest-beta); <br> [получение](/graph/api/bookingcurrency-get?view=graph-rest-beta). |
| Добавление        | Бета          | Добавлены объект [bookingCustomer](/graph/api/resources/bookingcustomer?view=graph-rest-beta) и следующие методы CRUD: <br> [перечисление](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta); <br> [создание](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta); <br> [получение](/graph/api/bookingcustomer-get?view=graph-rest-beta); <br> [обновление](/graph/api/bookingcustomer-update?view=graph-rest-beta); <br> [удаление](/graph/api/bookingcustomer-delete?view=graph-rest-beta).|
| Добавление        | Бета          | Добавлены объект [bookingService](/graph/api/resources/bookingservice?view=graph-rest-beta) и следующие методы CRUD: <br> [перечисление](/graph/api/bookingbusiness-list-services?view=graph-rest-beta); <br> [создание](/graph/api/bookingbusiness-post-services?view=graph-rest-beta); <br> [получение](/graph/api/bookingservice-get?view=graph-rest-beta); <br> [обновление](/graph/api/bookingservice-update?view=graph-rest-beta); <br> [удаление](/graph/api/bookingservice-delete?view=graph-rest-beta).|
| Добавление        | Бета          | Добавлены объект [bookingStaffMember](/graph/api/resources/bookingstaffmember?view=graph-rest-beta) и следующие методы CRUD: <br> [перечисление](/graph/api/bookingbusiness-list-staffmembers?view=graph-rest-beta); <br> [создание](/graph/api/bookingbusiness-post-staffmembers?view=graph-rest-beta); <br> [получение](/graph/api/bookingstaffmember-get?view=graph-rest-beta); <br> [обновление](/graph/api/bookingstaffmember-update?view=graph-rest-beta); <br> [удаление](/graph/api/bookingstaffmember-delete?view=graph-rest-beta).|
| Добавление        | Бета          | Добавлены следующие сложные типы: <br> [bookingNamedEntity](/graph/api/resources/bookingnamedentity?view=graph-rest-beta); <br> [bookingPerson](/graph/api/resources/bookingperson?view=graph-rest-beta); <br> [bookingReminder](/graph/api/resources/bookingreminder?view=graph-rest-beta); <br> [bookingWorkHours](/graph/api/resources/bookingworkhours?view=graph-rest-beta); <br> [bookingWorkTimeSlot](/graph/api/resources/bookingworktimeslot?view=graph-rest-beta).|

### <a name="microsoft-intune-apis"></a>API Microsoft Intune
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta);<br/>[easEmailProfileConfigurationBase](/graph/api/resources/intune-deviceconfig-easemailprofileconfigurationbase?view=graph-rest-beta);<br/>[mobileAppIntentAndState](/graph/api/resources/intune-troubleshooting-mobileappintentandstate?view=graph-rest-beta);<br/>[mobileAppTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingevent?view=graph-rest-beta);<br/>[unsupportedDeviceConfiguration](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfiguration?view=graph-rest-beta);<br/>[windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta).<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[managedDeviceCleanupSettings](/graph/api/resources/intune-devices-manageddevicecleanupsettings?view=graph-rest-beta);<br/>[mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta);<br/>[mobileAppTroubleshootingAppPolicyCreationHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapppolicycreationhistory?view=graph-rest-beta);<br/>[mobileAppTroubleshootingAppStateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappstatehistory?view=graph-rest-beta);<br/>[mobileAppTroubleshootingAppTargetHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapptargethistory?view=graph-rest-beta);<br/>[mobileAppTroubleshootingAppUpdateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappupdatehistory?view=graph-rest-beta);<br/>[mobileAppTroubleshootingDeviceCheckinHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingdevicecheckinhistory?view=graph-rest-beta);<br/>[mobileAppTroubleshootingHistoryItem](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem?view=graph-rest-beta);<br/>[unsupportedDeviceConfigurationDetail](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail?view=graph-rest-beta);<br/>**windowsAutoPilotEnrollmentSettings**;<br/>[windowsKioskActiveDirectoryGroup](/graph/api/resources/intune-deviceconfig-windowskioskactivedirectorygroup?view=graph-rest-beta);<br/>[windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta);<br/>[windowsKioskAppConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskappconfiguration?view=graph-rest-beta);<br/>[windowsKioskAutologon](/graph/api/resources/intune-deviceconfig-windowskioskautologon?view=graph-rest-beta);<br/>[windowsKioskAzureADGroup](/graph/api/resources/intune-deviceconfig-windowskioskazureadgroup?view=graph-rest-beta);<br/>[windowsKioskAzureADUser](/graph/api/resources/intune-deviceconfig-windowskioskazureaduser?view=graph-rest-beta);<br/>[windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta);<br/>[windowsKioskLocalGroup](/graph/api/resources/intune-deviceconfig-windowskiosklocalgroup?view=graph-rest-beta);<br/>[windowsKioskLocalUser](/graph/api/resources/intune-deviceconfig-windowskiosklocaluser?view=graph-rest-beta);<br/>[windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta);<br/>[windowsKioskProfile](/graph/api/resources/intune-deviceconfig-windowskioskprofile?view=graph-rest-beta);<br/>[windowsKioskSingleUWPApp](/graph/api/resources/intune-deviceconfig-windowskiosksingleuwpapp?view=graph-rest-beta);<br/>[windowsKioskUser](/graph/api/resources/intune-deviceconfig-windowskioskuser?view=graph-rest-beta);<br/>[windowsKioskUWPApp](/graph/api/resources/intune-deviceconfig-windowskioskuwpapp?view=graph-rest-beta);<br/>[windowsKioskVisitor](/graph/api/resources/intune-deviceconfig-windowskioskvisitor?view=graph-rest-beta).<br/>|
|Дополнение|Бета|Добавлены новые типы перечисления:<br/>[defenderScheduleScanDay](/graph/api/resources/intune-deviceconfig-defenderschedulescanday?view=graph-rest-beta);<br/>[defenderSubmitSamplesConsentType](/graph/api/resources/intune-deviceconfig-defendersubmitsamplesconsenttype?view=graph-rest-beta);<br/>[domainNameSource](/graph/api/resources/intune-deviceconfig-domainnamesource?view=graph-rest-beta);<br/>[localSecurityOptionsSmartCardRemovalBehaviorType](/graph/api/resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype?view=graph-rest-beta);<br/>[mobileAppActionType](/graph/api/resources/intune-troubleshooting-mobileappactiontype?view=graph-rest-beta);<br/>[mobileAppIntent](/graph/api/resources/intune-troubleshooting-mobileappintent?view=graph-rest-beta);<br/>[roleAssignmentScopeType](/graph/api/resources/intune-rbac-roleassignmentscopetype?view=graph-rest-beta);<br/>[usernameSource](/graph/api/resources/intune-deviceconfig-usernamesource?view=graph-rest-beta);<br/>[windowsDeviceUsageType](/graph/api/resources/intune-enrollment-windowsdeviceusagetype?view=graph-rest-beta).<br/>|
|Дополнение|Бета-версия|Добавлено действие [setDeviceName](/graph/api/intune-devices-manageddevice-setdevicename?view=graph-rest-beta)<br/>для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Удаление|Бета|Удалены следующие объекты:<br/>**depEnrollmentProfile**;<br/>**enrollmentProfile**;<br/>**importedAppleDeviceIdentity**<br/>**importedAppleDeviceIdentityResult**.<br/>|
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**managementCertificateWithThumbprint**.<br/>|
|Удаление|Бета|Удалены следующие типы перечисления:<br/>**depTokenType**;<br/>**discoverySource**;<br/>**iTunesPairingMode**.<br/>|
|Удаление|Бета-версия|Удалено действие importAppleDeviceIdentityList для коллекции [importedAppleDeviceIdentity](/graph/api/resources/intune-corpenrollment-importedappledeviceidentity?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалено действие [updateDeviceProfileAssignment](/graph/api/intune-corpenrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta) для объекта [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалено действие setDefaultProfile для объекта [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалено действие shareForSchoolDataSyncService для объекта [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалено действие unshareForSchoolDataSyncService для объекта [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
|Удаление|бета|Удалена функция exportMobileConfig](/graph/api/intune_corpenrollment_enrollmentprofile_exportmobileconfig?view=graph-rest-beta) для объекта [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлены свойства **userDomainNameSource** и **customDomainName** объекта [androidEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-androideasemailprofileconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **workProfileBlockCamera** и **workProfileBlockCrossProfileContactsSearch** объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **workProfileBlockCamera** и **workProfileBlockCrossProfileContactsSearch** объекта [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **thirdPartyKeyboardsBlocked** и **filterOpenInToOnlyManagedApps** объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **conflictCount** объекта [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **conflictCount** объекта [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **managedDeviceCleanupSettings** объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалено свойство **usernameSource** объекта [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **thirdPartyKeyboardsBlocked** и **filterOpenInToOnlyManagedApps** объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **ignoreVersionDetection** объекта [macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **pinRequiredOnLaunchInsteadOfBiometric** и **pinRequiredInsteadOfBiometricTimeout** объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **autopilotEnrolled**, **requireUserEnrollmentApproval**, **iccid** и **udid** объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалено свойство **isAutopilotEnrolled** объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **notApplicablePlatformCount** и **conflictCount** объекта [managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **conflictCount** для объекта [managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **scopeType** объекта [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалено свойство **usernameSource** объекта [windows10EasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windows10easemailprofileconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees**, **localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers**, **localSecurityOptionsDisableServerDigitallySignCommunicationsAlways**, **localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees**, **localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares**, **localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts**, **localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares**, **localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange** и **localSecurityOptionsSmartCardRemovalBehavior** объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **showInstallationProgress**, **blockDeviceSetupRetryByUser**, **allowDeviceResetOnInstallFailure**, **allowLogCollectionOnInstallFailure**, **customErrorMessage**, **installProgressTimeoutInMinutes** и **allowDeviceUseOnInstallFailure** объекта [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалены свойства **title**, **bodyText**, **moreInfoUrl** и **moreInfoText** объекта [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **defenderBlockOnAccessProtection**, **defenderScheduleScanDay** и **defenderSubmitSamplesConsentType** объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **language** и **enrollmentSettings** объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **useDeviceContext** объекта [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалено свойство **usernameSource** объекта [windowsPhoneEASEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалено свойство навигации **localActions** объекта [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалены свойства навигации **enrollmentProfiles** и **importedAppleDeviceIdentities** объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства навигации **mobileAppIntentAndStates** и **mobileAppTroubleshootingEvents** объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **deviceUsageType** и **skipKeyboardSelectionPage** к сложному типу [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta).|
|Удаление|Бета-версия|Удален элемент **paloAltoGlobalProtect** из типа перечисления [androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены элементы **samAccountName** и **primarySmtpAddress** к типу перечисления [androidUsernameSource](/graph/api/resources/intune-deviceconfig-androidusernamesource?view=graph-rest-beta).|
|Удаление|Бета-версия|Удален элемент **paloAltoGlobalProtect** из типа перечисления [androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлен элемент **paloAltoGlobalProtect** к типу перечисления [windows10VpnConnectionType](/graph/api/resources/intune-deviceconfig-windows10vpnconnectiontype?view=graph-rest-beta).|

### <a name="insights-api"></a>API аналитики

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | Бета          | Добавлены объект [settings](/graph/api/resources/user-settings?view=graph-rest-beta) и следующие методы CRUD: <br> [получение](/graph/api/user-get-settings?view=graph-rest-beta); <br> [обновление](/graph/api/user-update-settings?view=graph-rest-beta). |

### <a name="azure-ad-apis"></a>API Azure AD

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение           | Бета          | Свойство **creatorUserId** сущности [subscription](/graph/api/resources/subscription?view=graph-rest-beta) переименовано в **creatorId** для лучшего отражения смысла. |

## <a name="april-2018"></a>Апрель 2018 г.

### <a name="audit-log-api"></a>API журнала аудита

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены объекты [directoryAudit](/graph/api/resources/directoryaudit?view=graph-rest-beta) и [signIn](/graph/api/resources/signin?view=graph-rest-beta) для поддержки нового API журнала аудита. |
|Добавление|Бета|Добавлены следующие ресурсы для поддержки API журнала аудита: [appIndentity](/graph/api/resources/appidentity?view=graph-rest-beta), [auditActivityInitiator](/graph/api/resources/auditactivityinitiator?view=graph-rest-beta), [conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta), [deviceDetail](/graph/api/resources/devicedetail?view=graph-rest-beta), [mfaDetail](/graph/api/resources/mfadetail?view=graph-rest-beta), [modifiedProperty](/graph/api/resources/modifiedproperty?view=graph-rest-beta), [signinLocation](/graph/api/resources/signinlocation?view=graph-rest-beta), [signinStatus](/graph/api/resources/signinstatus?view=graph-rest-beta), [targetResource](/graph/api/resources/targetresource?view=graph-rest-beta), [targetResourceApp](/graph/api/resources/targetresourceapp?view=graph-rest-beta), [targetResourceDevice](/graph/api/resources/targetresourcedevice?view=graph-rest-beta), [targetResourceDirectory](/graph/api/resources/targetresourcedirectory?view=graph-rest-beta), [targetResourceGroup](/graph/api/resources/targetresourcegroup?view=graph-rest-beta), [targetResourceOther](/graph/api/resources/targetresourceother?view=graph-rest-beta), [targetResourcePolicy](/graph/api/resources/targetresourcepolicy?view=graph-rest-beta), [targetResourceRole](/graph/api/resources/targetresourcerole?view=graph-rest-beta), [targetResourceServicePrincipal](/graph/api/resources/targetresourceserviceprincipal?view=graph-rest-beta), [targetResourceUser](/graph/api/resources/targetresourceuser?view=graph-rest-beta), [userIdentity](/graph/api/resources/useridentity?view=graph-rest-beta) |

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен сложный тип **privacyProfile** для объекта [organization](/graph/api/resources/organization?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлен сложный тип **legalAgeGroup, ageGroup and consentProvidedForMinor** для объекта [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Добавление        | 1.0        | Добавлена поддержка пользователей и групп для подписок на уведомления [веб-перехватчика](/graph/api/resources/webhooks?view=graph-rest-1.0). |
| Добавление        | Бета        | Добавлено действие [перечисления удаленных элементов, принадлежащих пользователю,](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta) для ресурса [каталог (удаленные элементы)](/graph/api/resources/directory?view=graph-rest-beta). |

### <a name="education-apis"></a>API для образования

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Изменение|Бета-версия|Добавлено свойство reportableIdentifier объекта [educationsynchronizationerror](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta).|
|Изменение|Бета-версия|Обновлены варианты ответа для API [uploadUrl](/graph/api/educationsynchronizationprofile-uploadurl?view=graph-rest-beta).|
|Изменение|Бета-версия|Обновлен текст описания типа ресурса [educationSynchronizationError](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta).|
|Изменение|Бета-версия|Обновлен текст описания для API [получения ошибок синхронизации](/graph/api/educationsynchronizationerrors-get?view=graph-rest-beta).|


### <a name="microsoft-intune-apis"></a>API Microsoft Intune
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлены новые объекты:<br/>[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-1.0).<br/>|
|Дополнение|1.0|Добавлены новые типы перечисления:<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-1.0).<br/>|
|Добавление|1.0|Добавлено свойство **managedDeviceOwnerType** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0).|
|Добавление|1.0|Добавлено свойство навигации **deviceStatuses** для объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0).|
|Добавление|1.0|Добавлен член **androidWorkProfile** для типа перечисления [policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-1.0).|
|Добавление|Бета|Добавлены новые объекты:<br/>[androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilecustomconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofileeasemailprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate?view=graph-rest-beta)<br/>[androidWorkProfileVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilewificonfiguration?view=graph-rest-beta)<br/>[restrictedAppsViolation](/graph/api/resources/intune-deviceconfig-restrictedappsviolation?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfileAssignment](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofileassignment?view=graph-rest-beta)<br/>|
|Добавление|Бета|Добавлены новые сложные типы:<br/>[managedDeviceModelsAndManufacturers](/graph/api/resources/intune-devices-manageddevicemodelsandmanufacturers?view=graph-rest-beta)<br/>[managedDeviceReportedApp](/graph/api/resources/intune-devices-manageddevicereportedapp?view=graph-rest-beta)<br/>[windowsEnrollmentStatusScreenSettings](/graph/api/resources/intune-enrollment-windowsenrollmentstatusscreensettings?view=graph-rest-beta)<br/>|
|Добавление|Бета|Добавлены новые типы перечисления:<br/>[androidWorkProfileCrossProfileDataSharingType](/graph/api/resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype?view=graph-rest-beta)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](/graph/api/resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype?view=graph-rest-beta)<br/>[androidWorkProfileRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype?view=graph-rest-beta)<br/>[androidWorkProfileVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconnectiontype?view=graph-rest-beta)<br/>[bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta)<br/>[localSecurityOptionsInformationShownOnLockScreenType](/graph/api/resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype?view=graph-rest-beta)<br/>[managedAppRemediationAction](/graph/api/resources/intune-mam-managedappremediationaction?view=graph-rest-beta)<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-beta)<br/>[restrictedAppsState](/graph/api/resources/intune-deviceconfig-restrictedappsstate?view=graph-rest-beta)<br/>[windows10VpnProfileTarget](/graph/api/resources/intune-deviceconfig-windows10vpnprofiletarget?view=graph-rest-beta)<br/>|
|Добавление|Бета|Добавлено действие [playLostModeSound](/graph/api/intune-devices-manageddevice-playlostmodesound?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Удаление|Бета|Удалены следующие типы перечисления:<br/>**bitLockerRecoveryinformationType**<br/>**windowsUpdateRestartMode**<br/>|
|Добавление|бета|Добавлены свойства **workProfileBlockScreenCapture** и **workProfileBlockCrossProfileCallerId** для объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta).|
|Добавление|Бета|Добавлены свойства **minimumWipePatchVersion**, **allowedAndroidDeviceManufacturers** и **appActionIfAndroidDeviceManufacturerNotAllowed** для объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta).|
|Добавление|Бета|Добавлены свойства **minimumWipeSdkVersion**, **minimumWipePatchVersion**, **allowedIosDeviceModels**, **appActionIfIosDeviceModelNotAllowed**, **allowedAndroidDeviceManufacturers** и **appActionIfAndroidDeviceManufacturerNotAllowed** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta).|
|Добавление|Бета|Добавлены свойства **notApplicablePlatformCount** и **conflictCount** для объекта [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta).|
|Добавление|Бета|Добавлены свойства **notApplicablePlatformCount** и **conflictCount** для объекта [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta).|
|Добавление|Бета|Добавлено свойство **accountMoveCompletionDateTime** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta).|
|Добавление|Бета|Добавлены свойства **minimumWipeSdkVersion**, **allowedIosDeviceModels** и **appActionIfIosDeviceModelNotAllowed** для объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta).|
|Добавление|Бета|Добавлены свойства **minimumWipeOsVersion**, **minimumWipeAppVersion**, **appActionIfDeviceComplianceRequired** и **appActionIfMaximumPinRetriesExceeded** для объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta).|
|Добавление|Бета|Добавлены свойства **managedDeviceOwnerType**, **preferMdmOverGroupPolicyAppliedDateTime**, **isAutopilotEnrolled** и **requestUserEnrollmentApproval** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Добавление|Бета|Добавлено свойство **managedDeviceModelsAndManufacturers** для объекта [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta).|
|Добавление|Бета|Добавлены свойства **localSecurityOptionsMachineInactivityLimitInMinutes**, **localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool**, **localSecurityOptionsInformationShownOnLockScreen**, **defenderSecurityCenterDisableAccountUI**, **defenderSecurityCenterDisableHardwareUI**, **defenderSecurityCenterDisableRansomwareUI**, **defenderSecurityCenterDisableSecureBootUI** и **defenderSecurityCenterDisableTroubleshootingUI** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta).|
|Добавление|Бета|Добавлены свойства **printerNames**, **printerDefaultName**, **printerBlockAddition** и **searchBlockWebResults** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|
|Добавление|Бета|Добавлены свойства **profileTarget**, **enableAlwaysOn** и **enableDeviceTunnel** для объекта [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta).|
|Добавление|Бета|Добавлено свойство **enrollmentStatusScreenSettings** для объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta).|
|Добавление|Бета|Добавлено свойство навигации **deviceConfigurationRestrictedAppsViolations** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta).|
|Добавление|Бета|Добавлено свойство навигации **assignments** для объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta).|
|Добавление|Бета|Добавлено свойство навигации **networkAccessConfigurations** для объекта [windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta).|
|Удаление|Бета|Удалено свойство **permissions** из сложного типа [auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta).|
|Изменение|Бета|Изменен тип следующих свойств сложного типа [bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta):<br/>**recoveryInformationToStore** с [bitLockerRecoveryinformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta) на [bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta).<br/>|
|Добавление|Бета|Добавлено свойство **deviceInactivityBeforeRetirementInDay** для сложного типа [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta).|
|Добавление|Бета|Добавлено свойство **landingPageCustomizedImage** для сложного типа [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta).|
|Удаление|Бета|Удалено свойство **ipAddressOrFqdn** из сложного типа [vpnServer](/graph/api/resources/intune-deviceconfig-vpnserver?view=graph-rest-beta).|
|Удаление|Бета|Удалено свойство **restartMode** из сложного типа [windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta).|
|Добавление|Бета|Добавлен член **paloAltoGlobalProtect** для типа перечисления [androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta).|
|Добавление|Бета|Добавлен член **paloAltoGlobalProtect** для типа перечисления [androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta).|
|Добавление|Бета|Добавлен член **paloAltoGlobalProtect** для типа перечисления [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta).|
|Добавление|Бета|Добавлен член **androidWorkProfile** для типа перечисления [policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-beta).|

### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Добавлено свойство **locations** для объекта [event](/graph/api/resources/event?view=graph-rest-1.0), позволяющее организовать событие, в котором могут участвовать пользователи из нескольких мест. |
| Дополнение        | 1.0          | Добавлено свойство **locationType** для сложного типа [location](/graph/api/resources/location?view=graph-rest-1.0). |
| Дополнение        | 1.0          | Добавлены свойства **uniqueId** и **uniqueIdType** для сложного типа [location](/graph/api/resources/location?view=graph-rest-1.0). В настоящее время эти свойства предназначены только для внутреннего использования. |


### <a name="outlook-contacts"></a>Контакты Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0          | Добавлено свойство **flag** для объекта [contact](/graph/api/resources/contact?view=graph-rest-1.0). Добавлен общий сложный тип [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0).|


### <a name="outlook-mail"></a>Почта Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0          | Добавлено свойство **flag** для объекта [message](/graph/api/resources/message?view=graph-rest-1.0). Добавлен общий сложный тип [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0).|
| Добавление        | 1.0        | Добавлено свойство **internetMessageHeaders** для объекта [message](/graph/api/resources/message?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлен сложный тип [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлено свойство навигации **messageRules** для объекта [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0). **messageRules** — это набор экземпляров [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлены объект [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0) и сложные типы [messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-1.0), [messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-1.0) и [sizeRange](/graph/api/resources/sizerange?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлены следующие операции CRUD для правил обработки сообщений: [создание](/graph/api/mailfolder-post-messagerules?view=graph-rest-1.0), [перечисление](/graph/api/mailfolder-list-messagerules?view=graph-rest-1.0), [получение](/graph/api/messagerule-get?view=graph-rest-1.0), [обновление](/graph/api/messagerule-update?view=graph-rest-1.0) и [удаление](/graph/api/messagerule-delete?view=graph-rest-1.0). |
| Дополнение | Бета-версия | Добавлен объект [mailSearchFolder](/graph/api/resources/mailsearchfolder?view=graph-rest-beta). |
| Дополнение | Бета-версия | Добавлены следующие API для папки поиска почты: [API создания](/graph/api/mailsearchfolder-post?view=graph-rest-beta), [API обновления](/graph/api/mailsearchfolder-update?view=graph-rest-beta). |
| Изменение | Бета-версия | Для папки поиска почты добавлена поддержка [удаления объекта mailFolder](/graph/api/mailfolder-delete?view=graph-rest-beta), [получения объекта mailFolder](/graph/api/mailfolder-get?view=graph-rest-beta) и [перечисления дочерних папок](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta). |


### <a name="outlook-user-choices"></a>Настройки пользователей Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлено новое свойство навигации **masterCategories** для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0). **masterCategories** — это коллекция объектов [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлен объект [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлены следующие операции CRUD для объекта [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0): [create](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0), [get](/graph/api/outlookcategory-get?view=graph-rest-1.0), [update](/graph/api/outlookcategory-update?view=graph-rest-1.0) и [delete](/graph/api/outlookcategory-delete?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлена новая функция [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-1.0) для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлена новая функция [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-1.0) для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0). |
|Добавление | 1.0 | Добавлено новое свойство **workingHours** для объекта [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0). Сведения о поддерживаемых вариантах использования см. в описании [типа ресурса workingHours](/graph/api/resources/workinghours?view=graph-rest-1.0).|
|Дополнение | 1.0 | Добавлены следующие сложные типы: <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-1.0) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-1.0) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-1.0) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-1.0) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-1.0)|


### <a name="microsoft-teams"></a>Microsoft Teams

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлен новый объект [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-beta).|
|Добавление|Бета|Добавлен новый объект [teamGuestSettings](/graph/api/resources/teamguestsettings?view=graph-rest-beta).|
|Добавление|Бета|Добавлен новый объект [teamMessagingSettings](/graph/api/resources/teammessagingsettings?view=graph-rest-beta).|
|Добавление|Бета|Добавлен новый объект [teamFunSettings](/graph/api/resources/teamfunsettings?view=graph-rest-beta).|
|Добавление|Бета|Добавлена новая операция [удаления канала](/graph/api/channel-delete?view=graph-rest-beta).|
|Добавление|Бета|Добавлена новая операция [исправления канала](/graph/api/channel-patch?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено новое свойство webUrl для ресурса [команды](/graph/api/resources/team?view=graph-rest-beta).|
|Изменение|Бета|Обновлен путь к объекту [channel](/graph/api/resources/channel?view=graph-rest-beta).|


### <a name="project-rome-apis"></a>API Project Rome

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение | 1.0 | Добавлен [API для получения последних действий](/graph/api/projectrome-get-recent-activities?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлен [API для получения действий](/graph/api/projectrome-get-activities?view=graph-rest-1.0). |
| Добавление | 1.0 | Добавлена операция [создания или замены действия](/graph/api/projectrome-put-activity?view=graph-rest-1.0). |
| Добавление | 1.0 | Добавлена операция [создания или замены элемента журнала](/graph/api/projectrome-put-historyitem?view=graph-rest-1.0). |
| Добавление | 1.0 | Добавлена операция [удаления действия](/graph/api/projectrome-delete-activity?view=graph-rest-1.0). |
| Добавление | 1.0 | Добавлена операция [создания или замены элемента журнала](/graph/api/projectrome-delete-historyitem?view=graph-rest-1.0). |
| Добавление | 1.0 | Добавлен тип ресурса [activity](/graph/api/resources/projectrome-activity?view=graph-rest-1.0). |
| Добавление | Версия 10 | Добавлен тип ресурса [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-1.0). |
| Добавление | 1.0 | Добавлен тип ресурса [visualInfo](/graph/api/resources/projectrome-visualinfo?view=graph-rest-1.0). |
| Добавление | 1.0 | Добавлен тип ресурса [imageInfo](/graph/api/resources/projectrome-imageinfo?view=graph-rest-1.0). |
| Добавление | Версия 10 | Добавлен [обзор Project Rome](/graph/api/resources/project-rome-overview?view=graph-rest-1.0). |
| Изменение | Бета | Добавлена документация по глубокой вставке для [создания или замены действия](/graph/api/projectrome-put-activity?view=graph-rest-beta). |

### <a name="reports-apis"></a>API отчетов
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета| Добавлена поддержка делегированного доступа. |
|Добавление|1.0| Добавлена поддержка делегированного доступа. |

### <a name="security-apis"></a>API безопасности

| **Тип изменения** | **Версия** | **Описание**              |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия       | Добавлен [API безопасности](/graph/api/resources/security-api-overview?view=graph-rest-beta), включающий следующие ресурсы и операции:<br/>[оповещение](/graph/api/resources/alert?view=graph-rest-beta) (и соответствующие объекты);<br/>[получение оповещения](/graph/api/alert-get?view=graph-rest-beta);<br/>[перечисление оповещений](/graph/api/alert-list?view=graph-rest-beta);<br/>[обновление оповещения](/graph/api/alert-update?view=graph-rest-beta).<br/><br/>Добавлена следующая вспомогательная документация:<br/>[сведения об ошибках](/graph/api/resources/security-error-codes?view=graph-rest-beta);<br/>[Интеграция с SIEM](security-siemintegration.md)


## <a name="march-2018"></a>Март 2018 г.

### <a name="data-policy-operations"></a>Операции с политикой данных

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлен новый объект [dataPolicyOperation](/graph/api/resources/datapolicyoperation?view=graph-rest-beta). Он представляет собой отправленную операцию с политикой данных с целью отслеживания.
| Добавление        | Бета        | Добавлено действие [exportPersonalData](/graph/api/user-exportpersonaldata?view=graph-rest-beta) для [пользователей](/graph/api/resources/users?view=graph-rest-beta). Это действие отправляет запрос на экспорт персональных данных, которые корпорация Майкрософт хранит для пользователя. |

### <a name="activityfeedservice-apis"></a>API ActivityFeedService

| **Тип изменения** | **Версия** | **Описание**              |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия       | Добавлен API [Получение последних действий](/graph/api/projectrome-get-recent-activities?view=graph-rest-beta). |
| Дополнение        | Бета-версия       | Добавлен API [Получение действий](/graph/api/projectrome-get-activities?view=graph-rest-beta). |
| Изменение | Бета-версия | В API [Upsert Activity](/graph/api/projectrome-put-activity?view=graph-rest-beta) добавлено разрешение UserActivity.ReadWrite.CreatedByApp. |
| Изменение | Бета-версия | В API [Upsert HistoryItem](/graph/api/projectrome-put-historyitem?view=graph-rest-beta) добавлено разрешение UserActivity.ReadWrite.CreatedByApp. |
| Изменение | Бета-версия | В API [Delete Activity](/graph/api/projectrome-delete-activity?view=graph-rest-beta) добавлено разрешение UserActivity.ReadWrite.CreatedByApp. |
| Изменение | Бета-версия | В API [Upsert HistoryItem](/graph/api/projectrome-delete-historyitem?view=graph-rest-beta) добавлено разрешение UserActivity.ReadWrite.CreatedByApp. |
| Изменение | Бета-версия | В ресурс [activity](/graph/api/resources/projectrome-activity?view=graph-rest-beta) добавлено свойство **status**. |
| Изменение | Бета-версия | В ресурс [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta) добавлено свойство навигации **activity**. |
| Изменение | Бета-версия | В [общие сведения о Project Rome](/graph/api/resources/project-rome-overview?view=graph-rest-beta) добавлены новые API. |

### <a name="azure-ad-apis"></a>API Azure AD

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Изменение|Бета-версия|Добавлены свойства **applicationID** и **creatorUserID** ресурса [subscription](/graph/api/resources/subscription?view=graph-rest-beta). |
|Изменение|Бета-версия|Добавлена операция [list](/graph/api/subscription-list?view=graph-rest-beta) для объекта [subscription](/graph/api/resources/subscription?view=graph-rest-beta). |


### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлен сложный тип **onPremisesExtensionAttributes** для объекта [user](/graph/api/resources/user?view=graph-rest-beta). Он содержит локальные атрибуты расширения AD 1–15. |
| Добавление        | Бета        | Добавлен сложный тип **privacyProfile** для объекта [organization](/graph/api/resources/organization?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлена поддержка [восстановления и окончательного удаления пользователей и групп](/graph/api/resources/directory?view=graph-rest-1.0). |

### <a name="excel-apis"></a>API Excel

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Изменение|1.0|Добавлено свойство **legacyId** для объекта [Excel Table](/graph/api/resources/table?view=graph-rest-1.0). Оно будет содержать числовой идентификатор (строковый тип данных), который будет оставаться постоянным для определенной таблицы Excel. Это свойство входит в состав дополнительных метаданных, если приложение использует устаревший идентификатор из старых клиентских приложений Excel. Примечание. Свойства `id` и `legacyId` должны интерпретироваться как непрозрачные строковые значения и не должны преобразовываться в другой тип в приложении. |

### <a name="reports-apis"></a>API отчетов

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Дополнение|Бета-версия|Добавлено свойство **siteId** для объекта [sharePointSiteUsageDetail](/graph/api/resources/sharepointsiteusagedetail?view=graph-rest-beta).|

### <a name="group-lifecycle-policy"></a>Политика жизненного цикла группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен объект [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-1.0) |
| Добавление        | 1.0        | Для политики жизненного цикла группы добавлены API [создания](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-1.0), [перечисления](/graph/api/grouplifecyclepolicy-list?view=graph-rest-1.0), [получения](/graph/api/grouplifecyclepolicy-get?view=graph-rest-1.0), [обновления](/graph/api/grouplifecyclepolicy-update?view=graph-rest-1.0), [удаления](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-1.0), [добавления группы](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-1.0), [удаления группы](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-1.0) |
| Добавление        | 1.0        | Добавлена функция [перечисления groupLifecyclePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-1.0) для [group](/graph/api/resources/group?view=graph-rest-1.0) |
| Изменение | 1.0 | Добавлено свойство renewedDateTime и [renew](/graph/api/group-renew?view=graph-rest-1.0) для [group](/graph/api/resources/group?view=graph-rest-1.0). |

### <a name="terms-of-use"></a>Условия использования

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены ресурсы [agreement](/graph/api/resources/agreement?view=graph-rest-beta) и [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Для ресурса [agreement](/graph/api/resources/agreement?view=graph-rest-beta) добавлены API [создания](/graph/api/greement-post-agreements?view=graph-rest-beta), [перечисления](/graph/api/agreement-list?view=graph-rest-beta), [получения](/graph/api/agreement-get?view=graph-rest-beta), [обновления](/graph/api/agreement-update?view=graph-rest-beta) и [удаления](/graph/api/agreement-delete?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Для ресурса [user](/graph/api/resources/user?view=graph-rest-beta) добавлены отношения [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta). |

### <a name="microsoft-intune-apis"></a>API Microsoft Intune

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлены новые объекты:<br/>[iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-1.0);<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0).<br/>|
|Дополнение|1.0|Добавлены новые сложные типы:<br/>[appConfigurationSettingItem](/graph/api/resources/intune-apps-appconfigurationsettingitem?view=graph-rest-1.0).<br/>|
|Дополнение|1.0|Добавлено действие [syncLicenses](/graph/api/intune-onboarding-vpptoken-synclicenses?view=graph-rest-1.0) для объекта [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлено свойство навигации **vppTokens** для объекта [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0).|
|Дополнение|Бета-версия|Добавлено свойство **managementCertificateExpirationDate** объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **enhancedJailBreak** для сложного типа [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta);<br/>[androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta);<br/>[androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta);<br/>[androidManagedStoreAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschema?view=graph-rest-beta);<br/>[dataSharingConsent](/graph/api/resources/intune-devices-datasharingconsent?view=graph-rest-beta);<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta);<br/>[macOSEndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-macosendpointprotectionconfiguration?view=graph-rest-beta);<br/>[macOSImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-macosimportedpfxcertificateprofile?view=graph-rest-beta);<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta);<br/>[managedEBookCategory](/graph/api/resources/intune-books-managedebookcategory?view=graph-rest-beta);<br/>[microsoftStoreForBusinessContainedApp](/graph/api/resources/intune-apps-microsoftstoreforbusinesscontainedapp?view=graph-rest-beta);<br/>[mobileContainedApp](/graph/api/resources/intune-apps-mobilecontainedapp?view=graph-rest-beta);<br/>[windowsUniversalAppXContainedApp](/graph/api/resources/intune-apps-windowsuniversalappxcontainedapp?view=graph-rest-beta).<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[androidManagedStoreAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem?view=graph-rest-beta);<br/>[deviceAndAppManagementData](/graph/api/resources/intune-onboarding-deviceandappmanagementdata?view=graph-rest-beta);<br/>[loggedOnUser](/graph/api/resources/intune-devices-loggedonuser?view=graph-rest-beta);<br/>[macOSFirewallApplication](/graph/api/resources/intune-deviceconfig-macosfirewallapplication?view=graph-rest-beta);<br/>[macOSLobChildApp](/graph/api/resources/intune-apps-macoslobchildapp?view=graph-rest-beta);<br/>[macOSMinimumOperatingSystem](/graph/api/resources/intune-apps-macosminimumoperatingsystem?view=graph-rest-beta);<br/>[windowsAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsappxappassignmentsettings?view=graph-rest-beta);<br/>[windowsUniversalAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsuniversalappxappassignmentsettings?view=graph-rest-beta).<br/>|
|Дополнение|Бета|Для ресурса [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) добавлено действие [requestSignupUrl](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl?view=graph-rest-beta). |
|Дополнение|Бета|Для ресурса [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) добавлено действие [completeSignup](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено действие [syncApps](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps?view=graph-rest-beta) для ресурса [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено действие [unbind](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind?view=graph-rest-beta) для ресурса [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено действие [revokeToken](/graph/api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken?view=graph-rest-beta) для ресурса [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено действие [createToken](/graph/api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken?view=graph-rest-beta) для ресурса [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено действие [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) для ресурса [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено действие [consentToDataSharing](/graph/api/intune-devices-datasharingconsent-consenttodatasharing?view=graph-rest-beta) для ресурса [dataSharingConsent](/graph/api/resources/intune-devices-datasharingconsent?view=graph-rest-beta). |
|Дополнение|Бета|Добавлена функция [getLoggedOnManagedDevices](/graph/api/intune-devices-user-getloggedonmanageddevices?view=graph-rest-beta) для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta). |
|Дополнение|Бета|Добавлена функция [exportDeviceAndAppManagementData](/graph/api/intune-onboarding-user-exportdeviceandappmanagementdata?view=graph-rest-beta) для объекта [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta). |
|Дополнение|Бета|Добавлена функция [exportDeviceAndAppManagementData](/graph/api/intune-onboarding-user-exportdeviceandappmanagementdata?view=graph-rest-beta) для объекта [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta). |
|Удаление|Бета|Удалены следующие объекты:<br/>**appleVolumePurchaseProgramToken**;<br/>**mdmAppConfigGroupAssignment**;<br/>**windows10KioskConfiguration**.<br/>|
|Удаление|Бета|Удалено действие [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) для ресурса [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta). |
|Удаление|Бета|Удалено действие [syncApps](/graph/api/intune-onboarding-applevolumepurchaseprogramtoken-syncapps?view=graph-rest-beta) для ресурса [appleVolumePurchaseProgramToken](/graph/api/resources/intune-onboarding-applevolumepurchaseprogramtoken?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено свойство **workProfileBluetoothEnableContactSharing** в объект [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **intendedPurpose** в объект [androidForWorkImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **intendedPurpose** в объект [androidImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidimportedpfxcertificateprofile?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **intendedPurpose** в объект [iosImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-iosimportedpfxcertificateprofile?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **encodedSettingXml** в объект [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **managedDeviceId** и **azureADDeviceId** в объект [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **usersLoggedOn** в объект [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Удаление|Бета|Удалено свойство **lastLoggedOnUserId** из объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **lastModifiedDateTime** в объект [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **isDependency** в объект [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **windowsEnabled**, **macEnabled**, **windowsDeviceBlockedOnMissingPartnerData** и **macDeviceBlockedOnMissingPartnerData** в объект [mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **shouldUninstallOlderVersionsOfOffice** в объект [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **dataSharingConsentGranted** в объект [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **localSecurityOptionsBlockRemoteLogonWithBlankPassword**, **localSecurityOptionsAdministratorAccountName**, **localSecurityOptionsEnableGuestAccount**, **localSecurityOptionsGuestAccountName**, **localSecurityOptionsAllowUndockWithoutHavingToLogon**, **localSecurityOptionsBlockUsersInstallingPrinterDrivers**, **localSecurityOptionsBlockRemoteOpticalDriveAccess**, **localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser**, **localSecurityOptionsMachineInactivityLimit**, **localSecurityOptionsDoNotRequireCtrlAltDel**, **localSecurityOptionsInformationDisplayedOnLockScreen**, **localSecurityOptionsHideLastSignedInUser**, **localSecurityOptionsHideUsernameAtSignIn**, **localSecurityOptionsLogOnMessageTitle**, **localSecurityOptionsLogOnMessageText**, **localSecurityOptionsAllowPKU2UAuthenticationRequests**, **localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager**, **localSecurityOptionsClearVirtualMemoryPageFile**, **localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn**, **localSecurityOptionsAllowUIAccessApplicationElevation**, **localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations**, **localSecurityOptionsOnlyElevateSignedExecutables**, **localSecurityOptionsAdministratorElevationPromptBehavior**, **localSecurityOptionsStandardUserElevationPromptBehavior**, **localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation**, **localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation**, **localSecurityOptionsAllowUIAccessApplicationsForSecureLocations**, **localSecurityOptionsUseAdminApprovalMode**, **localSecurityOptionsUseAdminApprovalModeForAdministrators**, **deviceGuardLocalSystemAuthorityCredentialGuardSettings**, **deviceGuardEnableVirtualizationBasedSecurity** и **deviceGuardEnableSecureBootWithDMA** в объект [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta).|
|Удаление|Бета|Удалено свойство **defenderPasswordProtectedEmailContentExecutionType** из объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **intendedPurpose** в объект [windows10ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10importedpfxcertificateprofile?view=graph-rest-beta).|
|Удаление|Бета|Удалены свойства **printerNames**, **defaultPrinterName** и **blockAddingNewPrinter** из объекта [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **certificateStore** в объект [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **purchaseOrderIdentifier** в объект [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta).|
|Изменение|Бета|Изменены следующие свойства объекта [windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta):<br/>свойство **subjectAlternativeNameType** преобразовано из требуемого в необязательное.<br/>|
|Дополнение|Бета|Добавлены свойства **advancedThreatProtectionOnboardingFilename** и **advancedThreatProtectionOffboardingFilename** в объект [windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **intendedPurpose** в объект [windowsPhone81ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **skipChecksBeforeRestart** и **updateWeeks** в объект [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство навигации **managedEBookCategories** в объект [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства навигации **androidManagedStoreAccountEnterpriseSettings**, **androidManagedStoreAppConfigurationSchemas**, **androidDeviceOwnerEnrollmentProfiles**, **dataSharingConsents** и **deviceConfigurationUserStateSummaries** в объект [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta).|
|Удаление|Бета|Удалено свойство навигации **deviceSetupConfigurations** из объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta).|
|Удаление|Бета|Удалено свойство навигации **groupAssignments** из объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство навигации **categories** в объект [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство навигации **containedApps** в объект [microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство навигации **containedApps** в объект [mobileAppContent](/graph/api/resources/intune-apps-mobileappcontent?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство навигации **committedContainedApps** для объекта [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta).|

### <a name="onedrive"></a>OneDrive
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлены новые объекты:<br/>[baseItemVersion](/graph/api/resources/baseitemversion?view=graph-rest-1.0);<br/>[driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0);<br/>[listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0).<br/> |
|Добавление|1.0|Добавлены новые сложные типы:<br/>[publicationFacet](/graph/api/resources/publicationfacet?view=graph-rest-1.0).<br/> |
|Добавление|1.0|Добавлено свойство <b>publication</b> для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0). |
|Добавление|1.0|Добавлено свойство навигации <b>versions</b> для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0). |
|Добавление|1.0|Добавлено свойство навигации <b>versions</b> для объекта [listItem](/graph/api/resources/listitem?view=graph-rest-1.0). |
|Добавление|1.0|Добавлено свойство <b>root</b> для объекта [siteCollection](/graph/api/resources/sitecollection?view=graph-rest-1.0). |
|Добавление|1.0|Добавлено действие [restoreVersion](/graph/api/driveitemversion-restore?view=graph-rest-1.0) для объекта [driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0). |
|Добавление|1.0|Добавлено действие [restoreVersion](/graph/api/listitemversion-restore?view=graph-rest-1.0) для объекта [listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0). |


### <a name="onedrive"></a>OneDrive
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлен новый сложный тип:<br/>[itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-beta).<br/> |
|Добавление|Бета|Добавлено свойство <b>name</b> для сложного типа [contentTypeInfo](/graph/api/resources/contenttypeinfo?view=graph-rest-beta). |
|Добавление|Бета|Добавлено свойство <b>objectType</b> для сложного типа [deleteAction](/graph/api/resources/deleteaction?view=graph-rest-beta). |
|Добавление|Бета|Добавлено свойство <b>newName</b> для сложного типа [renameAction](/graph/api/resources/renameaction?view=graph-rest-beta). |
|Добавление|Бета|Добавлено свойство <b>tenantId</b> для сложного типа [sharepointIds](/graph/api/resources/renameaction?view=graph-rest-beta). |
|Добавление|Бета|Добавлено свойство <b>lastRecordedDateTime</b> для сложного типа [itemActivityTimeSet](/graph/api/resources/itemactivitytimeset?view=graph-rest-beta). |
|Добавление|Бета|Добавлено свойство [preview](/graph/api/driveitem-preview?view=graph-rest-beta) для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta). |


## <a name="february-2018"></a>Февраль 2018 г.

### <a name="microsoft-intune-apis"></a>API Microsoft Intune
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidForWorkImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[androidImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[iosImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-iosimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10importedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10KioskConfiguration](/graph/api/resources/intune-deviceconfig-windows10kioskconfiguration?view=graph-rest-beta)<br/>[windowsPhone81ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile?view=graph-rest-beta)<br/>|
|Добавление|Бета|Добавлены новые сложные типы:<br/>[importedWindowsAutopilotDeviceIdentityState](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлена функция [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
|Дополнение|Бета|Добавлена функция [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
|Дополнение|Бета|Добавлена функция [managedDeviceEnrollmentFailureTrends](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuretrends?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
|Добавление|Бета|Добавлена функция [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
|Добавление|Бета|Добавлена функция [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
|Изменение|Бета|Удалены свойства **requireAppVerify**, **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders** и **requireCompanyPortalAppIntegrity** из объекта [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta).|
|Изменение|Бета|Удалены свойства **requireAppVerify**, **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders** и **requireCompanyPortalAppIntegrity** из объекта [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta).|
|Изменение|Бета|Удалены свойства **name**, **modifiedDateTime**, **totalEnrollmentCount** и **qrCode** из объекта [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta).|
|Изменение|Бета|Удалены свойства **nonEapAuthenticationMethodForEapTtls**, **nonEapAuthenticationMethodForPeap** и **enableOuterIdentityPrivacy** из объекта [androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **workProfileBlockAddingAccounts** в объект [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta).|
|Изменение|Бета|Удалены свойства **blockCrossProfileCopyPaste** и **requireAppVerify** из объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **deviceOwnerManagementEnabled** в объект [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta).|
|Изменение|Бета|Удалено свойство **requireAppVerify** из объекта [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **exemptedAppPackages** в объект [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **exemptedAppProtocols** и **exemptedAppPackages** в объект [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **exemptedAppProtocols** в объект [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **lastLoggedOnUserId** в объект [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **isFrameworkFile** в объект [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **targetedAppManagementLevels** в объект [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **localSecurityOptionsBlockMicrosoftAccounts**, **localSecurityOptionsEnableAdministratorAccount**, **defenderPreventCredentialStealingType**, **defenderProcessCreationType**, **defenderUntrustedUSBProcessType**, **defenderUntrustedExecutableType**, ** defenderPasswordProtectedEmailContentExecutionType**, **defenderAdvancedRansomewareProtectionType** и **applicationGuardAllowFileSaveOnHost** в объект [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **edgeFavoritesListLocation** и **edgeBlockEditFavorites** в объект [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **printerNames**, **defaultPrinterName** и **blockAddingNewPrinter** в объект [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство навигации **importedWindowsAutopilotDeviceIdentities** в объект [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **shareAPNSData** для сложного типа [adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta).|
|Изменение|Бета|Удалено свойство **collectFullIOSAppInventory** из сложного типа [adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta).|
|Изменение|Бета|Удалено свойство **deviceUsageType** из сложного типа [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta).|


### <a name="planner-apis"></a>API Планировщика

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[plannerPlanContext](/graph/api/resources/plannerplancontext?view=graph-rest-beta);<br/>[plannerPlanContextDetails](/graph/api/resources/plannerplancontextdetails?view=graph-rest-beta);<br/>[plannerPlanContextCollection](/graph/api/resources/plannerplancontextcollection?view=graph-rest-beta);<br/>[plannerPlanContextDetailsCollection](/graph/api/resources/plannerplancontextdetailscollection?view=graph-rest-beta);<br/>[plannerFavoritePlanReference](/graph/api/resources/plannerfavoriteplanreference?view=graph-rest-beta);<br/>[plannerRecentPlanReference](/graph/api/resources/plannerrecentplanreference?view=graph-rest-beta);<br/>[plannerFavoritePlanReferenceCollection](/graph/api/resources/plannerfavoriteplanreferencecollection?view=graph-rest-beta);<br/>[plannerRecentPlanReferenceCollection](/graph/api/resources/plannerrecentplanreferencecollection?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства `favoritePlanReferences` и `recentPlanReferences` для объекта [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлены свойства навигации `favoritePlans` и `recentPlans` для объекта [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено свойство `contexts` для объекта [plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено свойство `contextDetails` для объекта [plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta). |
|Добавление|Бета|Добавлен [разностный запрос](/graph/api/planneruser-list-delta?view=graph-rest-beta) планировщика. |

### <a name="reports-apis"></a>API отчетов
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | Бета-версия    | Добавлено свойство **activatedOnSharedComputer** для объекта [userActivationCounts](/graph/api/resources/useractivationcounts?view=graph-rest-beta).|
| Дополнение    | Бета    | Добавлено свойство **sharedComputerActivation** для объекта [office365ActivationsUserCounts](/graph/api/resources/office365activationsusercounts?view=graph-rest-beta).|

## <a name="january-2018"></a>Январь 2018 г.

### <a name="json-batching"></a>Пакетная обработка JSON

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Версия 1.0|Добавлена поддержка [пакетной обработки JSON](json-batching.md). Установлено ограничение в 20 внутренних запросов.|
|Изменение|Бета-версия|Максимальное количество внутренних запросов при [пакетной обработке JSON](json-batching.md) увеличено с 5 до 20.|

### <a name="education-apis"></a>API для образования

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены свойства навигации и улучшена поддержка фильтрации для [API списков](/graph/api/resources/education-overview?view=graph-rest-beta).|

### <a name="microsoft-intune-apis"></a>API Microsoft Intune
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлены новые объекты:<br/>[androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-1.0);<br/>[androidCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidcustomconfiguration?view=graph-rest-1.0);<br/>[androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-1.0);<br/>[androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-1.0);<br/>[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-1.0);<br/>[androidManagedAppRegistration](/graph/api/resources/intune-mam-androidmanagedappregistration?view=graph-rest-1.0);<br/>[androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-1.0);<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-1.0);<br/>[applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0);<br/>[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-1.0);<br/>[detectedApp](/graph/api/resources/intune-devices-detectedapp?view=graph-rest-1.0);<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-1.0);<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-1.0);<br/>[deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0);<br/>[deviceCategory](/graph/api/resources/intune-shared-devicecategory?view=graph-rest-1.0);<br/>[deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0);<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-1.0);<br/>[deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-1.0);<br/>[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0);<br/>[deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-1.0);<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-1.0);<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-1.0);<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-1.0);<br/>[deviceComplianceScheduledActionForRule](/graph/api/resources/intune-deviceconfig-devicecompliancescheduledactionforrule?view=graph-rest-1.0);<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-1.0);<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-1.0);<br/>[deviceComplianceUserStatus](/graph/api/resources/intune-deviceconfig-devicecomplianceuserstatus?view=graph-rest-1.0);<br/>[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0);<br/>[deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-1.0);<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-1.0);<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-1.0);<br/>[deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-1.0);<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-1.0);<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-1.0);<br/>[deviceConfigurationUserStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatus?view=graph-rest-1.0);<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0);<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-1.0);<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-1.0);<br/>[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0);<br/>[deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0);<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-1.0);<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-1.0);<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0);<br/>[editionUpgradeConfiguration](/graph/api/resources/intune-deviceconfig-editionupgradeconfiguration?view=graph-rest-1.0);<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-1.0);<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-1.0);<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-1.0);<br/>[iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-1.0);<br/>[iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-1.0);<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-1.0);<br/>[iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-1.0);<br/>[iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-1.0);<br/>[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-1.0);<br/>[iosManagedAppRegistration](/graph/api/resources/intune-mam-iosmanagedappregistration?view=graph-rest-1.0);<br/>[iosStoreApp](/graph/api/resources/intune-apps-iosstoreapp?view=graph-rest-1.0);<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-1.0);<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-1.0);<br/>[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-1.0);<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-1.0);<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-1.0);<br/>[localizedNotificationMessage](/graph/api/resources/intune-notification-localizednotificationmessage?view=graph-rest-1.0);<br/>[macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0);<br/>[macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-1.0);<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-1.0);<br/>[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-1.0);<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-1.0);<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-1.0);<br/>[managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-1.0);<br/>[managedApp](/graph/api/resources/intune-apps-managedapp?view=graph-rest-1.0);<br/>[managedAppConfiguration](/graph/api/resources/intune-mam-managedappconfiguration?view=graph-rest-1.0);<br/>[managedAppOperation](/graph/api/resources/intune-mam-managedappoperation?view=graph-rest-1.0);<br/>[managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-1.0);<br/>[managedAppPolicyDeploymentSummary](/graph/api/resources/intune-mam-managedapppolicydeploymentsummary?view=graph-rest-1.0);<br/>[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0);<br/>[managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0);<br/>[managedAppStatus](/graph/api/resources/intune-mam-managedappstatus?view=graph-rest-1.0);<br/>[managedAppStatusRaw](/graph/api/resources/intune-mam-managedappstatusraw?view=graph-rest-1.0);<br/>[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0);<br/>[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0);<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-1.0);<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-1.0);<br/>[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-1.0);<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-1.0);<br/>[managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-1.0);<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-1.0);<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-1.0);<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-1.0);<br/>[managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-1.0);<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-1.0);<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-1.0);<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-1.0mwindowsinformationprotectionpolicy);<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-1.0);<br/>[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0);<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-1.0);<br/>[mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-1.0);<br/>[mobileAppContent](/graph/api/resources/intune-apps-mobileappcontent?view=graph-rest-1.0);<br/>[mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0);<br/>[mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-1.0);<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-1.0);<br/>[notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-1.0);<br/>[onPremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0);<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0);<br/>[resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-1.0);<br/>[roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-1.0);<br/>[roleDefinition](/graph/api/resources/intune-rbac-roledefinition?view=graph-rest-1.0);<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-1.0);<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-1.0);<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-1.0);<br/>[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0);<br/>targetedManagedAppPolicyAssignment;<br/>[targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-1.0);<br/>[telecomExpenseManagementPartner](/graph/api/resources/intune-tem-telecomexpensemanagementpartner?view=graph-rest-1.0);<br/>[termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-1.0);<br/>[termsAndConditionsAcceptanceStatus](/graph/api/resources/intune-companyterms-termsandconditionsacceptancestatus?view=graph-rest-1.0);<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-1.0);<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-1.0);<br/>[webApp](/graph/api/resources/intune-apps-webapp?view=graph-rest-1.0);<br/>[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-1.0);<br/>[windows10CustomConfiguration](/graph/api/resources/intune-deviceconfig-windows10customconfiguration?view=graph-rest-1.0);<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-1.0);<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-1.0);<br/>[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0);<br/>[windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-1.0);<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-1.0);<br/>[windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-1.0);<br/>[windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-1.0);<br/>[windows81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows81generalconfiguration?view=graph-rest-1.0);<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-1.0);<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-1.0);<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-1.0);<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-1.0);<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-1.0);<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0);<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-1.0);<br/>[windowsPhone81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windowsphone81compliancepolicy?view=graph-rest-1.0);<br/>[windowsPhone81CustomConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81customconfiguration?view=graph-rest-1.0);<br/>[windowsPhone81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81generalconfiguration?view=graph-rest-1.0);<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-1.0);<br/>[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-1.0).<br/>|
|Дополнение|1.0|Добавлены новые сложные типы:<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-1.0);<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-1.0);<br/>[androidMinimumOperatingSystem](/graph/api/resources/intune-apps-androidminimumoperatingsystem?view=graph-rest-1.0);<br/>[androidMobileAppIdentifier](/graph/api/resources/intune-mam-androidmobileappidentifier?view=graph-rest-1.0);<br/>[appListItem](/graph/api/resources/intune-deviceconfig-applistitem?view=graph-rest-1.0);<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-1.0);<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-1.0);<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-1.0);<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devices-deleteuserfromsharedappledeviceactionresult?view=graph-rest-1.0);<br/>[deviceActionResult](/graph/api/resources/intune-devices-deviceactionresult?view=graph-rest-1.0);<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-1.0);<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-1.0);<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-1.0);<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-1.0);<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-devices-deviceexchangeaccessstatesummary?view=graph-rest-1.0)<br/>[deviceGeoLocation](/graph/api/resources/intune-devices-devicegeolocation?view=graph-rest-1.0);<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-1.0);<br/>[deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-1.0);<br/>[deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-1.0);<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-1.0);<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-1.0);<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-1.0);<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-1.0);<br/>[fileEncryptionInfo](/graph/api/resources/intune-apps-fileencryptioninfo?view=graph-rest-1.0);<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-1.0);<br/>[intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-1.0);<br/>[iosDeviceType](/graph/api/resources/intune-apps-iosdevicetype?view=graph-rest-1.0);<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-1.0);<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-1.0)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-1.0)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-1.0)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-1.0);<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-1.0);<br/>[iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0);<br/>[iosMobileAppIdentifier](/graph/api/resources/intune-mam-iosmobileappidentifier?view=graph-rest-1.0);<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-1.0);<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-1.0);<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-1.0);<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-1.0);<br/>[ipRange](/graph/api/resources/intune-mam-iprange?view=graph-rest-1.0);<br/>[iPv4Range](/graph/api/resources/intune-mam-ipv4range?view=graph-rest-1.0);<br/>[iPv6Range](/graph/api/resources/intune-mam-ipv6range?view=graph-rest-1.0);<br/>[keyValuePair](/graph/api/resources/intune-androidforwork-keyvaluepair?view=graph-rest-1.0);<br/>[locateDeviceActionResult](/graph/api/resources/intune-devices-locatedeviceactionresult?view=graph-rest-1.0);<br/>[managedAppDiagnosticStatus](/graph/api/resources/intune-mam-managedappdiagnosticstatus?view=graph-rest-1.0);<br/>[managedAppPolicyDeploymentSummaryPerApp](/graph/api/resources/intune-mam-managedapppolicydeploymentsummaryperapp?view=graph-rest-1.0);<br/>[mediaContentRatingAustralia](/graph/api/resources/intune-deviceconfig-mediacontentratingaustralia?view=graph-rest-1.0);<br/>[mediaContentRatingCanada](/graph/api/resources/intune-deviceconfig-mediacontentratingcanada?view=graph-rest-1.0);<br/>[mediaContentRatingFrance](/graph/api/resources/intune-deviceconfig-mediacontentratingfrance?view=graph-rest-1.0);<br/>[mediaContentRatingGermany](/graph/api/resources/intune-deviceconfig-mediacontentratinggermany?view=graph-rest-1.0);<br/>[mediaContentRatingIreland](/graph/api/resources/intune-deviceconfig-mediacontentratingireland?view=graph-rest-1.0);<br/>[mediaContentRatingJapan](/graph/api/resources/intune-deviceconfig-mediacontentratingjapan?view=graph-rest-1.0);<br/>[mediaContentRatingNewZealand](/graph/api/resources/intune-deviceconfig-mediacontentratingnewzealand?view=graph-rest-1.0);<br/>[mediaContentRatingUnitedKingdom](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedkingdom?view=graph-rest-1.0);<br/>[mediaContentRatingUnitedStates](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedstates?view=graph-rest-1.0);<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-1.0);<br/>[mimeContent](/graph/api/resources/intune-shared-mimecontent?view=graph-rest-1.0);<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-1.0);<br/>[mobileAppIdentifier](/graph/api/resources/intune-mam-mobileappidentifier?view=graph-rest-1.0);<br/>[omaSetting](/graph/api/resources/intune-deviceconfig-omasetting?view=graph-rest-1.0);<br/>[omaSettingBase64](/graph/api/resources/intune-deviceconfig-omasettingbase64?view=graph-rest-1.0);<br/>[omaSettingBoolean](/graph/api/resources/intune-deviceconfig-omasettingboolean?view=graph-rest-1.0);<br/>[omaSettingDateTime](/graph/api/resources/intune-deviceconfig-omasettingdatetime?view=graph-rest-1.0);<br/>[omaSettingFloatingPoint](/graph/api/resources/intune-deviceconfig-omasettingfloatingpoint?view=graph-rest-1.0);<br/>[omaSettingInteger](/graph/api/resources/intune-deviceconfig-omasettinginteger?view=graph-rest-1.0);<br/>[omaSettingString](/graph/api/resources/intune-deviceconfig-omasettingstring?view=graph-rest-1.0);<br/>[omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-1.0);<br/>[proxiedDomain](/graph/api/resources/intune-mam-proxieddomain?view=graph-rest-1.0);<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-1.0);<br/>[resetPasscodeActionResult](/graph/api/resources/intune-devices-resetpasscodeactionresult?view=graph-rest-1.0);<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-1.0);<br/>[rgbColor](/graph/api/resources/intune-onboarding-rgbcolor?view=graph-rest-1.0);<br/>[rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-1.0);<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-1.0);<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-1.0);<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-1.0);<br/>[vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-1.0);<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-1.0);<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-1.0);<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-1.0);<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-1.0);<br/>[windowsDeviceAzureADAccount](/graph/api/resources/intune-devices-windowsdeviceazureadaccount?view=graph-rest-1.0);<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-1.0);<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-1.0);<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-1.0);<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-1.0);<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-1.0);<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-1.0);<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-1.0);<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-1.0);<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-1.0);<br/>[windowsUpdateActiveHoursInstall](/graph/api/resources/intune-deviceconfig-windowsupdateactivehoursinstall?view=graph-rest-1.0);<br/>[windowsUpdateInstallScheduleType](/graph/api/resources/intune-deviceconfig-windowsupdateinstallscheduletype?view=graph-rest-1.0);<br/>[windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-1.0).<br/>|
|Дополнение|Версия 1.0|Добавлено действие [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-1.0) для объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [commit](/graph/api/intune-apps-mobileappcontentfile-commit?view=graph-rest-1.0) для объекта [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [renewUpload](/graph/api/intune-apps-mobileappcontentfile-renewupload?view=graph-rest-1.0) для объекта [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [retire](/graph/api/intune-devices-manageddevice-retire?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [resetPasscode](/graph/api/intune-devices-manageddevice-resetpasscode?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [remoteLock](/graph/api/intune-devices-manageddevice-remotelock?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [requestRemoteAssistance](/graph/api/intune-devices-manageddevice-requestremoteassistance?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [disableLostMode](/graph/api/intune-devices-manageddevice-disablelostmode?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [locateDevice](/graph/api/intune-devices-manageddevice-locatedevice?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [bypassActivationLock](/graph/api/intune-devices-manageddevice-bypassactivationlock?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [rebootNow](/graph/api/intune-devices-manageddevice-rebootnow?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [shutDown](/graph/api/intune-devices-manageddevice-shutdown?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [recoverPasscode](/graph/api/intune-devices-manageddevice-recoverpasscode?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [cleanWindowsDevice](/graph/api/intune-devices-manageddevice-cleanwindowsdevice?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [logoutSharedAppleDeviceActiveUser](/graph/api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [deleteUserFromSharedAppleDevice](/graph/api/intune-devices-manageddevice-deleteuserfromsharedappledevice?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [syncDevice](/graph/api/intune-devices-manageddevice-syncdevice?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [updateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [removeAllDevicesFromManagement](/graph/api/intune-devices-user-removealldevicesfrommanagement?view=graph-rest-1.0) для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-1.0) для объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-1.0) для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [scheduleActionsForRules](/graph/api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules?view=graph-rest-1.0) для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [setMobileDeviceManagementAuthority](/graph/api/intune-onboarding-organization-setmobiledevicemanagementauthority?view=graph-rest-1.0) для объекта [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-1.0) для объекта [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [sync](/graph/api/intune-onboarding-devicemanagementexchangeconnector-sync?view=graph-rest-1.0) для объекта [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [setPriority](/graph/api/intune-onboarding-deviceenrollmentconfiguration-setpriority?view=graph-rest-1.0) для объекта [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [assign](/graph/api/intune-onboarding-deviceenrollmentconfiguration-assign?view=graph-rest-1.0) для объекта [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [assign](/graph/api/intune-mam-targetedmanagedappprotection-assign?view=graph-rest-1.0) для объекта [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [assign](/graph/api/intune-mam-targetedmanagedappconfiguration-assign?view=graph-rest-1.0) для объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [assign](/graph/api/intune-mam-windowsinformationprotection-assign?view=graph-rest-1.0) для объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [targetApps](/graph/api/intune-mam-managedapppolicy-targetapps?view=graph-rest-1.0) для объекта [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [targetApps](/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-1.0) для объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [targetApps](/graph/api/intune-mam-targetedmanagedappconfiguration-targetapps?view=graph-rest-1.0) для объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [wipeManagedAppRegistrationsByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationsbydevicetag?view=graph-rest-1.0) для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [sendTestMessage](/graph/api/intune-notification-notificationmessagetemplate-sendtestmessage?view=graph-rest-1.0) для объекта [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-1.0) для объекта [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-1.0) для объекта [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-1.0) для объекта [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-1.0) для объекта [applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-1.0) для объекта [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-1.0) для объекта [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-onboarding-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-1.0) для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция **getUserIdsWithFlaggedAppRegistration** в коллекции [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [getManagedAppDiagnosticStatuses](/graph/api/intune-mam-user-getmanagedappdiagnosticstatuses?view=graph-rest-1.0) для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [getManagedAppPolicies](/graph/api/intune-mam-user-getmanagedapppolicies?view=graph-rest-1.0) для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-1.0) для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0). |
|Изменение|Версия 1.0|Добавлено свойство **mobileDeviceManagementAuthority** для объекта [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0).|
|Изменение|Версия 1.0|Добавлено свойство **deviceEnrollmentLimit** для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0).|
|Изменение|Версия 1.0|Добавлены свойства навигации **managedDevices**, **managedAppRegistrations** и **deviceManagementTroubleshootingEvents** для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0).|
|||
|Дополнение|Бета|Добавлены новые объекты:<br/>[deviceManagementScriptAssignment](/graph/api/resources/intune-devices-devicemanagementscriptassignment?view=graph-rest-beta);<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-beta);<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-beta).<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[revokeAppleVppLicensesActionResult](/graph/api/resources/intune-devices-revokeapplevpplicensesactionresult?view=graph-rest-beta);<br/>[vppTokenRevokeLicensesActionResult](/graph/api/resources/intune-onboarding-vpptokenrevokelicensesactionresult?view=graph-rest-beta).<br/>|
|Дополнение|Бета-версия|Добавлено действие [revokeToken](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketoken?view=graph-rest-beta) для объекта [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-beta) для объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [assign](/graph/api/intune-devices-devicemanagementscript-assign?view=graph-rest-beta) к объекту [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [revokeAppleVppLicenses](/graph/api/intune-devices-manageddevice-revokeapplevpplicenses?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-beta) для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [revokeLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta) для объекта [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие [wipeManagedAppRegistrationsByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationsbydevicetag?view=graph-rest-beta) для объекта [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено действие [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) для объекта [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлена функция [getEffectiveDeviceEnrollmentConfigurations](/graph/api/intune-onboarding-user-geteffectivedeviceenrollmentconfigurations?view=graph-rest-beta) для объекта [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**appReportingOverviewStatus**;<br/>**complianceSettingStateSummary**;<br/>**deviceConfigurationUserStateSummary**;<br/>**eBookGroupAssignment**;<br/>**eBookVppGroupAssignment**;<br/>**mobileAppGroupAssignment**;<br/>**mobileAppVppGroupAssignment**.<br/>|
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**androidForWorkAppConfigurationExample**;<br/>**androidForWorkAppConfigurationExampleJson**;<br/>**appInstallationFailure**;<br/>**appsComplianceListItem**;<br/>**defaultDeviceEnrollmentRestrictions**;<br/>**defaultDeviceEnrollmentWindowsHelloForBusinessSettings**;<br/>**deviceEnrollmentPlatformRestrictions**.<br/>|
|Изменение|Бета-версия|Добавлены свойства **securityRequireVerifyApps**, **securityRequireSafetyNetAttestationBasicIntegrity**, **securityRequireSafetyNetAttestationCertifiedDevice**, **securityRequireGooglePlayServices**, **securityRequireUpToDateSecurityProviders** и **securityRequireCompanyPortalAppIntegrity** для объекта [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **packageId** для объекта [androidForWorkApp](/graph/api/resources/intune-apps-androidforworkapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Изменен тип следующих свойств объекта [androidForWorkAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschema?view=graph-rest-beta):<br/>вместо **exampleJson** [androidForWorkAppConfigurationExample](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexample?view=graph-rest-beta) теперь используется Binary.<br/>|
|Изменение|Бета-версия|Добавлены свойства **securityRequireVerifyApps**, **securityRequireSafetyNetAttestationBasicIntegrity**, **securityRequireSafetyNetAttestationCertifiedDevice**, **securityRequireGooglePlayServices**, **securityRequireUpToDateSecurityProviders** и **securityRequireCompanyPortalAppIntegrity** для объекта [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **displayName**, **lastModifiedDateTime**, **enrolledDeviceCount**, **qrCodeContent** и **qrCodeImage** для объекта [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **isTokenActive** для объекта [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **innerAuthenticationProtocolForEapTtls**, **innerAuthenticationProtocolForPeap** и **outerIdentityPrivacyTemporaryValue** для объекта [androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **workProfileBlockCrossProfileCopyPaste** и **securityRequireVerifyApps** для объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **securityRequireVerifyApps** для объекта [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **packageId** и **identityVersion** для объекта [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **packageId** для объекта [androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **faceIdBlocked** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **members** для объекта [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **macOSRestriction** для объекта [deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **whenPartnerDevicesWillBeRemovedDateTime** и **whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime** для объекта [deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta).|
|Изменение|Бета-версия|Изменен тип следующих свойств объекта [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta):<br/>**scriptContent** со String на Binary.<br/>|
|Изменение|Бета-версия|Добавлено свойство **smimeEnablePerMessageSwitch** для объекта [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **identityVersion** для объекта [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **faceIdBlocked** для объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **packageId** и **identityVersion** для объекта [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **azureADDeviceId** и **remoteAssistanceSessionErrorDetails** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **legacyAppConfiguration** для объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **identityVersion** для объекта [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **identityVersion** для объекта [managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **publishingState** для объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **installState** для объекта [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **identityVersion** для объекта [mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **allowPartnerToCollectIOSApplicationMetadata** для объекта [mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **members** для объекта [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **lastModifiedDateTime** для объекта [termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **deviceThreatProtectionEnabled** и **deviceThreatProtectionRequiredSecurityLevel** для объекта [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **minimumUpdateAutoInstallClassification** для объекта [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **privacyBlockPublishUserActivities** и **privacyBlockActivityFeed** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **configurationAccountType** для объекта [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **trustedNetworkDomains** для объекта [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **minimumUpdateAutoInstallClassification** для объекта [windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **identityVersion** для объекта [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **daysWithoutContactBeforeUnenroll** для объекта [windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **identityVersion** для объекта [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **identityVersion** для объекта [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **identityVersion** для объекта [windowsPhoneXAP](/graph/api/resources/intune-apps-windowsphonexap?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **identityVersion** для объекта [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **domainJoinConfiguration** для объекта [activeDirectoryWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **notificationMessageTemplate** для объекта [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **groupAssignments** для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **windowsInformationProtectionNetworkLearningSummaries** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **deviceConfigurationUserStateSummaries** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Изменен тип следующих свойств объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta):<br/>вместо **roleAssignments** из коллекции [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) теперь используется коллекция [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta).<br/>|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **smimeEncryptionCertificate** для объекта [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Изменен тип следующих свойств объекта [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta):<br/>вместо **smimeSigningCertificate** [iosCertificateProfileBase](/graph/api/resources/intune-deviceconfig-ioscertificateprofilebase?view=graph-rest-beta) теперь используется [iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-beta).<br/>|
|Изменение|Бета-версия|Удалено свойство навигации **vppToken** для объекта [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **groupAssignments** для объекта [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **groupAssignments** для объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалены свойства навигации **depOnboardingSettings** и **appleVolumePurchaseProgramTokens** для объекта [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **deviceEnrollmentConfigurations** для объекта [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta).|
|Изменение|Бета|Удалены свойства **windowsCommercialId** и **windowsCommercialIdLastModifiedTime** из сложного типа [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **showDisplayNameNextToLogo** для сложного типа [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **deviceUsageType** для сложного типа [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **supportsUserLicensing** и **supportsDeviceLicensing** для сложного типа [vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **actionMessage** для сложного типа [vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta).|

### <a name="reports-apis"></a>API отчетов
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | 1.0    | Добавлены следующие API:<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-1.0);<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-1.0);<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-1.0);<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-1.0);<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-1.0);<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-1.0). |

## <a name="december-2017"></a>Декабрь 2017 г.

### <a name="delta-query"></a>Разностный запрос

| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Изменение      | 1.0    | Добавлена возможность фильтрации [пользователей](/graph/api/user-delta?view=graph-rest-1.0) и [групп](/graph/api/group-delta?view=graph-rest-1.0). |

### <a name="microsoft-intune-apis"></a>API Microsoft Intune

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta);<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta);<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-beta);<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta).<br/>|
|Добавление|Бета|Добавлены новые сложные типы:<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-beta);<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-beta);<br/>[vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta);<br/>[windowsDeviceAADAccount](/graph/api/resources/intune-devices-windowsdeviceaadaccount?view=graph-rest-beta);<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-beta);<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-beta).<br/>|
|Добавление|Бета-версия|Добавлено действие [revokeTokens](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketokens?view=graph-rest-beta) для объекта [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие [createToken](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-createtoken?view=graph-rest-beta) для объекта [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие [updateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие [revokeLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta) для объекта [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлена функция [getDevicePasscode](/graph/api/intune-deviceconfig-devicecompliancepolicy-getdevicepasscode?view=graph-rest-beta) для коллекции [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлена функция [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-beta) для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**windowsStoreForBusinessApp**.<br/>|
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**windowsStoreForBusinessAppAssignmentSettings**.<br/>|
|Изменение|Бета-версия|Добавлено свойство **dateAndTimeBlockChanges** для объекта [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **enableAuthenticationViaCompanyPortal** объекта [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалены свойства **windowsStoreForBusinessLastSuccessfulSyncDateTime**, **isEnabledForWindowsStoreForBusiness**, **windowsStoreForBusinessLanguage** и **windowsStoreForBusinessLastCompletedApplicationSyncTime** для объекта [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **maximumDepTokens** и **intuneAccountId** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **enableAuthenticationViaCompanyPortal** для объекта [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **managedDeviceName** и **partnerReportedThreatState** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **installProgressDisplayLevel** для объекта [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **resourceScopes** для объекта [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **rolePermissions** и **isBuiltIn** для объекта [roleDefinition](/graph/api/resources/intune-rbac-roledefinition?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **tokenActionResults** для объекта [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **minimumUpdateAutoInstallClassification** для объекта [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **defenderSecurityCenterDisableAppBrowserUI**, **defenderSecurityCenterDisableFamilyUI**, **defenderSecurityCenterDisableHealthUI**, **defenderSecurityCenterDisableNetworkUI**, **defenderSecurityCenterDisableVirusUI**, **defenderSecurityCenterOrganizationDisplayName**, **defenderSecurityCenterHelpEmail**, **defenderSecurityCenterHelpPhone**, **defenderSecurityCenterHelpURL**, **defenderSecurityCenterNotificationsFromApp**, **defenderSecurityCenterITContactDisplay** и **applicationGuardAllowVirtualGPU** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **enableAutomaticRedeployment** и **authenticationAllowFIDODevice** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **trustedNetworkDomains** для объекта [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **minimumUpdateAutoInstallClassification** для объекта [windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **androidForWorkEnrollmentProfiles** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **healthAttestationSupportedStatus** для сложного типа [deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **tpmSpecificationVersion**, **operatingSystemEdition**, **deviceFullQualifiedDomainName**, **deviceGuardVirtualizationBasedSecurityHardwareRequirementState**, **deviceGuardVirtualizationBasedSecurityState** и **deviceGuardLocalSystemAuthorityCredentialGuardState** для сложного типа [hardwareInformation](/graph/api/resources/intune-devices-hardwareinformation?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **vpnConfigurationId** для сложного типа [iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **resourceActions** для сложного типа [rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-beta).|

### <a name="reports-apis"></a>API отчетов
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | 1.0    | Добавлены следующие API:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-1.0);<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-1.0);<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-1.0);<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-1.0);<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-1.0);<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-1.0);<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-1.0);<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0);<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-1.0);<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-1.0);<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-1.0);<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0);<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-1.0);<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0);<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-1.0);<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-1.0);<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0);<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0);<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-1.0);<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-1.0);<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-1.0);<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-1.0);<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-1.0);<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-1.0);<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-1.0);<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0);<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-1.0);<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-1.0);<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-1.0);<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-1.0);<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-1.0);<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-1.0);<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-1.0);<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0);<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-1.0);<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-1.0);<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-1.0);<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-1.0);<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-1.0);<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-1.0);<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-1.0);<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-1.0);<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-1.0);<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-1.0);<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-1.0);<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-1.0);<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-1.0);<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-1.0);<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-1.0);<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-1.0);<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-1.0);<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-1.0);<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-1.0);<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-1.0);<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-1.0);<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-1.0).|
| Дополнение    | Бета-версия    | Добавлены следующие API:<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-beta);<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-beta);<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-beta);<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-beta);<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-beta);<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-beta). |

## <a name="november-2017"></a>Ноябрь 2017 г.

### <a name="azure-ad-synchronization-apis"></a>API синхронизации Azure AD

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета-версия    | Добавлена поддержка синхронизации удостоверений Azure AD, в том числе следующих ресурсов:<br/>[задание](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta);<br/>[схема](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta);<br/>[шаблон](/graph/api/resources/synchronization-synchronizationtemplate?view=graph-rest-beta).<br/>Сведения о доступных методах см. в статьях об этих ресурсах.|

### <a name="education-apis"></a>API для образования

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета-версия|Добавлена поддержка сценариев для образования, в том числе следующих ресурсов:<br/>[учебные заведения](/graph/api/resources/educationschool?view=graph-rest-beta);<br/>[занятия](/graph/api/resources/educationclass?view=graph-rest-beta);<br/>[пользователи](/graph/api/resources/educationuser?view=graph-rest-beta);<br/>[назначения](/graph/api/resources/educationassignment?view=graph-rest-beta);<br/>[сданные работы](/graph/api/resources/educationsubmission?view=graph-rest-beta).<br/>Сведения о доступных методах см. в статьях об этих ресурсах.|

### <a name="microsoft-intune-apis"></a>API Microsoft Intune
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta);<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-beta);<br/>[deviceSetupConfiguration](/graph/api/resources/intune-deviceconfig-devicesetupconfiguration?view=graph-rest-beta);<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-beta);<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-beta);<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta);<br/>[ndesConnector](/graph/api/resources/intune-deviceconfig-ndesconnector?view=graph-rest-beta).<br/>|
|Добавление|Бета|Добавлены новые сложные типы:<br/>[auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta);<br/>[auditProperty](/graph/api/resources/intune-auditing-auditproperty?view=graph-rest-beta);<br/>[auditResource](/graph/api/resources/intune-auditing-auditresource?view=graph-rest-beta);<br/>[bulkManagedDeviceActionResult](/graph/api/resources/intune-devices-bulkmanageddeviceactionresult?view=graph-rest-beta);<br/>[deviceProtectionOverview](/graph/api/resources/intune-devices-deviceprotectionoverview?view=graph-rest-beta);<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-beta);<br/>[operatingSystemVersionRange](/graph/api/resources/intune-deviceconfig-operatingsystemversionrange?view=graph-rest-beta);<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-beta).<br/>|
|Добавление|Бета-версия|Добавлено действие executeAction для коллекции [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие [shutDown](/graph/api/intune-devices-manageddevice-shutdown?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-beta) для объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-beta) для объекта [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие setDefaultProfile для объекта [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие shareForSchoolDataSyncService для объекта [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлено действие unshareForSchoolDataSyncService для объекта [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлена функция getAuditCategories для коллекции [auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta). |
|Добавление|Бета-версия|Добавлена функция getAuditActivityTypes для коллекции [auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**mobileAppIdentifierDeployment**.<br/>|
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**windowsInformationProtectionCloudResource**;<br/>**windowsInformationProtectionCloudResourceCollection**.<br/>|
|Изменение|Бета-версия|Изменены следующие свойства объекта [androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta):<br/>свойство **passcode** сделано необязательным.<br/>|
|Изменение|Бета-версия|Добавлены свойства **microsoftStoreForBusinessLastSuccessfulSyncDateTime**, **isEnabledForMicrosoftStoreForBusiness**, **microsoftStoreForBusinessLanguage** и **microsoftStoreForBusinessLastCompletedApplicationSyncTime** для объекта [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **target** для объекта [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **deviceProtectionOverview** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **exchangeAlias** и **exchangeOrganization** для объекта [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **appStoreUrl** и **minimumSupportedOperatingSystem** для объекта [managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **remoteAssistanceSessionErrorString** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **appStoreUrl**, **applicableDeviceType** и **minimumSupportedOperatingSystem** для объекта [managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **notApplicableDeviceCount**, **pendingInstallDeviceCount**, **notApplicableUserCount** и **pendingInstallUserCount** для объекта [mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалены свойства **targetedSecurityGroupIds** и **targetedSecurityGroupsCount** объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалены свойства **targetedSecurityGroupsCount** и **targetedSecurityGroupIds** объекта [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **validOperatingSystemBuildRanges** для объекта [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **activeFirewallRequired**, **uacRequired** и **validOperatingSystemBuildRanges** для объекта [ windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **enableExpeditedTelemetryReporting** для объекта [windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалены свойства **allowedApps**, **enterpriseCloudResources** и **targetedSecurityGroupIds** объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **ignoreVersionDetection** для объекта [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **mobileAppIdentifierDeployments** объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **mobileAppIdentifierDeployments** объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **deviceConfiguration** объекта [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **deviceConfiguration** для объекта [deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства навигации **deviceSetupConfigurations**, **ndesConnectors**, **exchangeOnPremisesPolicies**, **conditionalAccessSettings**, **auditEvents** и **troubleshootingEvents** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **mobileAppIdentifierDeployments** объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство навигации **windowsProtectionState** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалены свойства навигации **mobileAppIdentifierDeployments** и **targetedSecurityGroups** объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **targetedSecurityGroups** объекта [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **deviceManagementTroubleshootingEvents** для объекта [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **allowedAppLockerFiles** объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **windowsProtectionState** объекта [windowsManagedDevice](/graph/api/resources/intune-devices-windowsmanageddevice?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **v11_0** для сложного типа [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **denied** для сложного типа [windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta).|

### <a name="reports-apis"></a>API отчетов
| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета-версия    | Добавлена поддержка JSON для следующих API:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta);<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta);<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta);<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta);<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta);<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta);<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta);<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta);<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta);<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta);<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta);<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta);<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta);<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta);<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta);<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta);<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta);<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta);<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta);<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta);<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta);<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta);<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta);<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta);<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta);<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta);<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta);<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta);<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta);<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta);<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta);<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta);<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta);<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta);<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta);<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta);<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta);<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-beta);<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-beta);<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-beta);<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-beta);<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-beta);<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-beta);<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-beta);<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-beta);<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-beta). |

### <a name="webhooks"></a>Веб-перехватчики

| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Критическое изменение | Бета-версия и версия 1.0 | Сокращен [максимальный период действия подписки](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type) с использованием [веб-перехватчиков](/graph/api/resources/webhooks?view=graph-rest-1.0) для элементов в корне диска. Новое значение — поддерживаемый максимальный срок действия для элементов в корне диска. |

## <a name="october-2017"></a>Октябрь 2017 г.

### <a name="azure-ad-apis"></a>API Azure AD

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
|Дополнение|Бета-версия|Добавлены объект [identityProvider](/graph/api/resources/identityprovider?view=graph-rest-beta) и операции [create](/graph/api/identityprovider-post-identityproviders?view=graph-rest-beta), [list](/graph/api/identityprovider-list?view=graph-rest-beta), [get](/graph/api/identityprovider-get?view=graph-rest-beta), [update](/graph/api/identityprovider-update?view=graph-rest-beta) и [delete](/graph/api/identityprovider-delete?view=graph-rest-beta).|


### <a name="microsoft-intune-apis"></a>API Microsoft Intune
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfigurationAssignment](/graph/api/resources/intune-apps-ioslobappprovisioningconfigurationassignment?view=graph-rest-beta)<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-beta)<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-beta)<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-beta)<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-beta)<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-beta)<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta)<br/>[windows10PFXImportCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pfximportcertificateprofile?view=graph-rest-beta)<br/>[windowsAssignedAccessProfile](/graph/api/resources/intune-deviceconfig-windowsassignedaccessprofile?view=graph-rest-beta)<br/>[windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-beta)<br/>[iosSingleSignOnSettings](/graph/api/resources/intune-deviceconfig-iossinglesignonsettings?view=graph-rest-beta)<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-beta)<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta)<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-beta)<br/>[proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta)<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-beta)<br/>[windowsStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-windowsstoreforbusinessappassignmentsettings?view=graph-rest-beta)<br/>|
|Дополнение|Бета-версия|Добавлено действие [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-beta) для объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) к объекту [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) для объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-beta) для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [assignedAccessMultiModeProfiles](/graph/api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles?view=graph-rest-beta) для объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [syncLicenses](/graph/api/intune-onboarding-vpptoken-synclicenses?view=graph-rest-beta) для объекта [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [targetApps](/graph/api/intune-mam-managedapppolicy-targetapps?view=graph-rest-beta) для объекта [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [targetApps](/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-beta) для объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [targetApps](/graph/api/intune-mam-targetedmanagedappconfiguration-targetapps?view=graph-rest-beta) для объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено действие [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) для объекта [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**cloudPkiSubscription**<br/>|
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**cloudPkiAdministratorCredentials**<br/>**windowsNetworkIsolationCloudResource**<br/>**windowsNetworkIsolationCloudResourceCollection**<br/>**windowsNetworkIsolationIPRangeCollection**<br/>**windowsNetworkIsolationResourceCollection**<br/>|
|Изменение|Бета-версия|Добавлено свойство **gracePeriodInMinutes** для объекта [androidDeviceComplianceLocalActionBase](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionbase?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **enableSplitTunneling** объекта [androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **versionName** и **versionCode** для объекта [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **minimumRequiredPatchVersion** и **minimumWarningPatchVersion** для объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **minimumRequiredPatchVersion** и **minimumWarningPatchVersion** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **target** для объекта [deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **singleSignOnSettings** для объекта [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **versionNumber** и **buildNumber** для объекта [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **bundleId** для объекта [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **preSharedKey** для объекта [iosWiFiConfiguration](/graph/api/resources/intune-deviceconfig-ioswificonfiguration?view=graph-rest-beta).|
|Изменение|бета|Добавлены свойства **versionName** и **versionCode** для объекта [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **periodBeforePinReset** для объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **subscriberCarrier**, **meid**, **totalStorageSpaceInBytes** и **freeStorageSpaceInBytes** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **enrollmentType** объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **versionNumber** и **buildNumber** для объекта [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **displayVersion** для объекта [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалены свойства **defaultDeviceEnrollmentRestrictions**, **defaultDeviceEnrollmentWindowsHelloForBusinessSettings** и **defaultDeviceEnrollmentLimit** объекта [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **isAssigned** для объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **isAssigned** для объекта [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **activeFirewallRequired**, **uacRequired**, **defenderEnabled**, **defenderVersion**, **signatureOutOfDate** и **rtpEnabled** объекта [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **assignedAccessSingleModeUserName**, **assignedAccessSingleModeAppUserModelId**, **microsoftAccountSignInAssistantSettings**, **authenticationAllowSecondaryDevice**, **cryptographyAllowFipsAlgorithmPolicy**, **securityBlockAzureADJoinedDevicesAutoEncryption**, **systemTelemetryProxyServer**, **inkWorkspaceAccess**, **inkWorkspaceBlockSuggestedApps**, **defenderCloudBlockLevel** и **defenderCloudExtendedTimeout** объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **protectedApps**, **enterpriseProxiedDomains** и **isAssigned** для объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **productVersion** для объекта [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **apps** для объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta).|
|Изменение|бета|Добавлено свойство навигации **apps** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **vppTokens** для объекта [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **deviceCompliancePolicy** объекта [deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **deviceCompliancePolicy** для объекта [deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **identityCertificateForClientAuthentication** для объекта [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **apps** для объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **apps** для объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignedAccessMultiModeProfiles** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **protectedAppLockerFiles** для объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **port** и **forceTls** для сложного типа [airPrintDestination](/graph/api/resources/intune-deviceconfig-airprintdestination?view=graph-rest-beta).|
|Изменение|Бета-версия|Изменен тип следующих свойств сложного типа [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta):<br/>вместо Int32 **errorCode** теперь используется Int64.<br/>|
|Изменение|Бета-версия|Изменен тип следующих свойств сложного типа [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta):<br/>вместо Int32 **errorCode** теперь используется Int64.<br/>|
|Изменение|Бета-версия|Изменен тип следующих свойств сложного типа [windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta):<br/>вместо **enterpriseCloudResources** [windowsNetworkIsolationCloudResourceCollection](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationcloudresourcecollection?view=graph-rest-beta) теперь используется коллекция [proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta);<br/>вместо **enterpriseInternalProxyServers** windowsNetworkIsolationResourceCollection теперь используется коллекция строк;<br/>**enterpriseIPRanges** windowsNetworkIsolationIPRangeCollection теперь используется коллекция [ipRange](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta);<br/>вместо **enterpriseNetworkDomainNames** windowsNetworkIsolationResourceCollection теперь используется коллекция строк;<br/>вместо **enterpriseProxyServers** windowsNetworkIsolationResourceCollection теперь используется коллекция строк;<br/>вместо **neutralDomainResources** windowsNetworkIsolationResourceCollection теперь используется коллекция строк.<br/>|

### <a name="microsoft-teams-apis"></a>API Microsoft Teams

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета-версия|Добавлен новый объект [team](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены операции [create](/graph/api/team-put-teams?view=graph-rest-beta), [get](/graph/api/team-get?view=graph-rest-beta) и [update](/graph/api/team-update?view=graph-rest-beta) для объекта [team](/graph/api/resources/team?view=graph-rest-beta).|

### <a name="outlook-messages"></a>Сообщения Outlook

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Это улучшение поведения связано с получением общей почтовой папки или содержимого сообщений в ней, если кто-то предоставил вошедшему пользователю доступ к почтовой папке или делегировал ему почтовый ящик пользователя. В таких случаях приложение может указать ИД пользователя или имя участника-пользователя, чтобы [получить эту общую почтовую папку](/graph/api/mailfolder-get?view=graph-rest-1.0) или [получить сообщения из этого общего календаря](/graph/api/user-list-messages?view=graph-rest-1.0), при условии что вошедший пользователь предоставил приложению делегированные разрешения. |


### <a name="outlook-user-choices"></a>Настройки пользователей Outlook

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
|Дополнение | Бета-версия | Добавлено новое свойство **workingHours** для объекта [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta). Сведения о поддерживаемых вариантах использования см. в описании [типа ресурса workingHours](/graph/api/resources/workinghours?view=graph-rest-beta).|
|Дополнение | Бета-версия | Добавлены следующие сложные типы: <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-beta) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-beta) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-beta) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-beta) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-beta)|


### <a name="reports-apis"></a>API отчетов
| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Изменение      | Бета-версия    | Добавлены API [getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta), [getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta) и [getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta). Они заменили API EmailActivity. |
| Изменение      | Бета-версия    | Добавлены API [getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta), [getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta), [getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta) и [getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta). Они заменили API EmailAppUsage. |
| Изменение      | Бета-версия    | Добавлены API [getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta), [getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta), [getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta) и [getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta). Они заменили API MailboxUsage. |
| Изменение      | Бета-версия    | Добавлены API [getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta), [getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta) и [getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta). Они заменили API Office365Activations. |
| Изменение      | Бета-версия    | Добавлены API [getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta), [getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta) и [getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta). Они заменили API Office365ActiveUser. |
| Изменение      | Бета-версия    | Добавлены API [getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta), [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta), [getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta), [getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta) и [getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta). Они заменили API Office365GroupsActivity. |
| Изменение      | Бета-версия    | Добавлены API [getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta), [getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta) и [getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta). Они заменили API OneDriveActivity. |
| Изменение      | Бета-версия    | Добавлены API [getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta), [getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta), [getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta) и [getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta). Они заменили API OneDriveUsage. |
| Изменение      | Бета-версия    | Добавлены API [getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta), [getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta), [getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta) и [getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta). Они заменили API SharePointActivity. |
| Изменение      | Бета-версия    | Добавлены API [getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta), [getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta), [getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta), [getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta) и [getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta). Они заменили API SharePointSiteUsage. |
| Изменение      | Бета-версия    | Добавлены API [getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta), [getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta) и [getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta). Они заменили API SfbActivity. |
| Изменение      | Бета-версия    | Добавлены API [getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta), [getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta) и [getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta). Они заменили API SfbDeviceUsage. |
| Изменение      | Бета-версия    | Добавлены API [getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta), [getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta) и [getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta). Они заменили API SfbOrganizerActivity. |
| Изменение      | Бета-версия    | Добавлены API [getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta), [getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta) и [getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta). Они заменили API SfbParticipantActivity. |
| Изменение      | Бета-версия    | Добавлены API [getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta), [getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta) и [getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta). Они заменили API SfbP2PActivity. |
| Изменение      | Бета-версия    | Добавлены API [getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-beta), [getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-beta) и [getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-beta). Они заменили API YammerActivity. |
| Изменение      | Бета-версия    | Добавлены API [getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-beta), [getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-beta) и [getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-beta). Они заменили API YammerDeviceUsage. |
| Изменение      | Бета-версия    | Добавлены API [getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-beta), [getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-beta) и [getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-beta). Они заменили API YammerGroupsActivity. |



## <a name="september-2017"></a>Сентябрь 2017 г.

### <a name="intune-apis"></a>API Intune

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета    | Добавлены новые объекты:<br/>[activeDirectoryWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[azureADWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-beta)<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta)<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-beta)<br/>[windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta)<br/>[windows10NetworkBoundaryConfiguration](/graph/api/resources/intune-deviceconfig-windows10networkboundaryconfiguration?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta)<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta)<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-beta)<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-beta)<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-beta)<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta)<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-beta)<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-beta)<br/>[outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-beta)<br/>windowsNetworkIsolationCloudResource<br/>windowsNetworkIsolationCloudResourceCollection<br/>windowsNetworkIsolationIPRangeCollection<br/>[windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta)<br/>windowsNetworkIsolationResourceCollection<br/> |
| Дополнение    | Бета    | Добавлено действие [sync](/graph/api/intune-enrollment-windowsautopilotsettings-sync?view=graph-rest-beta) для объекта [windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие [assign](/graph/api/intune-enrollment-windowsautopilotdeploymentprofile-assign?view=graph-rest-beta) для объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие localActions для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие [setPriority](/graph/api/intune-onboarding-deviceenrollmentconfiguration-setpriority?view=graph-rest-beta) для объекта [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие [assign](/graph/api/intune-onboarding-deviceenrollmentconfiguration-assign?view=graph-rest-beta) для объекта [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие uploadDepToken для коллекции [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие syncWithAppleDeviceEnrollmentProgram для коллекции [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие updateMobileAppIdentifierDeployments для объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие assign для объекта [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие assign для объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие assign для объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлена функция getEncryptionPublicKey для коллекции [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders**, **requireCompanyPortalAppIntegrity** и **conditionStatementId** для объекта [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **requireAppVerify**, **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders** и **requireCompanyPortalAppIntegrity** для объекта [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **blockCrossProfileCopyPaste** и **requireAppVerify** для объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **kioskModeApps** и **requireAppVerify** для объекта [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **kioskModeManagedApps** объекта [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **cloudPkiProvider**, **createdDateTime**, **description**, **lastModifiedDateTime**, **displayName**, **syncStatus**, **lastSyncError**, **lastSyncDateTime**, **credentials**, **trustedRootCertificate** и **version** объекта cloudPkiSubscription. |
| Изменение      | Бета-версия    | Удалены свойства **assignmentStatus**, **assignmentProgress** и **assignmentErrorMessage** объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **adminConsent** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **vppTokenOrganizationName**, **vppTokenAccountType** и **vppTokenAppleId** для объекта [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **deviceEnrollmentType**, **wiFiMacAddress** и **deviceHealthAttestationState** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **legacyAppConfiguration** для объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **notApplicableCount** для объекта [managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **notApplicableCount** для объекта [managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **firewallBlockStatefulFTP**, **firewallIdleTimeoutForSecurityAssociationInSeconds**, **firewallPreSharedKeyEncodingMethod**, **firewallIPSecExemptionsAllowNeighborDiscovery**, **firewallIPSecExemptionsAllowICMP**, **firewallIPSecExemptionsAllowRouterDiscovery**, **firewallIPSecExemptionsAllowDHCP**, **firewallCertificateRevocationListCheckMethod**, **firewallMergeKeyingModuleSettings**, **firewallPacketQueueingMethod**, **firewallProfileDomain**, **firewallProfilePublic**, **firewallProfilePrivate**, **defenderAttackSurfaceReductionExcludedPaths**, **defenderOfficeAppsOtherProcessInjectionType**, **defenderOfficeAppsExecutableContentCreationOrLaunchType**, **defenderOfficeAppsLaunchChildProcessType**, **defenderOfficeMacroCodeAllowWin32ImportsType**, **defenderScriptObfuscatedMacroCodeType**, **defenderScriptDownloadedPayloadExecutionType**, **defenderEmailContentExecutionType**, **defenderGuardMyFoldersType**, **defenderGuardedFoldersAllowedAppPaths**, **defenderAdditionalGuardedFolders**, **defenderNetworkProtectionType**, **defenderExploitProtectionXml**, **defenderExploitProtectionXmlFileName**, **defenderSecurityCenterBlockExploitProtectionOverride**, **appLockerApplicationControl**, **applicationGuardBlockClipboardSharing**, **applicationGuardAllowPrintToPDF**, **applicationGuardAllowPrintToXPS**, **applicationGuardAllowPrintToLocalPrinters**, **applicationGuardAllowPrintToNetworkPrinters** и **bitLockerDisableWarningForOtherDiskEncryption** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **displayAppListWithGdiDPIScalingTurnedOn**, **displayAppListWithGdiDPIScalingTurnedOff**, **messagingBlockSync**, **messagingBlockMMS** и **messagingBlockRichCommunicationServices** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **bluetoothDeviceName** объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Удалены свойства **deviceAccountBlockExchangeServices**, **deviceAccountEmailAddress**, **deviceAccountExchangeServerAddress**, **deviceAccountRequirePasswordRotation** и **deviceAccountSessionInitiationProtocolAddress** объекта [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **localActions** для объекта [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства навигации **windowsAutopilotSettings**, **windowsAutopilotDeviceIdentities**, **windowsAutopilotDeploymentProfiles**, **deviceEnrollmentConfigurations**, **deviceManagementPartners** и **depOnboardingSettings** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство навигации **cloudPkiSubscriptions** объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **assignments** для объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **assignments** для объекта [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **assignments** для объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta). |

### <a name="onedrive"></a>OneDrive

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлено свойство **system** для ресурса [Drive][]. |
| Дополнение        | 1.0        | Добавлена связь **list** для ресурса [Drive][]. |
| Дополнение        | 1.0        | Добавлена связь **listItem** для ресурса [DriveItem][]. |
| Дополнение        | 1.0        | Добавлены связи **list** и **listItem** для ресурса [SharedDriveItem][]. |
| Дополнение        | 1.0        | Добавлены новые сложные типы: [FolderView][]  |
| Дополнение        | 1.0        | Добавлено свойство **view** для сложного типа [Folder][]. |
| Дополнение        | 1.0        | Добавлено свойство **driveType** для сложного типа [ItemReference][]. |
| Дополнение        | 1.0        | Добавлены свойства **audioBitsPerSample**, **audioChannels**, **audioFormat**, **audioSamplesPerSecond**, **fourCC** и **frameRate** для сложного типа [Video][]. |
| Дополнение        | Бета        | Добавлено свойство **system** для ресурса [Drive][Drive-beta]. |
| Дополнение        | Бета        | Добавлена связь **activities** для ресурса [Drive][Drive-beta]. |
| Дополнение        | Бета        | Добавлено свойство **publication** для ресурса [DriveItem][DriveItem-beta]. |
| Дополнение        | Бета        | Добавлены связи **activities** и **versions** для ресурса [DriveItem][DriveItem-beta]. |
| Дополнение        | Бета        | Добавлены новые объекты: [DriveItemVersion][DriveItemVersion-beta], [ItemActivity][ItemActivity-beta]. |
| Дополнение        | Бета        | Добавлены новые сложные типы: [CommentAction][CommentAction-beta], [CreateAction][CreateAction-beta], [DeleteAction][DeleteAction-beta], [EditAction][EditAction-beta], [ItemActionSet][ItemActionSet-beta], [ItemActivityTimeSet][ItemActivityTimeSet-beta], [MentionAction][MentionAction-beta], [MoveAction][MoveAction-beta], [PublicationFacet][PublicationFacet-beta], [RenameAction][RenameAction-beta], [RestoreAction][RestoreAction-beta], [ShareAction][ShareAction-beta] и [VersionAction][VersionAction-beta]. |
| Дополнение        | Бета        | Добавлено свойство **driveType** для сложного типа [ItemReference][ItemReference-beta]. |
| Удаление        | Бета        | Удалено свойство **tenantId** сложного типа [SharepointIds][SharepointIds-beta]. |
| Дополнение        | 1.0        | Добавлены свойства **audioBitsPerSample**, **audioChannels**, **audioFormat**, **audioSamplesPerSecond**, **fourCC** и **frameRate** для сложного типа [Video][Video-beta]. |
| Дополнение        | Бета        | Добавлены действия [CheckIn][CheckIn-beta] и [CheckOut][CheckOut-beta] для ресурса [DriveItem][DriveItem-beta]. |
| Дополнение        | Бета        | Добавлены свойства **expirationDateTime**, **password**, **message** и **recipients** для действия [CreateLink][CreateLink-beta] ресурса [DriveItem][DriveItem-beta]. |

[Drive]: /graph/api/resources/drive?view=graph-rest-1.0
[DriveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[SharedDriveItem]: /graph/api/resources/shareddriveitem?view=graph-rest-1.0
[FolderView]: /graph/api/resources/folderview?view=graph-rest-1.0
[Folder]: /graph/api/resources/folder?view=graph-rest-1.0
[ItemReference]: /graph/api/resources/itemreference?view=graph-rest-1.0
[Video]: /graph/api/resources/video?view=graph-rest-1.0
[Drive-beta]: /graph/api/resources/drive?view=graph-rest-beta
[DriveItem-beta]: /graph/api/resources/driveitem?view=graph-rest-beta
[DriveItemVersion-beta]: /graph/api/resources/driveitemversion?view=graph-rest-beta
[ItemActivity-beta]: /graph/api/resources/itemactivity?view=graph-rest-beta
[CommentAction-beta]: /graph/api/resources/commentaction?view=graph-rest-beta
[CreateAction-beta]: /graph/api/resources/createaction?view=graph-rest-beta
[DeleteAction-beta]: /graph/api/resources/deleteaction?view=graph-rest-beta
[EditAction-beta]: /graph/api/resources/editaction?view=graph-rest-beta
[ItemActionSet-beta]: /graph/api/resources/itemactionset?view=graph-rest-beta
[ItemActivityTimeSet-beta]: /graph/api/resources/itemactivitytimeset?view=graph-rest-beta
[MentionAction-beta]: /graph/api/resources/mentionaction?view=graph-rest-beta
[MoveAction-beta]: /graph/api/resources/moveaction?view=graph-rest-beta
[PublicationFacet-beta]: /graph/api/resources/publicationfacet?view=graph-rest-beta
[RenameAction-beta]: /graph/api/resources/renameaction?view=graph-rest-beta
[RestoreAction-beta]: /graph/api/resources/restoreaction?view=graph-rest-beta
[ShareAction-beta]: /graph/api/resources/shareaction?view=graph-rest-beta
[VersionAction-beta]: /graph/api/resources/versionaction?view=graph-rest-beta
[ItemReference-beta]: /graph/api/resources/itemreference?view=graph-rest-beta
[SharepointIds-beta]: /graph/api/resources/sharepointids?view=graph-rest-beta
[Video-beta]: /graph/api/resources/video?view=graph-rest-beta
[CheckIn-beta]: /graph/api/driveitem-checkin?view=graph-rest-beta
[CheckOut-beta]: /graph/api/driveitem-checkout?view=graph-rest-beta
[CreateLink-beta]: /graph/api/driveitem-createlink?view=graph-rest-beta


### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | Бета          | Добавлены функции [findRoomLists](/graph/api/user-findroomlists?view=graph-rest-beta) и [findRooms](/graph/api/user-findrooms?view=graph-rest-beta) для объекта [user](/graph/api/resources/user?view=graph-rest-beta). |
| Дополнение        | Бета          | Добавлено свойство **locations** для объекта [event](/graph/api/resources/event?view=graph-rest-beta), позволяющее организовать событие, в котором могут участвовать пользователи из нескольких расположений. |
| Дополнение        | Бета          | Добавлено свойство **locationType** для сложного типа [location](/graph/api/resources/location?view=graph-rest-beta). |
| Дополнение        | Бета          | Добавлены свойства **uniqueId** и **uniqueIdType** для сложного типа [location](/graph/api/resources/location?view=graph-rest-beta). В настоящее время эти свойства предназначены только для внутреннего использования. |
| Изменение          | 1.0 и бета-версия | Это улучшение поведения связано с получением общего календаря или содержимого событий в нем, если кто-то предоставил вошедшему пользователю доступ к календарю или делегировал ему почтовый ящик пользователя. В таких случаях приложение может указать ИД пользователя или имя участника-пользователя, чтобы [получить этот общий календарь](/graph/api/calendar-get?view=graph-rest-1.0) или [получить события из этого общего календаря](/graph/api/user-list-events?view=graph-rest-1.0), при условии что вошедший пользователь предоставил приложению делегированные разрешения. |

### <a name="outlook-contacts"></a>Контакты Outlook

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Это улучшение поведения связано с получением общей папки контактов или содержимого контактов в ней, если кто-то предоставил вошедшему пользователю доступ к папке контактов или делегировал ему почтовый ящик пользователя. В таких случаях приложение может указать ИД пользователя или имя участника-пользователя, чтобы [получить эту общую папку контактов](/graph/api/contactfolder-get?view=graph-rest-1.0) или [получить контакты из этой общей папки](/graph/api/user-list-contacts?view=graph-rest-1.0), при условии что вошедший пользователь предоставил приложению делегированные разрешения. |

### <a name="outlook-mail"></a>Почта Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлено свойство **internetMessageHeaders** для объекта [message](/graph/api/resources/message?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлен сложный тип [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлено свойство навигации **messageRules** для объекта [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta). **messageRules** — это набор экземпляров [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлены объект [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta) и сложные типы [messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-beta), [messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-beta) и [sizeRange](/graph/api/resources/sizerange?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлены следующие операции CRUD для правил обработки сообщений: [create](/graph/api/mailfolder-post-messagerules?view=graph-rest-beta), [list](/graph/api/mailfolder-list-messagerules?view=graph-rest-beta), [get](/graph/api/messagerule-get?view=graph-rest-beta), [update](/graph/api/messagerule-update?view=graph-rest-beta) и [delete](/graph/api/messagerule-delete?view=graph-rest-beta). |


### <a name="outlook-user-choices"></a>Настройки пользователей Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлено новое свойство навигации **masterCategories** для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta). **masterCategories** — это коллекция объектов [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлен объект [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлены следующие операции CRUD для объекта [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta): [создание](/graph/api/outlookuser-post-mastercategories?view=graph-rest-beta), [получение](/graph/api/outlookcategory-get?view=graph-rest-beta), [обновление](/graph/api/outlookcategory-update?view=graph-rest-beta) и [удаление](/graph/api/outlookcategory-delete?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлена новая функция [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-beta) для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлена новая функция [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-beta) для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta). |


### <a name="sharepoint-lists"></a>Списки SharePoint

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлены новые объекты: [ColumnDefinition][], [ColumnLink][], [ContentType][], [List][], [ListItem][]. |
| Дополнение        | 1.0        | Добавлены связи **columns**, **contentTypes**, **items** и **lists** для ресурса [Site][]. |
| Дополнение        | 1.0        | Добавлены новые сложные типы: [BooleanColumn][], [CalculatedColumn][], [ChoiceColumn][], [ContentTypeInfo][], [ContentTypeOrder][], [CurrencyColumn][], [DateTimeColumn][], [DefaultColumnValue][], [ListInfo][], [LookupColumn][], [NumberColumn][], [PersonOrGroupColumn][], [SystemFacet][], [TextColumn][]. |
| Дополнение        | Бета        | Добавлены новые объекты: [BaseItemVersion][BaseItemVersion-beta], [ColumnLink][ColumnLink-beta], [ContentType][ContentType-beta], [ListItemVersion][ListItemVersion-beta]. |
| Дополнение        | Бета        | Добавлены свойства **columnGroup**, **currency**, **defaultValue** и **displayName** для объекта [ColumnDefinition][ColumnDefinition-beta]. |
| Дополнение        | Бета        | Добавлены свойства **displayName** и **system** для ресурса [List][List-beta]. |
| Дополнение        | Бета        | Добавлены связи **activities** и **contentTypes** для ресурса [List][List-beta]. |
| Дополнение        | Бета        | Добавлено свойство **contentType** для ресурса [ListItem][ListItem-beta]. |
| Дополнение        | Бета        | Добавлены связи **activities** и **versions** для ресурса [ListItem][ListItem-beta]. |
| Дополнение        | Бета        | Добавлена связь **contentTypes** для ресурса [Site][Site-beta]. |
| Дополнение        | Бета        | Добавлено свойство **outputType** для типа [BooleanColumn][BooleanColumn-beta]. |
| Дополнение        | бета        | Добавлены новые сложные типы: [ContentTypeInfo][ContentTypeInfo-beta], [ContentTypeOrder][ContentTypeOrder-beta], [CurrencyColumn][CurrencyColumn-beta] и [SystemFacet][SystemFacet-beta]. |
| Дополнение        | Бета        | Добавлено свойство **contentTypesEnabled** для сложного типа [ListInfo][ListInfo-beta]. |
| Дополнение        | Бета        | Добавлено свойство **allowUnlimitedLength** для сложного типа [LookupColumn][LookupColumn-beta]. |
| Изменение          | Бета        | Имя свойства **allowMultipleValue** изменено на **allowMultipleValues** для сложного типа [LookupColumn][LookupColumn-beta]. |
| Изменение          | Бета        | Имя свойства **chooseFrom** изменено на **chooseFromType** для сложного типа [PersonOrGroupColumn][PersonOrGroupColumn-beta]. |
| Удаление        | Бета        | Удалено свойство **locale** сложного типа [NumberColumn][NumberColumn-beta]. |
| Удаление        | Бета        | Удалено свойство **enforceUniqueValues** сложного типа [PersonOrGroupColumn][PersonOrGroupColumn-beta]. |

[BaseItemVersion-beta]: /graph/api/resources/baseitemversion?view=graph-rest-beta
[BooleanColumn-beta]:  /graph/api/resources/booleanColumn?view=graph-rest-beta
[BooleanColumn]: /graph/api/resources/booleancolumn?view=graph-rest-1.0
[CalculatedColumn]: /graph/api/resources/calculatedcolumn?view=graph-rest-1.0
[ChoiceColumn]: /graph/api/resources/choicecolumn?view=graph-rest-1.0
[ColumnDefinition-beta]: /graph/api/resources/columndefinition?view=graph-rest-beta
[ColumnDefinition]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[ColumnLink-beta]: /graph/api/resources/columnlink?view=graph-rest-beta
[ColumnLink]: /graph/api/resources/columnlink?view=graph-rest-1.0
[ContentType-beta]: /graph/api/resources/contenttype?view=graph-rest-beta
[ContentType]: /graph/api/resources/contenttype?view=graph-rest-1.0
[ContentTypeInfo-beta]: /graph/api/resources/contenttypeinfo?view=graph-rest-beta
[ContentTypeInfo]: /graph/api/resources/contenttypeinfo?view=graph-rest-1.0
[ContentTypeOrder-beta]: /graph/api/resources/contenttypeorder?view=graph-rest-beta
[ContentTypeOrder]: /graph/api/resources/contenttypeorder?view=graph-rest-1.0
[CurrencyColumn-beta]: /graph/api/resources/currencycolumn?view=graph-rest-beta
[CurrencyColumn]: /graph/api/resources/currencycolumn?view=graph-rest-1.0
[DateTimeColumn]: /graph/api/resources/datetimecolumn?view=graph-rest-1.0
[DefaultColumnValue]: /graph/api/resources/defaultcolumnvalue?view=graph-rest-1.0
[List-beta]: /graph/api/resources/list?view=graph-rest-beta
[List]: /graph/api/resources/list?view=graph-rest-1.0
[ListInfo-beta]: /graph/api/resources/listinfo?view=graph-rest-beta
[ListInfo]: /graph/api/resources/listinfo?view=graph-rest-1.0
[ListItem-beta]: /graph/api/resources/listitem?view=graph-rest-beta
[ListItem]: /graph/api/resources/listitem?view=graph-rest-1.0
[ListItemVersion-beta]: /graph/api/resources/listitemversion?view=graph-rest-beta
[LookupColumn-beta]: /graph/api/resources/lookupcolumn?view=graph-rest-beta
[LookupColumn]: /graph/api/resources/lookupcolumn?view=graph-rest-1.0
[NumberColumn-beta]: /graph/api/resources/numbercolumn?view=graph-rest-beta
[NumberColumn]: /graph/api/resources/numbercolumn?view=graph-rest-1.0
[PersonOrGroupColumn-beta]: /graph/api/resources/personorgroupcolumn?view=graph-rest-beta
[PersonOrGroupColumn]: /graph/api/resources/personorgroupcolumn?view=graph-rest-1.0
[Site-beta]: /graph/api/resources/site?view=graph-rest-beta
[Site]: /graph/api/resources/site?view=graph-rest-1.0
[SystemFacet-beta]: /graph/api/resources/systemfacet?view=graph-rest-beta
[SystemFacet]: /graph/api/resources/systemfacet?view=graph-rest-1.0
[TextColumn]: /graph/api/resources/textcolumn?view=graph-rest-1.0


### <a name="sharepoint-sites"></a>Сайты SharePoint

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлены свойства **dataLocationCode** и **root** для сложного типа [SiteCollection][SiteCollection-beta]. |

[SiteCollection-beta]: /graph/api/resources/sitecollection?view=graph-rest-beta


## <a name="august-2017"></a>Август 2017 г.

### <a name="group-lifecycle-policy"></a>Политика жизненного цикла группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена сущность [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлены следующие API для политики жизненного цикла группы, а именно для: [создания](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-beta), [перечисления](/graph/api/grouplifecyclepolicy-list?view=graph-rest-beta), [получения](/graph/api/grouplifecyclepolicy-get?view=graph-rest-beta), [обновления](/graph/api/grouplifecyclepolicy-update?view=graph-rest-beta), [удаления](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-beta), [добавления группы](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-beta), [удаления группы](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-beta) и [возобновления группы](/graph/api/grouplifecyclepolicy-renewgroup?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлена функция [List groupLifecylePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-beta) для объекта [group](/graph/api/resources/group?view=graph-rest-beta). |

### <a name="intune-apis"></a>API Intune
| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета-версия    | Добавлен новый объект:<br/>[windowsPrivacyDataAccessControlItem](/graph/api/resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem?view=graph-rest-beta)<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-beta)<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-beta)<br/> |
| Дополнение    | Бета-версия    | Добавлено действие [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-beta) для [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Дополнение    | Бета-версия    | Добавлено действие [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-beta) для [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Дополнение    | Бета-версия    | Добавлено действие [windowsPrivacyAccessControls](/graph/api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols?view=graph-rest-beta) для [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлены свойства **automaticallyUpdateApps** и **countryOrRegion** для объекта [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлено свойство **enableAuthenticationViaCompanyPortal** для объекта [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлено свойство **notificationMessageCCList** для объекта [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлено свойство **notApplicableCount** для объекта [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлено свойство **notApplicableCount** для объекта [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлено свойство **notApplicableCount** для объекта [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлено свойство **notApplicableCount** для объекта [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлено свойство **configurationManagerClientEnabledFeatures** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Удалено свойство **intuneBrand** для объекта [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлены свойства **smartScreenEnableInShell**, **smartScreenBlockOverrideForFiles**, **applicationGuardEnabled**, **applicationGuardBlockFileTransfer**, **applicationGuardBlockNonEnterpriseContent**, **applicationGuardAllowPersistence** и **applicationGuardForceAuditing** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлены свойства **searchBlockDiacritics**, **searchDisableAutoLanguageDetection**, **searchDisableIndexingEncryptedItems**, **searchEnableRemoteQueries**, **searchDisableUseLocation**, **searchDisableIndexerBackoff**, **searchDisableIndexingRemovableDrive**, **searchEnableAutomaticIndexSizeManangement**, **smartScreenEnableAppInstallControl** и **privacyAdvertisingId** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Удалено свойство **settingsDeviceName** для объекта [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Удалено свойство **restartMode** для объекта [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлены свойства навигации **detectedApps** и **managedDevices** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлено свойство навигации **privacyAccessControls** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлено свойство **secureByDefault** для сложного типа [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлено свойство **restartMode** для сложного типа [windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta) |

### <a name="onenote"></a>OneNote

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлено свойство навигации [onenote](/graph/api/resources/onenote?view=graph-rest-1.0) для **site**. |
| Дополнение        | Бета          | Добавлены целевые параметры *siteCollectionId* и *siteId* для операций копирования. Пример: [CopyNotebook](/graph/api/notebook-copynotebook?view=graph-rest-1.0). |

### <a name="people"></a>Люди

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | В версию 1.0 добавлены интерфейсы [People API](/graph/api/resources/person?view=graph-rest-1.0). Подробные сведения об этих API см. в статье, посвященной [получению релевантной информации о людях](people-example.md). |
| Добавление        | 1.0        | Добавлено разрешение People.Read.All. Дополнительные сведения см. в [справочнике по разрешениям](permissions-reference.md). |
| Добавление        | 1.0        | Добавлен ресурс [personType](/graph/api/resources/persontype?view=graph-rest-1.0). |
| Изменение          | 1.0        | Ресурс [scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0) заменил ресурс **rankedEmailAddress**. |
| Изменение          | 1.0        | Ресурс [person](/graph/api/resources/person?view=graph-rest-1.0) был обновлен следующим образом:<ul><li>Свойство **scoredEmailAddresses** (коллекция типа [scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0)) заменило свойство **emailAddresses**.</li><li>Свойство **jobTitle** заменило свойство **title**.</li><li>Удалены свойства **sources** и **mailboxType**.</li><li>Свойство **personType** теперь имеет тип [personType](/graph/api/resources/persontype?view=graph-rest-1.0), а не строковый, и заменяет существовавшие ранее свойства **sources** и **mailboxType**.</li><li>Добавлено свойство **imAddress**.</li></ul> |
| Удаление        | 1.0        | Удален ресурс **personDataSource**. |

### <a name="user"></a>User

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство **employeeId** для [user](/graph/api/resources/user?view=graph-rest-beta). |

## <a name="july-2017"></a>Июль 2017 г.

### <a name="group-settings"></a>Параметры группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлена поддержка параметров группы.<br/>Новые типы ресурсов: [groupSetting](/graph/api/resources/groupsetting?view=graph-rest-1.0), [groupSettingTemplate](/graph/api/resources/groupsettingtemplate?view=graph-rest-1.0), [settingValue](/graph/api/resources/settingvalue?view=graph-rest-1.0) и [settingTemplateValue](/graph/api/resources/settingtemplatevalue?view=graph-rest-1.0). |
| Изменение          | 1.0        | Добавлено свойство **classification** и свойство навигации **settings** для [group](/graph/api/resources/group?view=graph-rest-1.0). |

### <a name="intune-apis"></a>API Intune

| Тип&nbsp;изменения | Версия | Описание                              |
| :--------------- | :------ | :--------------------------------------- |
| Дополнение         | Бета-версия    | Добавлено действие [assign](/graph/api/intune-apps-iosmobileappconfiguration-assign?view=graph-rest-beta) для объекта [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta). |
| Дополнение         | Бета-версия    | Добавлено действие [syncDevice](/graph/api/intune-devices-manageddevice-syncdevice?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлены свойства **appsInstallAllowList**, **appsLaunchBlockList** и **appsHideList** для объекта [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **disableAppEncryptionIfDeviceEncryptionIsEnabled** для объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **disableAppEncryptionIfDeviceEncryptionIsEnabled** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **complianceGracePeriodExpirationDateTime** для объекта [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **complianceGracePeriodExpirationDateTime** для объекта [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **complianceGracePeriodExpirationDateTime** для объекта [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **subscriptions** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **version** для объекта [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **utcTimeOffsetInMinutes** для объекта [iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **complianceGracePeriodExpirationDateTime** для объекта [iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **preSharedKey** для объекта [macOSWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macoswificonfiguration?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлены свойства **phoneNumber**, **androidSecurityPatchLevel** и **userDisplayName** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлены свойства **userName**, **deviceModel**, **platform** и **complianceGracePeriodExpirationDateTime** для объекта [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **userPrincipalName** для объекта [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **overrideDefaultRule** для объекта [onPremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство **userPrincipalName** для объекта [userAppInstallStatus](/graph/api/resources/intune-apps-userappinstallstatus?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлены свойства **connectAppBlockAutoLaunch**, **deviceAccountBlockExchangeServices**, **deviceAccountEmailAddress**, **deviceAccountExchangeServerAddress**, **deviceAccountRequirePasswordRotation**, **deviceAccountSessionInitiationProtocolAddress**, **settingsBlockMyMeetingsAndFiles**, **settingsBlockSessionResume**, **settingsBlockSigninSuggestions**, **settingsDefaultVolume**, **settingsScreenTimeoutInMinutes**, **settingsSessionTimeoutInMinutes** и **settingsSleepTimeoutInMinutes** для объекта [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлено свойство навигации **deploymentSummary** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta). |
| Изменение           | Бета-версия    | Добавлены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** к сложному типу [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta). |
| Изменение           | Бета    | Для сложного типа [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) добавлены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** |
| Изменение           | Бета-версия    | Добавлено свойство **unknownCount** к сложному типу [deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-beta). |



## <a name="june-2017"></a>Июнь 2017 г.

### <a name="project-rome"></a>Project Rome

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлены следующие ресурсы и API:<br/>[Действие](/graph/api/resources/projectrome-activity?view=graph-rest-beta)<br/>[Создание или замена действия](/graph/api/projectrome-put-activity?view=graph-rest-beta)<br/>[Удаление действия](/graph/api/projectrome-delete-activity?view=graph-rest-beta)<br/>[Элемент журнала](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta)<br/>[Создание или замена элемента журнала](/graph/api/projectrome-put-historyitem?view=graph-rest-beta)<br/>[Удаление элемента журнала](/graph/api/projectrome-delete-historyitem?view=graph-rest-beta) |

### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Повышен уровень для следующих 4 свойств [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) до версии 1.0: **canEdit**, **canShare**, **canViewPrivateItems** и **owner**. |


### <a name="intune-apis"></a>Интерфейсы API Intune

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета    | Добавлены новые объекты:<br/>[defaultDeviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-defaultdevicecompliancepolicy?view=graph-rest-beta);<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta);<br/>[deviceManagementScriptDeviceState](/graph/api/resources/intune-devicefe-devicemanagementscriptdevicestate?view=graph-rest-beta);<br/>[deviceManagementScriptRunSummary](/graph/api/resources/intune-devicefe-devicemanagementscriptrunsummary?view=graph-rest-beta);<br/>[deviceManagementScriptUserState](/graph/api/resources/intune-devicefe-devicemanagementscriptuserstate?view=graph-rest-beta);<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-beta);<br/>[windowsManagedDevice](/graph/api/resources/intune-devicefe-windowsmanageddevice?view=graph-rest-beta);<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-devicefe-windowsmanagementapphealthstate?view=graph-rest-beta);<br/>[windowsManagementAppHealthSummary](/graph/api/resources/intune-devicefe-windowsmanagementapphealthsummary?view=graph-rest-beta).<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[bitLockerFixedDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerfixeddrivepolicy?view=graph-rest-beta);<br/>[bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta);<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-beta);<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devicefe-deleteuserfromsharedappledeviceactionresult?view=graph-rest-beta);<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-beta).<br/> |
| Удаление    | Бета-версия    | Удалены следующие объекты:<br/>**deviceManagementScriptState**.<br/> |
| Удаление    | Бета-версия    | Удалено действие wipeByDeviceTag для [user](/graph/api/resources/intune-devicefe-user?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **innerAuthenticationProtocolForEapTtls**, **innerAuthenticationProtocolForPeap** и **outerIdentityPrivacyTemporaryValue** для объекта [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **nonEapAuthenticationMethodForEapTtls**, **nonEapAuthenticationMethodForPeap** и **enableOuterIdentityPrivacy** для объекта [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **deployedAppCount** для объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **instanceDisplayName** и **settingPlatform** для объекта [complianceSettingStateSummary](/graph/api/resources/compliancesettingstatesummary?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **deployedAppCount** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **excludeGroup** для объекта [deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Удалены свойства **instanceDisplayName** и **settingPlatform** для объекта [deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство **devicePlatform** для объекта [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **assignmentStatus**, **assignmentProgress** и **assignmentErrorMessage** для объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **intuneBrand** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **enforceSignatureCheck** и **fileName** для объекта [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **innerAuthenticationProtocolForEapTtls** и **outerIdentityPrivacyTemporaryValue** для объекта [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **nonEapAuthenticationMethodForEapTtls** и **enableOuterIdentityPrivacy** для объекта [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **classroomAppForceUnpromptedScreenObservation**, **keyboardBlockDictation**, **networkUsageRules** и **wiFiConnectOnlyToConfiguredNetworks** для объекта [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **deployedAppCount** для объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **preSharedKey** для объекта [iosWiFiConfiguration](/graph/api/resources/intune-deviceconfig-ioswificonfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **innerAuthenticationProtocolForEapTtls** и **outerIdentityPrivacyTemporaryValue** для объекта [macOSEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macosenterprisewificonfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **nonEapAuthenticationMethodForEapTtls** и **enableOuterIdentityPrivacy** для объекта [macOSEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macosenterprisewificonfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **lastModifiedTime** и **deployedAppCount** для объекта [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **serialNumber** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство **managementAgents** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **deployedAppCount** для объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **bitLockerFixedDrivePolicy** и **bitLockerRemovableDrivePolicy** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **enterpriseCloudPrintDiscoveryEndPoint**, **enterpriseCloudPrintOAuthAuthority**, **enterpriseCloudPrintOAuthClientIdentifier**, **enterpriseCloudPrintResourceIdentifier**, **enterpriseCloudPrintDiscoveryMaxLimit**, **enterpriseCloudPrintMopriaDiscoveryResourceIdentifier**, **edgeBlockAddressBarDropdown**, **edgeBlockCompatibilityList**, **edgeClearBrowsingDataOnExit**, **edgeAllowStartPagesModification**, **edgeDisableFirstRunPage**, **edgeBlockLiveTileDataCollection** и **edgeSyncFavoritesWithInternetExplorer** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **availableVersion** для объекта [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **onboardingStatus**, **deployedVersion** и **lastModifiedTime** для объекта [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **packageIdentityName** для объекта [windowsStoreForBusinessApp](/graph/api/resources/intune-apps-windowsstoreforbusinessapp?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** для объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **mobileAppIdentifierDeployments** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **deviceConfigurationUserStateSummaries** и **iosUpdateStatuses** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство навигации **complianceSettingStateSummaries** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **runSummary**, **deviceRunStates** и **userRunStates** для объекта [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство навигации **runStates** для объекта [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** для объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** для объекта [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **mobileAppIdentifierDeployments** и **deploymentSummary** для объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **healthSummary** и **healthStates** для объекта [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **applicationId**, **appName**, **platformId**, **userFailures** и **deviceFailures** для сложного типа [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **encryptionMethod**, **startupAuthenticationRequired**, **startupAuthenticationBlockWithoutTpmChip**, **startupAuthenticationTpmUsage**, **startupAuthenticationTpmPinUsage**, **startupAuthenticationTpmKeyUsage**, **startupAuthenticationTpmPinAndKeyUsage**, **recoveryOptions** и **prebootRecoveryEnableMessageAndUrl** для сложного типа [bitLockerSystemDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockersyst?view=graph-rest-betarivepolicy). |
| Изменение      | Бета-версия    | Удалены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** для сложного типа [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** для сложного типа [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **windowsCommercialId** и **windowsCommercialIdLastModifiedTime** для сложного типа [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **address** для сложного типа [vpnServer](/graph/api/resources/intune-deviceconfig-vpnserver?view=graph-rest-beta). |


## <a name="may-2017"></a>Май 2017 г.

### <a name="application-api-changes"></a>Изменения в API приложений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версии        | Обновление API приложений. Это первый набор изменений, включающий изменение структуры и переименование свойств объекта [application](/graph/api/resources/application?view=graph-rest-beta).<br/>**Новые объекты:** [api](/graph/api/resources/api?view=graph-rest-beta]), [informationalUrl](/graph/api/resources/informationalurl?view=graph-rest-beta), [installedClient](/graph/api/resources/installedclient?view=graph-rest-beta), [permissionScope](/graph/api/resources/permissionscope?view=graph-rest-beta), [preauthorizedApplication](/graph/api/resources/preauthorizedapplication?view=graph-rest-beta), [web](/graph/api/resources/web?view=graph-rest-beta).<br/>**Удаленные свойства:** addIns, appRoles, availableToOtherOrganizations, knownClientApplications, oauth2AllowUrlPathMatching, recordConsentConditions.<br/>**Переименованные свойства:** с appId на id, с identifierUris на applicationAliases, с availableToOtherTenants на orgRestrictions, с mainLogo на logo, с oauth2Permissions на publishedPermissionsScopes, с publicClient на allowPublicClient, с replyUrls на redirectUrls.<br/>**Новые свойства:** tags. |

### <a name="remove-deprecated-planner-api"></a>Удаление устаревшего API Планировщика
| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Удаление        | Бета-версия        | Удалены следующие объекты:<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard** |

### <a name="project-rome"></a>Project Rome

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлена поддержка Project Rome, в том числе [получения списка устройств](/graph/api/user-list-devices?view=graph-rest-beta), [отправки команды устройству](/graph/api/send-device-command?view=graph-rest-beta) и [проверки состояния команды](/graph/api/get-device-command-status?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена поддержка ресурсов [activity](/graph/api/resources/projectrome-activity?view=graph-rest-beta) и [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta) для объектов user, включая [создание или замену activity](/graph/api/projectrome-put-activity?view=graph-rest-beta) и [создание или замену historyItem](/graph/api/projectrome-put-historyitem?view=graph-rest-beta). |

### <a name="administrative-units-property-changes"></a>Изменения свойств административных единиц

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | Тип свойства roleMemberInfo объекта [scopedRoleMembership](/graph/api/resources/scopedrolemembership?view=graph-rest-beta) изменен на [identity](/graph/api/resources/identity?view=graph-rest-1.0). |
| Изменение          | Бета        | Свойство навигации scopedAdministratorOf объекта [user](/graph/api/resources/user?view=graph-rest-beta) заменено на scopedRoleMemberOf. |
| Изменение          | Бета        | Свойство навигации scopedAdministrators объекта [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) заменено на scopedRoleMembers. |
| Изменение          | Бета        | Свойство навигации scopedAdministrators объекта [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-beta) заменено на scopedMembers. |

### <a name="add-users-and-groups-webhook-support-in-preview"></a>Добавлена поддержка пользователей и групп в веб-перехватчиках в бета-версии

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
| Изменение        | Бета       | Добавлена поддержка пользователей и групп в [веб-перехватчиках](/graph/api/resources/webhooks?view=graph-rest-beta).

### <a name="add-delta-query-to-v10"></a>Добавлена поддержка запросов изменений в версии 1.0

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлена поддержка функции delta в версии 1.0. Она позволяет выполнять [разностный запрос](delta-query-overview.md) для следующих объектов:<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Примеры см. в следующих статьях:<br/>[Получение добавочных изменений для групп](delta-query-groups.md)<br/>[Получение добавочных изменений для сообщений в папке](delta-query-messages.md)<br/>[Получение добавочных изменений для пользователей](delta-query-users.md) |
| Изменение          | Бета        | Добавлена возможность дополнительной фильтрации запросов (по идентификатору) для [пользователей](/graph/api/user-delta?view=graph-rest-beta) и [групп](/graph/api/group-delta?view=graph-rest-beta). |

### <a name="added-user-resource-support-for-deleted-items"></a>Добавлена поддержка работы с удаленными элементами для ресурса user

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлена поддержка [восстановления и окончательного удаления пользователей](/graph/api/resources/directory?view=graph-rest-beta). |

### <a name="added-onpremisesprovisioningerror"></a>Добавлен объект OnPremisesProvisioningError

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Новый объект: [OnPremisesProvisioningError](/graph/api/resources/onpremisesprovisioningerror?view=graph-rest-beta) |
| Изменение          | Бета        | В объекты [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta) и [orgcontact](/graph/api/resources/orgcontact?view=graph-rest-beta) добавлено свойство OnPremisesProvisioningError. |

### <a name="added-deleteddatetime-property"></a>Добавлено свойство deletedDateTime

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Изменение|Бета|В объект [user](/graph/api/resources/user?view=graph-rest-beta) добавлено свойство deletedDateTime.
|Изменение|Бета|В объект [group](/graph/api/resources/group?view=graph-rest-beta) добавлено свойство deletedDateTime.
|Изменение|Бета|В объект [application](/graph/api/resources/application?view=graph-rest-beta) добавлено свойство deletedDateTime.

### <a name="added-domain-operations-to-v10"></a>Добавлены операции с доменами в версии 1.0

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлены операции с [domains](/graph/api/resources/domain?view=graph-rest-1.0).<br/>Новые объекты:</br>[domain](/graph/api/resources/domain?view=graph-rest-1.0);<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-1.0);<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-1.0);<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-1.0);<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-1.0);<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-1.0);<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-1.0).<br/>Новые действия:</br>[verify](/graph/api/domain-verify?view=graph-rest-1.0) |

### <a name="added-contracts-to-v10"></a>Добавлены контракты в версии 1.0

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Новый объект:</br>[contract](/graph/api/resources/contract?view=graph-rest-1.0) |

### <a name="added-licensedetails-to-v10"></a>Добавлен объект licenseDetails в версии 1.0

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Новый объект:</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-1.0) |
| Изменение          | 1.0        | Добавлено свойство навигации [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-1.0) для объекта [user](/graph/api/resources/user?view=graph-rest-1.0). |


### <a name="drive-api"></a>API Диска

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Дополнение | 1.0 | Добавлен тип ресурса **baseItem**, состоящий из базовых свойств объекта **driveItem**.
| Дополнение | 1.0 и бета | В объект **thumbnail** добавлено свойство **sourceItemId**. <br/> В объект **sharepointIds** добавлено свойство **siteUrl**. <br/> В объект **shared** добавлены свойства **sharedBy** и **sharedDateTime**. <br/> В объект **remoteItem** добавлено свойство **shared**. <br/> В объекты**drive** и **itemReference** добавлено свойство **sharepointIds**. <br/> В объект **fileSystemInfo** добавлено свойство **lastAccessedDateTime**. <br/> В объект **sharedDriveItem** добавлены свойства навигации **driveItem** и **site**. <br/> В объект **baseItem** добавлено свойство **parentReference**.
| Изменение | 1.0 и бета | Объекты **driveItem** и **sharedDriveItem** теперь наследуются от объекта **baseItem**. <br/> Тип **identity** отмечен как открытый.
| Изменение | Бета | В объект **sharingLink** добавлены свойства **configuratorUrl** и **webHtml**. <br/> Добавлены тип ресурса **folderView** и свойство **view** для типа ресурса **folder**. <br/> В объект **driveItem** добавлено свойство навигации **listItem**. <br/> В объект **drive** добавлено свойство навигации **list**.


### <a name="extensions-open-extensions"></a>Расширения (открытые расширения)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Поддержка [openTypeExtension](/graph/api/resources/opentypeextension?view=graph-rest-1.0) в ресурсах [device](/graph/api/resources/device?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0), [organization](/graph/api/resources/organization?view=graph-rest-1.0) и [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Дополнение        | 1.0 и бета-версия | Если пользователь вошел с помощью личной учетной записи Майкрософт, открытые расширения поддерживаются в ресурсах event, post, group, message, contact и user. (При использовании рабочей или учебной учетной записи открытые расширения также поддерживаются в ресурсах device, group, organization и user.) |
| Дополнение        | 1.0 и бета | Поддержка параметра `$expand` для [получения открытых расширений](/graph/api/opentypeextension-get?view=graph-rest-1.0) в ресурсах [device](/graph/api/resources/device?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0), [organization](/graph/api/resources/organization?view=graph-rest-1.0), [post](/graph/api/resources/post?view=graph-rest-1.0) и [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Дополнение        | Бета          | Поддержка параметра `$expand` для [получения открытых расширений](/graph/api/opentypeextension-get?view=graph-rest-1.0) в объекте [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta). |


### <a name="extensions-schema-extensions"></a>Расширения (расширения схемы)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Новый ресурс [schemaExtension](/graph/api/resources/schemaextension?view=graph-rest-1.0) и методы CRUD для управления определениями расширений для следующих ресурсов: [contact](/graph/api/resources/contact?view=graph-rest-1.0), [device](/graph/api/resources/device?view=graph-rest-1.0), [event](/graph/api/resources/event?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0), [message](/graph/api/resources/message?view=graph-rest-1.0), [organization](/graph/api/resources/organization?view=graph-rest-1.0), [post](/graph/api/resources/post?view=graph-rest-1.0) и [user](/graph/api/resources/user?view=graph-rest-1.0). Обратите внимание, что объект [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) по-прежнему поддерживается только в бета-версии. |
| Дополнение        | 1.0          | Существующие методы POST, GET и PATCH ресурсов [contact](/graph/api/resources/contact?view=graph-rest-1.0), [device](/graph/api/resources/device?view=graph-rest-1.0), [event](/graph/api/resources/event?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0), [message](/graph/api/resources/message?view=graph-rest-1.0), [organization](/graph/api/resources/organization?view=graph-rest-1.0), [post](/graph/api/resources/post?view=graph-rest-1.0) и [user](/graph/api/resources/user?view=graph-rest-1.0) теперь поддерживают добавление, получение, обновление и удаление пользовательских данных, хранящихся в виде расширений схемы в соответствующих экземплярах ресурсов. |
| Дополнение        | 1.0 и бета-версия | Теперь вы можете использовать параметр `$filter` для поиска экземпляров ресурсов, свойства которых совпадают с определенным значениями свойств расширений, например имени. Эта возможность рассматривается подробнее в этом [примере](extensibility-schema-groups.md#5-get-a-group-and-its-extension-data). |
| Изменение          | 1.0 и бета | [Удаление определения расширения схемы](/graph/api/schemaextension-delete?view=graph-rest-1.0) больше не влияет на доступ к пользовательским данным, добавленным на основе этого определения. |
| Изменение          | 1.0 и бета | Теперь вы можете задать для сложного типа расширения схемы значение null, чтобы удалить расширение схемы из экземпляра ресурса. |


### <a name="group"></a>Группа

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Дополнение | 1.0 и бета | Добавлены свойства навигации **drives** и **sites** для объекта **group**.

### <a name="insights-apis"></a>API Insights

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета|Добавлен [API Shared](/graph/api/resources/insights-shared?view=graph-rest-beta).<br />Новые ресурсы:<br />[sharingDetail](/graph/api/resources/insights-sharingdetail?view=graph-rest-beta) <br />[insightIdentity](/graph/api/resources/insights-insightidentity?view=graph-rest-beta) <br />
|Дополнение|Бета|Добавлен [API Used](/graph/api/resources/insights-used?view=graph-rest-beta).<br />Новые ресурсы:<br />[usageDetails](/graph/api/resources/insights-usagedetails?view=graph-rest-beta) <br />
|Изменение|Бета|Новое свойство **Type** в<br />ресурсе [resourceVisualization](/graph/api/resources/insights-resourcevisualization?view=graph-rest-beta). <br />
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="intune-apis"></a>API Intune

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета    | Добавлены новые объекты:<br/>[androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta)<br/>[cartToClassAssociation](/graph/api/resources/intune-deviceconfig-carttoclassassociation?view=graph-rest-beta)<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta)<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-beta)<br/>[eBookVppGroupAssignment](/graph/api/resources/intune-books-ebookvppgroupassignment?view=graph-rest-beta)<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta)<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta)<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)<br/>[windowsDeviceMalwareState](/graph/api/resources/intune-endpointprotection-windowsdevicemalwarestate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-beta)<br/>[windowsMalwareInformation](/graph/api/resources/intune-endpointprotection-windowsmalwareinformation?view=graph-rest-beta)<br/>[windowsProtectionState](/graph/api/resources/intune-endpointprotection-windowsprotectionstate?view=graph-rest-beta)<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[androidPermissionAction](/graph/api/resources/intune-apps-androidpermissionaction?view=graph-rest-beta)<br/>[bitLockerSystemDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockersyst?view=graph-rest-betarivepolicy)<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-beta)<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-beta)<br/> |
| Дополнение    | Бета    | Добавлено действие [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) для объекта [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-beta) для объекта [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-beta) для объекта [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta). |
| Удаление    | Бета-версия    | Удалены следующие объекты:<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/> |
| Удаление    | Бета-версия    | Удалены следующие сложные типы:<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/> |
| Изменение      | Бета    | Добавлены свойства **workProfilePasswordBlockFingerprintUnlock**, **workProfilePasswordBlockTrustAgents**, **workProfilePasswordExpirationDays**, **workProfilePasswordMinimumLength**, **workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**, **workProfilePasswordPreviousPasswordBlockCount**, **workProfilePasswordSignInFailureCountBeforeFactoryReset**, **workProfilePasswordRequiredType** и **workProfileRequirePassword** для объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **kioskModeManagedApps** для объекта [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **kioskModeManagedAppId** для объекта [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [androidPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidpkcscertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [androidScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidscepcertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **hexColor** для объекта [calendar](/graph/api/resources/calendar?view=graph-rest-beta). |
| Изменение      | Бета    | Для объекта [complianceSettingStateSummary](/graph/api/resources/intune-deviceconfig-compliancesettingstatesummary?view=graph-rest-beta) добавлены свойства **setting** и **platformType** |
| Изменение      | Бета-версия    | Удалено свойство **windowsManagementAppEnabled** для объекта [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **userName**, **deviceModel** и **platform** для объекта [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **userPrincipalName** и **deviceModel** для объекта [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta). |
| Изменение      | Бета    | Для объекта [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) добавлены свойства **platformType**, **setting**, **userId** и **userEmail** |
| Изменение      | Бета    | Для объекта [deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-beta) добавлено свойство **inGracePeriodCount** |
| Изменение      | Бета    | Добавлены свойства **userName**, **deviceModel** и **platform** для объекта [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **creationOptions** для объекта [event](/graph/api/resources/event?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **isDelegated** для объекта [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-beta). |
| Изменение      | Бета    | Удалены свойства **unseenConversationsCount** и **unseenMessagesCount** для объекта [group](/graph/api/resources/group?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **settingXml** и **settings** для объекта [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [iosPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-iospkcscertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **systemIntegrityProtectionEnabled** для объекта [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета    | Для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) добавлены свойства **complianceGracePeriodExpirationDateTime**, **userPrincipalName** и **imei** |
| Изменение      | Бета    | Удалены свойства **settingXml** и **settings** для объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **useSharedComputerActivation**, **updateChannel**, **officePlatformArchitecture** и **localesToInstall** для объекта [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **applePushNotificationCertificateSetting** для объекта [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta). |
| Изменение      | Бета    | Изменены следующие свойства объекта [post](/graph/api/resources/post?view=graph-rest-beta):<br/>свойство **sender** сделано обязательным.<br/> |
| Изменение      | Бета    | Добавлены свойства **compliantUserCount**, **nonCompliantUserCount**, **remediatedUserCount**, **errorUserCount**, **unknownUserCount**, **conflictUserCount** и **notApplicableUserCount** для объекта [softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **bluetoothAllowedServices**, **bluetoothBlockPrePairing**, **cellularData**, **defenderDetectedMalwareActions**, **defenderPotentiallyUnwantedAppAction**, **lockScreenAllowTimeoutConfiguration**, **lockScreenBlockCortana**, **lockScreenBlockToastNotifications**, **lockScreenTimeoutInSeconds**, **passwordBlockSimple**, **privacyAutoAcceptPairingAndConsentPrompts**, **privacyBlockInputPersonalization**, **startMenuHideChangeAccountSettings**, **startMenuHideHibernate**, **startMenuHideLock**, **startMenuHideShutDown**, **startMenuHideSignOut**, **startMenuHideSleep**, **startMenuHideSwitchAccount**, **settingsBlockAppsPage**, **settingsBlockGamingPage**, **windowsSpotlightBlockConsumerSpecificFeatures**, **windowsSpotlightBlocked**, **windowsSpotlightBlockOnActionCenter**, **windowsSpotlightBlockTailoredExperiences**, **windowsSpotlightBlockThirdPartyNotifications**, **windowsSpotlightBlockWelcomeExperience**, **windowsSpotlightBlockWindowsTips**, **windowsSpotlightConfigureOnLockScreen** и **connectedDevicesServiceBlocked** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Удалены свойства **automaticUpdateMode**, **automaticUpdateSchedule**, **automaticUpdateTime**, **prereleaseFeatures**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips** и **experienceBlockConsumerSpecificFeatures** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [windows10PkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pkcscertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **indexingEncryptedStoresOrItemsBlocked** и **smbAutoEncryptedFileExtensions** для объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta). |
| Изменение      | Бета    | Изменены следующие свойства объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta):<br/>свойство **rightsManagementServicesTemplateId** сделано необязательным.<br/> |
| Изменение      | Бета    | Изменены следующие свойства объекта [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta):<br/>свойство **productCode** сделано необязательным.<br/> |
| Изменение      | Бета    | Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [windowsPhone81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81scepcertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **mobileAppConfigurations** для объекта [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta). |
| Изменение      | Бета    | Для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) добавлены свойства **cartToClassAssociations**, **deviceCompliancePolicySettingStateSummaries**, **remoteAssistancePartners**, **windowsInformationProtectionAppLearningSummaries** и **windowsMalwareInformation** |
| Изменение      | Бета    | Добавлено свойство навигации **eBook** для объекта [eBookGroupAssignment](/graph/api/resources/intune-books-ebookgroupassignment?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **windowsProtectionState** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **installSummary** для объекта [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство навигации **outlook** для объекта [user](/graph/api/resources/intune-deviceconfig-user?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство навигации **healthStates** для объекта [windowsManagementApp](/graph/api/resources/intune-deviceconfig-windowsmanagementapp?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **androidForWorkRestrictions** для сложного типа [defaultDeviceEnrollmentRestrictions](/graph/api/resources/intune-onboarding-defaultdeviceenrollmentrestrictions?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **userPrincipalName** и **sources** для сложного типа [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **userPrincipalName** и **sources** для сложного типа [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta). |
| Изменение      | Бета    | Для сложного типа [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) добавлены свойства **settingName**, **userId**, **userName**, **userEmail** и **currentValue** |
| Изменение      | Бета    | Удалено свойство **archiveFolder** для сложного типа [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta). |


### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Для метода **findMeetingTimes** добавлено значение перечисления **unrestricted**, указываемое в качестве свойства **activityDomain** в составе параметра **timeConstraint**. Это позволяет методу **findMeetingTimes** искать интервалы времени, соответствующие типу планируемого мероприятия. Дополнительные сведения см. в разделе [request body](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body). |
| Дополнение        | Бета-версия          | Содержание объекта **event** теперь можно получать в виде обычного текста, а не только в формате HTML. Дополнительные сведения см. в описаниях событий [get](/graph/api/event-get?view=graph-rest-beta) и [list](/graph/api/user-list-events?view=graph-rest-beta). |

### <a name="outlook-mail"></a>Почта Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | Содержание объекта **message** теперь можно получать в виде обычного текста, а не только в формате HTML. Дополнительные сведения см. в описаниях событий [get](/graph/api/message-get?view=graph-rest-beta) и [list](/graph/api/user-list-messages?view=graph-rest-beta). |


### <a name="outlook-tasks"></a>Задачи Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | В объект [user](/graph/api/resources/user?view=graph-rest-beta) добавлено новое свойство навигации **outlook** для доступа к задачам Outlook. |
| Дополнение        | Бета        | Новые объекты [outlookuser](/graph/api/resources/outlookuser?view=graph-rest-beta), [outlookTaskGroup](/graph/api/resources/outlooktaskgroup?view=graph-rest-beta), [outlookTaskFolder](/graph/api/resources/outlooktaskfolder?view=graph-rest-beta) и [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-beta), а также их методы поддерживают доступ к задачам Outlook. |
| Дополнение        | Бета        | Задачи Outlook поддерживают вложения (ресурсы [attachment](/graph/api/resources/attachment?view=graph-rest-beta), [fileAttachment](/graph/api/resources/fileattachment?view=graph-rest-beta), [itemAttachment](/graph/api/resources/itemattachment?view=graph-rest-beta) и [referenceAttachment](/graph/api/resources/referenceattachment?view=graph-rest-beta)). |
| Дополнение        | Бета        | Задачи Outlook поддерживают [расширенные свойства](/graph/api/resources/extended-properties-overview?view=graph-rest-beta) (ресурсы [singleValueLegacyExtendedProperty](/graph/api/resources/singlevaluelegacyextendedproperty?view=graph-rest-beta) и [multiValueLegacyExtendedProperty](/graph/api/resources/multivaluelegacyextendedproperty?view=graph-rest-beta)). |

### <a name="planner-apis"></a>API Планировщика

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен [API Планировщика](/graph/api/resources/planner-overview?view=graph-rest-1.0).<br />Новые ресурсы:<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-1.0) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-1.0); <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-1.0); <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-1.0); <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-1.0); <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-1.0); <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-1.0); <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-1.0) |

### <a name="sharepoint-sites"></a>Сайты SharePoint

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Дополнение      | 1.0      | Теперь в конечной точке версии 1.0 доступен ресурс сайтов.<br/> Добавлены типы ресурсов **site** и **siteCollection**.
| Изменение        | Бета      | Изменился формат идентификатора ресурса **site**. Это критическое изменение в бета-версии API.
| Удаленные элементы       | Бета      | Объект **sharePoint** удален из бета-версии API. Эта функциональность теперь доступна из коллекции **sites**.

### <a name="sharepoint-lists"></a>Списки SharePoint

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Изменение | Бета | Удалены свойства навигации **sharepoint**. Теперь для доступа к сайтам используется свойство навигации **sites**. <br/> Удален ресурс **fieldDefinition**. Он заменен ресурсом **columnDefinition**. <br/> Удалены свойства **siteCollectionId** и **siteId** объекта **site**. Используйте вместо них свойство **sharepointIds**. <br/> Удалено свойство **listItemId** объекта **listItem**. Используйте вместо него свойство **sharepointIds**. <br/> Свойство **columnSet** объекта **listItem** переименовано на **fields**. <br/> Идентификаторы ресурсов **site** теперь включают имя узла SharePoint.
| Дополнение | Бета | Добавлены типы ресурсов **booleanColumn**, **calculatedColumn**, **choiceColumn**, **dateTimeColumn**, **lookupColumn**, **numberColumn**, **personOrGroupColumn** и **textColumn**. <br/> В объект **site** добавлено свойство **displayName**. <br/> В объект **site** добавлено свойство навигации **columns**. <br/> В объект **sharedDriveItem** добавлены свойства навигации **list** и **listItem**. <br/> В объекты **list**, **listItem** и **site** добавлено свойство **sharepointIds**. <br/> Добавлен тип ресурса **columnDefinition**.




## <a name="april-2017"></a>Апрель 2017 г.

### <a name="administrative-units-property-changes"></a>Изменения свойств административных единиц

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | Обновления API административных единиц будут предоставлены в бета-версиях. Первый набор изменений будет применен 3 мая 2017 г. Изменения включают в себя следующие переименования:<br />сложный тип - **roleMemberInfo** для объекта scopedRoleMembership теперь зовется **identity**;<br />свойство навигации - **scopedAdministratorOf** для объекта user теперь зовется **scopedRoleMemberOf**;<br />свойство навигации - **scopedAdministrators** для объекта administrativeUnit теперь зовется **scopedRoleMembers**;<br />свойство навигации - **scopedAdministrators** для объекта directoryRole теперь зовется **scopedMembers**. |

### <a name="application-and-serviceprincipal-api-changes"></a>Изменения в API application и servicePrincipal

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | API [application](/graph/api/resources/application?view=graph-rest-beta) и [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) будут обновлены в бета-версии. Первый набор изменений будет применен 15 мая 2017 г. Изменения включают переименование и реструктуризацию свойств. Некоторые свойства (например, appRoles и addIns) будут доступны только после применения изменений. Прежде чем выйдет версия 1.0 с изменениями, будут выпущены бета-версии. |

### <a name="added-preview-support-for-cloud-solution-provider-developers"></a>Добавлена поддержка бета-версий для разработчиков, присоединившихся к программе Cloud Solution Provider

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Приложения, разрешение на использование которых было заранее предоставлено согласно программе Cloud Solution Provider, теперь могут вызывать Microsoft Graph. Описание см. в новой [статье об авторизации](auth-cloudsolutionprovider.md). |

### <a name="added-onpremises-properties-to-user-entity"></a>Добавлены свойства onPremises к объекту user

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | К объекту [user](/graph/api/resources/user?view=graph-rest-beta) добавлены новые свойства для onPremises: onPremisesDomainName, OnPremisesSamAccountName и onPremisesUserPrincipalName. |

### <a name="new-planner-apis-and-an-update-to-the-group-visibility-property"></a>Новые API Планировщика и обновление свойства видимости группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | Добавлено значение **HiddenMembership** для свойства видимости объекта [Group](/graph/api/resources/group?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлен новый [API Планировщика](/graph/api/resources/planner-overview?view=graph-rest-beta).<br />Новые ресурсы:<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-beta); <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta); <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-beta); <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-beta); <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-beta); <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-beta); <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-beta). |

### <a name="intune-apis"></a>API Intune
| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлены новые объекты:<br/>[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta);<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta);<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-beta);<br/>[deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta)<br/>[deviceManagementScriptGroupAssignment](/graph/api/resources/intune-deviceconfig-devicemanagementscriptgroupassignment?view=graph-rest-beta)<br/>[deviceManagementScriptState](/graph/api/resources/intune-deviceconfig-devicemanagementscriptstate?view=graph-rest-beta)<br/>[eBookGroupAssignment](/graph/api/resources/intune-books-ebookgroupassignment?view=graph-rest-beta);<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-beta);<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta);<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-beta);<br/>[windowsManagementApp](/graph/api/resources/intune-deviceconfig-windowsmanagementapp?view=graph-rest-beta)<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-deviceconfig-windowsmanagementapphealthstate?view=graph-rest-beta)<br/> |
| Дополнение        | Бета        | Добавлены новые сложные типы:<br/>[dailySchedule](/graph/api/resources/intune-deviceconfig-dailyschedule?view=graph-rest-beta)<br/>[hourlySchedule](/graph/api/resources/intune-deviceconfig-hourlyschedule?view=graph-rest-beta)<br/>[iosBookmark](/graph/api/resources/intune-deviceconfig-iosbookmark?view=graph-rest-beta);<br/>[iosWebContentFilterAutoFilter](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterautofilter?view=graph-rest-beta);<br/>[iosWebContentFilterBase](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterbase?view=graph-rest-beta);<br/>[iosWebContentFilterSpecificWebsitesAccess](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterspecificwebsitesaccess?view=graph-rest-beta);<br/>[runSchedule](/graph/api/resources/intune-deviceconfig-runschedule?view=graph-rest-beta)<br/>[sharedAppleDeviceUser](/graph/api/resources/intune-deviceconfig-sharedappledeviceuser?view=graph-rest-beta)<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-beta).<br/> |
| Дополнение        | Бета-версия        | Добавлено действие [requestRemoteAssistance](/graph/api/intune-devices-manageddevice-requestremoteassistance?view=graph-rest-beta) к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлено действие [cleanWindowsDevice](/graph/api/intune-devices-manageddevice-cleanwindowsdevice?view=graph-rest-beta) к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлено действие [logoutSharedAppleDeviceActiveUser](/graph/api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser?view=graph-rest-beta) к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлено действие [deleteUserFromSharedAppleDevice](/graph/api/intune-devices-manageddevice-deleteuserfromsharedappledevice?view=graph-rest-beta) к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлено действие [assign](/graph/api/intune-deviceconfig-devicemanagementscript-assign?view=graph-rest-beta) к объекту [deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлено действие [syncLicenses](/graph/api/intune-onboarding-applevolumepurchaseprogramtoken-synclicenses?view=graph-rest-beta) к объекту [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена функция **getTopMobileApps** для коллекции [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена функция [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-deviceconfig-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-beta) к объекту [applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена функция [getDeviceComplianceSettingStates](/graph/api/intune-deviceconfig-devicemanagement-getdevicecompliancesettingstates?view=graph-rest-beta) к объекту [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена функция [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-beta) к объекту [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена функция [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-beta) к объекту [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
| Удаление        | Бета-версия        | Удалены следующие сложные типы:<br/>**enterpriseCloudResource**;<br/>**windowsInformationProtectionAppRule**;<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**<br/>**windowsInformationProtectionAppRuleDesktopTemplate**<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**<br/>**windowsInformationProtectionAppRuleTemplate**<br/>**windowsInformationProtectionCorporateNetworkLocation**;<br/>**windowsInformationProtectionProtectedLocation**;<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**<br/>**windowsInformationProtectionProtectedLocationNeutralResources**.<br/> |
| Изменение          | Бета-версия        | Добавлено свойство **deviceSharingAllowed** к объекту [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Удалено **deviceSharingBlocked** свойство из объекта [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **minimumRequiredSdkVersion** к объекту [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **windowsManagementAppEnabled** к объекту [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **notificationTemplateId** к объекту [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **excludeGroup** к объекту [deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta) |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-beta):<br/>**payloadFileName** теперь можно не указывать.<br/> |
| Изменение          | Бета-версия        | Добавлено свойство **contentFilterSettings** к объекту [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлены свойства **cellularBlockPersonalHotspot** и **passcodeBlockFingerprintModification** к объекту [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **minimumRequiredSdkVersion** к объекту [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-beta):<br/>**payloadFileName** теперь можно не указывать.<br/> |
| Изменение          | Бета-версия        | Добавлены свойства **disableAppPinIfDevicePinIsSet**, **minimumRequiredOsVersion**, **minimumWarningOsVersion**, **minimumRequiredAppVersion** и **minimumWarningAppVersion** к объекту [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлены свойства **remoteAssistanceSessionUrl**, **isEncrypted**, **model** и **manufacturer** к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [getMobileAppCount](/graph/api/intune-apps-mobileapp-getmobileappcount?view=graph-rest-beta):<br/>для **bindingParameter** вместо **mobileApp** теперь используется **коллекция** *mobileApp*;<br/>для свойства **status** вместо типа GUID теперь используется String.<br/> |
| Изменение          | Бета-версия        | Добавлено свойство **vpnConfigurationId** к объекту [mobileAppGroupAssignment](/graph/api/resources/intune-apps-mobileappgroupassignment?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Удалено свойство **fromEmailAddress** из объекта [notificationMessageTemplate](/graph/api/resources/intune-deviceconfig-notificationmessagetemplate?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **excludedApps** к объекту [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Удалено свойство **excludedOfficeApps** из объекта [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **enabled** к объекту [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлены свойства **networkProxyApplySettingsDeviceWide**, **networkProxyDisableAutoDetect**, **networkProxyAutomaticConfigurationUrl**, **networkProxyServer**, **bluetoothDeviceName**, **wiFiScanInterval**, **wirelessDisplayBlockProjectionToThisDevice**, **wirelessDisplayBlockUserInputFromReceiver**, **wirelessDisplayRequirePinForPairing**, **experienceBlockDeviceDiscovery**, **experienceBlockErrorDialogWhenNoSIM**, **experienceBlockTaskSwitcher**, **startMenuPinnedFolderDocuments**, **startMenuPinnedFolderDownloads**, **startMenuPinnedFolderFileExplorer**, **startMenuPinnedFolderHomeGroup**, **startMenuPinnedFolderMusic**, **startMenuPinnedFolderNetwork**, **startMenuPinnedFolderPersonalFolder**, **startMenuPinnedFolderPictures**, **startMenuPinnedFolderSettings**, **startMenuPinnedFolderVideos**, **startMenuAppListVisibility**, **startMenuHideFrequentlyUsedApps**, **startMenuHideRecentJumpLists**, **startMenuHideRecentlyAddedApps**, **startMenuHideRestartOptions**, **startMenuHideUserTile**, **startMenuHidePowerButton**, **startMenuLayoutEdgeAssetsXml**, **personalizationDesktopImageUrl** и **personalizationLockScreenImageUrl** к объекту [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Изменен тип следующих свойств объекта [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta):<br/>**productCode** теперь относится не к Guid, а к String.<br/> |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta):<br/>**phoneProductIdentifier** больше не обязательно указывать;<br/>**phonePublisherId** больше не обязательно указывать.<br/> |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [windowsPhone81AppXBundle](/graph/api/resources/intune-apps-windowsphone81appxbundle?view=graph-rest-beta):<br/>**appXPackageInformationList** больше не обязательно указывать.<br/> |
| Изменение          | Бета-версия        | Добавлены свойства **productKey** и **licenseType** к объекту [windowsStoreForBusinessApp](/graph/api/resources/intune-apps-windowsstoreforbusinessapp?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **previewBuildSetting** к объекту [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлены свойства навигации **windowsManagementApp** и **managedEBooks** к объекту [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлены свойства навигации **deviceManagementScripts**, **managedDeviceOverview** и **cloudPkiSubscriptions** к объекту [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлены свойства **osMinimumVersion** и **osMaximumVersion** к сложному типу [deviceEnrollmentPlatformRestrictions](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictions?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлены свойства **isSharedDevice** и **sharedDeviceCachedUsers** к сложному типу [hardwareInformation](/graph/api/resources/intune-deviceconfig-hardwareinformation?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Изменены следующие свойства сложного типа [omaSettingBase64](/graph/api/resources/intune-deviceconfig-omasettingbase64?view=graph-rest-beta):<br/>**fileName** больше не обязательно указывать.<br/> |
| Изменение          | Бета-версия        | Изменены следующие свойства сложного типа [omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-beta):<br/>**fileName** больше не обязательно указывать.<br/> |

## <a name="march-2017"></a>Март 2017 г.

### <a name="intune-apis"></a>API Intune

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета    | Добавлены новые объекты:<br/>[androidForWorkApp](/graph/api/resources/intune-apps-androidforworkapp?view=graph-rest-beta);<br/>[androidForWorkAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschema?view=graph-rest-beta);<br/>[androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta);<br/>[androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta);<br/>[applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta)<br/>[complianceSettingStateSummary](/graph/api/resources/intune-deviceconfig-compliancesettingstatesummary?view=graph-rest-beta);<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-beta);<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-beta);<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-beta);<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-beta);<br/>[enterpriseCodeSigningCertificate](/graph/api/resources/intune-apps-enterprisecodesigningcertificate?view=graph-rest-beta);<br/>[iosEduDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosedudeviceconfiguration?view=graph-rest-beta);<br/>[managedDeviceCertificateState](/graph/api/resources/intune-devices-manageddevicecertificatestate?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta);<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta);<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy);<br/>[mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta);<br/>[mobileAppProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-mobileappprovisioningconfiggroupassignment?view=graph-rest-beta);<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta);<br/>[officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta);<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-beta);<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-beta);<br/>[symantecCodeSigningCertificate](/graph/api/resources/intune-apps-symanteccodesigningcertificate?view=graph-rest-beta);<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta);<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta);<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-beta);<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta);<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta).<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[androidForWorkAppConfigurationExample](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexample?view=graph-rest-beta);<br/>[androidForWorkAppConfigurationExampleJson](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexamplejson?view=graph-rest-beta);<br/>[androidForWorkAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschemaitem?view=graph-rest-beta);<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta);<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta);<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-deviceconfig-deviceexchangeaccessstatesummary?view=graph-rest-beta)<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-beta);<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-beta);<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-beta);<br/>[excludedApps](/graph/api/resources/intune-apps-excludedapps?view=graph-rest-beta);<br/>[iosEduCertificateSettings](/graph/api/resources/intune-deviceconfig-ioseducertificatesettings?view=graph-rest-beta);<br/>[ipRange](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta);<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta);<br/>[windowsInformationProtectionCloudResource](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresource?view=graph-rest-beta);<br/>[windowsInformationProtectionCloudResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresourcecollection?view=graph-rest-beta);<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-beta);<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-beta);<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-beta);<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-beta).<br/> |
| Дополнение    | Бета    | Добавлено действие [requestSignupUrl](/graph/api/intune-androidforwork-androidforworksettings-requestsignupurl?view=graph-rest-beta) к объекту [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [completeSignup](/graph/api/intune-androidforwork-androidforworksettings-completesignup?view=graph-rest-beta) к объекту [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [syncApps](/graph/api/intune-androidforwork-androidforworksettings-syncapps?view=graph-rest-beta) к объекту [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [unbind](/graph/api/intune-androidforwork-androidforworksettings-unbind?view=graph-rest-beta) к объекту [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) к объекту [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [recoverPasscode](/graph/api/intune-devices-manageddevice-recoverpasscode?view=graph-rest-beta) к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [removeApplePushNotificationCertificate](/graph/api/intune-onboarding-organization-removeapplepushnotificationcertificate?view=graph-rest-beta) к объекту [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-iosmanagedappprotection-updatemobileappidentifierdeployments?view=graph-rest-beta) к объекту [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-androidmanagedappprotection-updatemobileappidentifierdeployments?view=graph-rest-beta) к объекту [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-targetedmanagedappconfiguration-updatemobileappidentifierdeployments?view=graph-rest-beta) к объекту [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [updateTargetedSecurityGroups](/graph/api/intune-mam-iosmanagedappprotection-updatetargetedsecuritygroups?view=graph-rest-beta) к объекту [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [updateTargetedSecurityGroups](/graph/api/intune-mam-androidmanagedappprotection-updatetargetedsecuritygroups?view=graph-rest-beta) к объекту [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [updateTargetedSecurityGroups](/graph/api/intune-mam-windowsinformationprotection-updatetargetedsecuritygroups?view=graph-rest-beta) к объекту [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [updateTargetedSecurityGroups](/graph/api/intune-mam-windowsinformationprotection-updatetargetedsecuritygroups?view=graph-rest-beta) к объекту [windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [updateTargetedSecurityGroups](/graph/api/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy-updatetargetedsecuritygroups) к объекту [mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy). |
| Дополнение    | Бета-версия    | Добавлено действие [wipeManagedAppRegistrationByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationbydevicetag?view=graph-rest-beta) к объекту [user](/graph/api/resources/intune-deviceconfig-user?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлена функция [getTopMobileApps](/graph/api/intune-apps-mobileapp-gettopmobileapps?view=graph-rest-beta) к объекту [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлена функция [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-corpenrollment-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-beta) к объекту [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Удаление    | Бета-версия    | Удалены следующие объекты:<br/>**appProvisioningConfigGroupAssignment**;<br/>**defaultManagedAppConfiguration**;<br/>**enterpriseCertificate**;<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**;<br/>**symantecCertificate**;<br/>**windows10WindowsInformationProtectionConfiguration**.<br/> |
| Удаление    | Бета-версия    | Удалены следующие сложные типы:<br/>**mobileAppInstallSummary**;<br/>**windowsArchitecture**;<br/>**windowsDeviceType**.<br/> |
| Изменение      | Бета-версия    | Добавлено свойство **webBrowserBlockPopups** к объекту [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство **webBrowserAllowPopups** из объекта [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **appIdentifier** к объекту [androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **applicationCount**, **failedApplicationCount** и **appInstallFailures** из объекта [appReportingOverviewStatus](/graph/api/resources/appreportingoverviewstatus?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **sharedIPadMaximumUserCount** и **enableSharedIPad** к объекту [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **shareTokenWithSchoolDataSyncService** и **lastSyncErrorCode** к объекту [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** и **policyRevision** из объекта [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **numberOfPendingUsers**, **numberOfSucceededUsers**, **numberOfErrorUsers**, **numberOfFailedUsers**, **lastUpdateTime** и **policyRevision** из объекта [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** и **policyRevision** из объекта [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** и **configurationVersion** к объекту [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **numberOfPendingUsers**, **numberOfSucceededUsers**, **numberOfErrorUsers**, **numberOfFailedUsers**, **lastUpdateTime** и **policyRevision** из объекта [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **subscriptionState** к объекту [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **managedEmailProfileRequired** к объекту [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **appsSingleAppModeList** к объекту [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство **appsSingleAppModeBundleIds** из объекта [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **expirationDateTime** к объекту [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство **expiration** из объекта [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **passwordMinimumCharacterSetCount**, **osMinimumVersion**, **osMaximumVersion**, **deviceThreatProtectionEnabled**, **deviceThreatProtectionRequiredSecurityLevel** и **storageRequireEncryption** к объекту [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство **manifest** из объекта [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **isSupervised**, **exchangeLastSuccessfulSyncDateTime**, **exchangeAccessState** и **exchangeAccessStateReason** к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **deviceExchangeAccessStateSummary** к объекту [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство **manifest** из объекта [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство **installSummary** из объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **uploadState** к объекту [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Изменены следующие свойства объекта [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta):<br/>**azureStorageUriExpirationDateTime** больше не обязательно указывать.<br/> |
| Изменение      | Бета-версия    | Добавлены свойства **initiatedByUserPrincipalName**, **deviceOwnerUserPrincipalName**, **deviceIMEI** и **actionState** к объекту [remoteActionAudit](/graph/api/resources/intune-deviceconfig-remoteactionaudit?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **oneDriveDisableFileSync**, **safeSearchFilter**, **edgeSearchEngine**, **settingsBlockSettingsApp**, **settingsBlockSystemPage**, **settingsBlockDevicesPage**, **settingsBlockNetworkInternetPage**, **settingsBlockPersonalizationPage**, **settingsBlockAccountsPage**, **settingsBlockTimeLanguagePage**, **settingsBlockEaseOfAccessPage**, **settingsBlockPrivacyPage**, **settingsBlockUpdateSecurityPage**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips**, **experienceBlockConsumerSpecificFeatures**, **startMenuLayoutXml**, **startMenuMode**, **logonBlockFastUserSwitching** и **startBlockUnpinningAppsFromTaskbar** к объекту [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **allowPrinting**, **allowScreenCapture** и **allowTextSuggestion** к объекту [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **blockPrinting**, **blockScreenCapture** и **blockTextSuggestion** из объекта [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **identityName** к объекту [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Изменен тип следующих свойств объекта [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta):<br/>**applicableArchitectures** теперь относится не к [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta), а к String.<br/> |
| Изменение      | Бета-версия    | Добавлено свойство **identityName** к объекту [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Изменен тип следующих свойств объекта [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta):<br/>**applicableArchitectures** теперь относится не к [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta), а к String.<br/> |
| Изменение      | Бета-версия    | Добавлены свойства **identityName**, **identityPublisherHash** и **identityResourceIdentifier** к объекту [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Изменен тип следующих свойств объекта [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta):<br/>**applicableArchitectures** теперь относится не к [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta), а к String;<br/>**applicableDeviceTypes** теперь относится не к [windowsDeviceType](/graph/api/resources/windowsdevicetype?view=graph-rest-beta), а к String.<br/> |
| Изменение      | Бета-версия    | Добавлено свойство **restartMode** к объекту [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [androidScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidscepcertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **enterpriseCodeSigningCertificates**, **symantecCodeSigningCertificate**, **sideLoadingKeys**, **managedAppPolicies**, **iosManagedAppProtections**, **androidManagedAppProtections**, **defaultManagedAppProtections**, **targetedManagedAppConfigurations**, **mdmWindowsInformationProtectionPolicies**, **windowsInformationProtectionPolicies**, **managedAppRegistrations** и **managedAppStatuses** к объекту [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства навигации **appReportingOverview**, **enterpriseCerts** и **symantecCert** из объекта [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **deviceSettingStateSummaries** к объекту [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **deviceSettingStateSummaries** к объекту [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **termsAndConditions**, **androidForWorkSettings**, **androidForWorkAppConfigurationSchemas**, **applePushNotificationCertificate**, **softwareUpdateStatusSummary**, **deviceCompliancePolicyDeviceStateSummary**, **complianceSettingStateSummaries**, **deviceConfigurationDeviceStateSummaries** и **mobileThreatDefenseConnectors** к объекту [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства навигации **teacherRootCertificates**, **teacherIdentityCertificate**, **studentRootCertificates** и **studentIdentityCertificate** из объекта [iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Изменен тип следующих свойств объекта [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta):<br/>**deviceStatuses** теперь относится не к коллекции [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](/graph/api/resources/manageddevicemobileappprovisioningconfigurationdevicestatus?view=graph-rest-beta), а к коллекции [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta).<br/>**groupAssignments** теперь относится не к коллекции [appProvisioningConfigGroupAssignment](/graph/api/resources/appprovisioningconfiggroupassignment?view=graph-rest-beta), а к коллекции [mobileAppProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-mobileappprovisioningconfiggroupassignment?view=graph-rest-beta).<br/> |
| Изменение      | Бета-версия    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **deviceConfigurationStates** и **deviceCompliancePolicyStates** к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства навигации **deviceStatusSummary** и **userStatusSummary** к объекту [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **installSummary** к объекту [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство навигации **sideLoadingKeys** из объекта [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta). |
| Изменение      | бета    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [windowsPhone81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81scepcertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **applicationId**, **appName**, **platformId**, **userFailures** и **deviceFailures** из сложного типа [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **displayName** к сложному типу [iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **displayName** к сложному типу [iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **subjectName**, **description**, **expirationDateTime** и **certificate** к сложному типу [windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **dataRecoveryCertificate** и **certificateFileName** из сложного типа [windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **displayName** к сложному типу [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Изменен тип следующих свойств сложного типа [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta):<br/>**applicableArchitecture** теперь относится не к [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta), а к String.<br/> |
| Изменение      | Бета-версия    | Изменены следующие свойства сложного типа [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta):<br/>свойство **applicableArchitecture** сделано обязательным.<br/> |

### <a name="add-contracts-to-microsoft-graph"></a>Добавление контрактов в Microsoft Graph

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Новый ресурс:</br>[contract](/graph/api/resources/contract?view=graph-rest-beta). |

### <a name="add-domain-operations-to-microsoft-graph"></a>Добавление операций с доменами в Microsoft Graph

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены функции к объектам [domains](/graph/api/resources/domain?view=graph-rest-beta).<br/>Новые объекты:</br>[domain](/graph/api/resources/domain?view=graph-rest-beta);<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-beta);<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-beta);<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-beta);<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-beta);<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-beta);<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-beta).<br/>Новые действия:</br>[forceDelete](/graph/api/domain-forcedelete?view=graph-rest-beta);</br>[verify](/graph/api/domain-verify?view=graph-rest-beta). |

### <a name="add-custom-data-to-microsoft-graph-using-schema-extensions"></a>Добавление пользовательских данных в Microsoft Graph с помощью расширений схемы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавление данных приложения в Microsoft Graph с помощью [расширений схемы](extensibility-overview.md#schema-extensions)  поддерживается для следующих ресурсов:<br/>administrative unit;<br/>calendar event;<br/>device;<br/>group;<br/>message;<br/>organization;<br/>personal contact;<br/>post;<br/>user.<br/>Пример приведен в следующей статье:<br/>[Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](extensibility-schema-groups.md). |
| Дополнение        | Бета        | Предоставлен альтернативный способ создания определения расширения схемы без подтвержденного личного домена .com. Подробности см. в разделе [Расширения схемы](extensibility-overview.md#schema-extensions). |

### <a name="add-custom-data-to-microsoft-graph-using-open-extensions"></a>Добавление пользовательских данных в Microsoft Graph с помощью открытых расширений

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Вместо термина "расширения данных Office 365" теперь используется "открытые расширения". |
| Дополнение        | Бета-версия          | Добавлены ресурсы, которые поддерживают [открытые расширения](extensibility-overview.md#open-extensions): <br/>administrative unit;<br/>device;<br/>группа<br/>organization;<br/>user.<br/>Пример приведен в следующей статье:<br/>[Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](extensibility-open-users.md). |

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена поддержка [восстановления и окончательного удаления групп](/graph/api/resources/directory?view=graph-rest-beta).<br/>Новый объект: каталог со свойством навигации deleteditems. |
| Дополнение        | Бета        | Новый объект:</br>[Конечная точка](/graph/api/resources/endpoint?view=graph-rest-beta) |
| Изменение          | Бета        | Новое свойство навигации [endpoints](/graph/api/group-list-endpoints?view=graph-rest-beta) для ресурса [group](/graph/api/resources/group?view=graph-rest-beta) |
| Дополнение        | Бета        | Новый объект:</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-beta) |
| Изменение          | Бета        | Добавлено свойство навигации [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-beta) для объекта [user](/graph/api/resources/user?view=graph-rest-beta). |

### <a name="reports-apis"></a>API отчетов

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Представлена предварительная версия нового API для функций создания отчетов в Office 365. С его помощью можно получать отчеты об использовании служб Office 365 сотрудниками компании. Например, вы можете определить, кто использует службу по максимуму, а кому вообще не нужна лицензия Office 365. Дополнительные сведения см. в статье о ресурсе [report](/graph/api/resources/report?view=graph-rest-beta). |

### <a name="directory-apis"></a>API каталогов

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Новый объект:</br>[contract](/graph/api/resources/contract?view=graph-rest-beta). |

## <a name="february-2017"></a>Февраль 2017 г.

### <a name="intune-apis"></a>API Intune

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета    | Добавлены новые объекты:<br/>[androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta)<br/>[androidForWorkEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkeasemailprofilebase?view=graph-rest-beta)<br/>[androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidForWorkGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgmaileasconfiguration?view=graph-rest-beta)<br/>[androidForWorkNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworknineworkeasconfiguration?view=graph-rest-beta)<br/>[androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta)<br/>[androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta)<br/>[androidForWorkTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidforworktrustedrootcertificate?view=graph-rest-beta)<br/>[androidForWorkWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkwificonfiguration?view=graph-rest-beta)<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-beta)<br/>[appProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-appprovisioningconfiggroupassignment?view=graph-rest-beta)<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta)<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta)<br/>[enterpriseCertificate](/graph/api/resources/intune-apps-enterprisecertificate?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappprovisioningconfigurationdevicestatus?view=graph-rest-beta)<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta)<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta)<br/>[symantecCertificate](/graph/api/resources/intune-apps-symanteccertificate?view=graph-rest-beta)<br/>[windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta)<br/>[windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta)<br/>[windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta)<br/>[windowsPhone81AppXBundle](/graph/api/resources/intune-apps-windowsphone81appxbundle?view=graph-rest-beta)<br/>[windowsPhoneXAP](/graph/api/resources/intune-apps-windowsphonexap?view=graph-rest-beta)<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta)<br/> |
| Дополнение    | Бета    | Добавлены новые сложные типы:<br/>[airPrintDestination](/graph/api/resources/intune-deviceconfig-airprintdestination?view=graph-rest-beta)<br/>[windowsArchitecture](/graph/api/resources/intune-apps-windowsarchitecture?view=graph-rest-beta)<br/>[windowsDeviceType](/graph/api/resources/intune-apps-windowsdevicetype?view=graph-rest-beta)<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta)<br/>[windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta)<br/> |
| Дополнение    | Бета    | Добавлено действие [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) к объекту [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие [scheduleActionsForRules](/graph/api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules?view=graph-rest-beta) к объекту [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие [updateTargetedSecurityGroups](/graph/api/intune-mam-targetedmanagedappconfiguration-updatetargetedsecuritygroups?view=graph-rest-beta) к объекту [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлена функция [getScopesForUser](/graph/api/intune-rbac-resourceoperation-getscopesforintune-devices-user?view=graph-rest-beta) к объекту [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **manifest** из объекта [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **assetTagTemplate**, **lockScreenFootnote**, **homeScreenDockIcons** и **homeScreenPages** к объекту [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Удалены свойства **deviceSharingAssetTagInformation**, **deviceSharingLockScreenFootnote**, **homeScreenLayoutDockIcons** и **homeScreenLayoutPages** из объекта [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **appsSingleAppModeBundleIds** к объекту [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **manifest** из объекта [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **createdDateTime**, **description**, **lastModifiedDateTime**, **displayName** и **version** к объекту [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **createdDateTime** и **lastModifiedDateTime** к объекту [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **deviceRegistrationState** из объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **manifest** к объекту [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **osDescription** и **userName** к объекту [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **deviceType** из объекта [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta). |
| Изменение      | Бета    | Изменен тип следующих свойств объекта [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta):<br/>**mobileAppInstallStatusValue** (с Int32 на String) |
| Изменение      | Бета    | Добавлены свойства **targetedSecurityGroupIds** и **targetedSecurityGroupsCount** к объекту [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **numberOfTargetedSecurityGroups** из объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **id** к объекту [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta). |
| Изменение      | Бета    | Удалены свойства **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** и **certificateValidityPeriodScale** из объекта [windows10CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows10certificateprofilebase?view=graph-rest-beta). |
| Изменение      | Бета    | Удалены свойства **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** и **certificateValidityPeriodScale** из объекта [windows81CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows81certificateprofilebase?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство **applyToWindows10Mobile** из объекта [windowsPhone81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81generalconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства навигации **enterpriseCerts**, **iosLobAppProvisioningConfigurations** и **symantecCert** к объекту [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **userStatusOverview** к объекту [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **userStatusOverview** к объекту [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства навигации **groupAssignments**, **deviceStatuses** и **userStatuses** к объекту [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Изменен тип следующих свойств объекта [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta):<br/>**identityCertificate** (с [windows10CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows10certificateprofilebase?view=graph-rest-beta) на [windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta)) |
| Изменение      | Бета    | Добавлены свойства **deviceComplianceCheckinThresholdDays** и **isScheduledActionEnabled** к сложному типу [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta). |
| Изменение      | Бета    | Удалены свойства **windowsCommercialId** и **windowsCommercialIdLastModifiedTime** из сложного типа [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **bundleID**, **appName**, **publisher**, **enabled** и **showOnLockScreen** к сложному типу [iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta). |
| Изменение      | Бета    | Удалены свойства **bundleIdentifier**, **notificationsEnabled** и **showInLockScreen** из сложного типа [iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta). |



## <a name="january-2017"></a>Январь 2017 г.

### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | v1.0        | Новое действие [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) для ресурса [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Новый сложный тип [attendeeBase](/graph/api/resources/attendeebase?view=graph-rest-1.0), который состоит из свойства типа участников. |
| Дополнение        | 1.0        | Новые сложные типы:<br/>[attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-1.0)<br/>[locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-1.0) <br/>[locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-1.0)<br/>[meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-1.0)<br/>[meetingTimeSuggestionsResult](/graph/api/resources/meetingtimesuggestionsresult?view=graph-rest-1.0)<br/>[timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-1.0)<br/>[timeSlot](/graph/api/resources/timeslot?view=graph-rest-1.0) |
| Изменение          | 1.0        | Сложный тип [attendee](/graph/api/resources/attendee?view=graph-rest-1.0) теперь является производным от attendeeBase, который, в свою очередь, является производным от [recipient](/graph/api/resources/recipient?view=graph-rest-1.0). Он состоит из тех же свойств **status**, **type** и **emailAddress**, что и раньше, а также унаследованных свойств. |
| Дополнение        | Бета        | В ресурс [calendar](/graph/api/resources/calendar?view=graph-rest-beta) добавлено свойство hexColor. |

### <a name="intune-apis"></a>API Intune

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлены новые объекты: <br/>[appReportingOverviewStatus](/graph/api/resources/intune-apps-appreportingoverviewstatus?view=graph-rest-beta)<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta)<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta)<br/>[deviceManagementExchangeOnpremisesPolicy](/graph/api/resources/intune-onboarding-devicemanagementexchangeonpremisespolicy?view=graph-rest-beta)<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)<br/>[onpremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-beta)<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta)<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-beta)<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)<br/>[windows10WindowsInformationProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10windowsinformationprotectionconfiguration?view=graph-rest-beta) |
|Дополнение|Бета|Добавлены новые сложные типы: <br/> [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta)<br/>[enterpriseCloudResource](/graph/api/resources/intune-deviceconfig-enterprisecloudresource?view=graph-rest-beta)<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-beta)<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-beta)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-beta)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-beta)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-beta)<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta)<br/>[iPv6Range](/graph/api/resources/intune-deviceconfig-ipv6range?view=graph-rest-beta)<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRule](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprule?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruleapplockerpolicyfiletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruledesktoptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprulestoreapptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionCorporateNetworkLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectioncorporatenetworklocation?view=graph-rest-beta)<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocation?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisecloudresources?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv4ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv6ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationneutralresources?view=graph-rest-beta)
|Удаление|Бета|Следующие сложные типы удалены и заменены на тип microsoft.graph.Json:<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|Изменение|Бета|Для следующих объектов тип свойства appConfigComplianceStatus заменен на complianceStatus: <br/>[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-beta)|
|Изменение|Бета|Для ресурса [managedAppStatusRaw](/graph/api/resources/intune-mam-managedappstatusraw?view=graph-rest-beta) тип свойства content изменен с managedAppSummary на Json.|
|Изменение|Бета|Из коллекции [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta) удалена функция getUsersWithFlaggedAppRegistration.|
|Изменение|Бета|Изменено свойство навигации **vppToken** объекта [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta), теперь он не является включенной коллекцией.|
|Изменение|Бета|Добавлено свойство **deviceStatusOverview** к объектам [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) и [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **appReportingOverview** к одиночному объекту [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **deviceDisplayName** и **userPrincipalName** к объектам [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta), [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) и [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **ruleName** к объекту [deviceComplianceScheduledActionForRule](/graph/api/resources/intune-deviceconfig-devicecompliancescheduledactionforrule?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **devicesCount**, **userDisplayName** и **userPrincipalName** к объектам [deviceConfigurationUserStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatus?view=graph-rest-beta), [deviceComplianceUserStatus](/graph/api/resources/intune-deviceconfig-devicecomplianceuserstatus?view=graph-rest-beta) и [managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-beta).|
|Изменение|Бета|Добавлена коллекция [notificationMessageTemplates](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta) к одиночному объекту [deviceManagement](/graph/api/resources/intune-deviceconfig-devicemanagement?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **isDefault**, **lastModifiedDateTime**, **locale**, **messageTemplate** и **subject** к объекту [localizedNotificationMessage](/graph/api/resources/intune-deviceconfig-localizednotificationmessage?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **azureActiveDirectoryDeviceId**, **deviceCategory**, **deviceRegistrationState** и **managementAgent** к объекту [managedDevice](/graph/api/resources/intune-onboarding-manageddevice?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **lastModifiedDateTime** к объекту [mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **brandingOptions**, **defaultLocale**, **displayName**, **fromEmailAddress**, **lastModifiedDateTime**, **localizedNotificationMessages** к объекту [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **appsAllowTrustedAppsSideloading**, **appsBlockWindowsStoreOriginatedApps**, **developerUnlockSetting**, **edgeBlockAccessToAboutFlags**, **edgeBlockDeveloperTools**, **edgeBlockExtensions**, **edgeBlockInPrivateBrowsing**, **edgeFirstRunUrl**, **edgeHomepageUrls**, **gameDvrBlocked**, **settingsBlockAddProvisioningPackage**, **settingsBlockChangeLanguage**, **settingsBlockChangePowerSleep**, **settingsBlockChangeRegion**, **settingsBlockChangeSystemTime**, **settingsBlockEditDeviceName**, **settingsBlockRemoveProvisioningPackage**, **sharedUserAppDataAllowed**, **smartScreenBlockPromptOverride**, **smartScreenBlockPromptOverrideForFiles**, **storageRestrictAppDataToSystemVolume**, **storageRestrictAppInstallToSystemVolume**, **webRtcBlockLocalhostIpAddress**, **windowsStoreBlockAutoUpdate** и **windowsStoreEnablePrivateStoreOnly** к объекту [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|

## <a name="december-2016"></a>Декабрь 2016 г.

### <a name="delta-query"></a>Запрос на получение различий

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | В следующие объекты добавлена новая функция delta для выполнения [запроса на получение различий](delta-query-overview.md):<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Примеры см. в следующих статьях:<br/>[Получение добавочных изменений групп (предварительная версия)](delta-query-groups.md)<br/>[Получение добавочных изменений сообщений в папке (предварительная версия)](delta-query-messages.md)<br/>[Получение добавочных изменений пользователей (предварительная версия)](delta-query-users.md) |

### <a name="excel-apis"></a>API Excel

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | v1.0        | Добавлены ресурс workbookPivotTable, действия refresh и refreshAll в сводных таблицах, ресурс workbookRangeView, действие visibleView в отфильтрованном диапазоне для возврата workbookRangeView пользователю, коллекция строк get и ресурс range из visibleView, функции columnsAfter, columnsBefore, resizedRange, rowsAbove и rowsBelow из ресурса range и новые свойства таблицы. |

### <a name="intune-apis"></a>API Intune

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлены API ресурсов и методов для Microsoft Intune. Это большой набор ресурсов и методов для поддержки общедоступной предварительной версии Intune на портале Azure. Сведения о службе Intune см. в статье [Документация по Intune](https://go.microsoft.com/fwlink/?linkid=836405). Сведения о ресурсах и API Intune см. в разделе [Работа с Intune в Microsoft Graph](/graph/api/resources/intune-graph-overview?view=graph-rest-beta). |

## <a name="october-2016"></a>Октябрь 2016 г.

### <a name="authorization-provider"></a>Поставщик услуг авторизации

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Конечная точка авторизации 2.0 теперь поддерживает тип предоставления OAuth client_credentials, который можно использовать для [процессов управляющей программы и длительных процессов в бизнес-сценариях](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow). |
| Дополнение        | 1.0 и бета-версия | Конечная точка авторизации 2.0 теперь поддерживает [разрешения, требующие согласия администратора](permissions-reference.md) ([конечная точка предоставления согласия администратора](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#admin-restricted-permissions)). |
| Дополнение        | 1.0 и бета-версия | Конечная точка авторизации 2.0 теперь поддерживает согласие администратора для всех пользователей клиента ([конечная точка предоставления согласия администратора](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#admin-restricted-permissions)). |

### <a name="invitation-apis"></a>API приглашений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство invitedUserType к типу объекта приглашений, определяющее тип приглашаемого пользователя (**Guest** или **Member**). |
| Удаление        | Бета        | Мы удалим свойство invitedToGroups для типа объекта invitation 11 ноября 2016 г. Это значит, что вы больше не сможете добавить приглашаемого пользователя в группу с помощью этого API. Это можно будет сделать с помощью [API добавления членов](/graph/api/group-post-members?view=graph-rest-1.0). |

## <a name="september-2016"></a>Сентябрь 2016 г.

### <a name="azure-ad-application-proxy"></a>Прокси приложения Azure AD

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Теперь API Azure AD Application Proxy доступны в конечной точке Microsoft Graph бета-версии. Эти API позволяют безопасно публиковать локальные приложения для пользователей, находящихся за пределами корпоративной сети, используя Azure AD в качестве общей системы управления доступом. Опубликованные API позволяют создавать приложения, которые могут получать и обновлять различные аспекты прокси приложения, например параметры _connectors_, _connectorGroups_ и _onPremisesPublishing_ приложения. |

### <a name="drive"></a>Drive

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена коллекция _shared_, благодаря которой можно получать доступ к общим элементам driveItem с помощью идентификатора shareId или URL-адреса для совместного доступа. |
| Дополнение        | Бета-версия        | Добавлена функция _search_ к объекту drive, которая позволяет искать элементы не только в корневой папке диска. |


### <a name="driveitem"></a>DriveItem

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена поддержка элемента _createUploadSession_, который позволяет отправлять файлы размером более 4 МБ в OneDrive, OneDrive для бизнеса и библиотеки документов SharePoint. |
| Дополнение        | Бета-версия        | Добавлено свойство _sharepointIds_, которое возвращает традиционные идентификаторы API SharePoint для элементов driveItem, хранящихся в SharePoint. |
| Дополнение        | Бета-версия        | Добавлены дополнительные свойства для _remoteItem_. |
| Дополнение        | Бета-версия        | Добавлено значение _quickXorHash_ для файлов в OneDrive для бизнеса. |
| Дополнение        | Бета-версия        | Добавлена область для объекта _createSharingLink_, которая позволяет создавать ссылки для совместного доступа в компании или анонимного совместного доступа. |

### <a name="extended-properties"></a>Расширенные свойства

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Теперь [расширенные свойства](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) поддерживаются в следующих ресурсах: message, mailFolder, event, calendar, contact, contactFolder, group event, group calendar, group post. |

### <a name="groups"></a>Группы

Добавлена поддержка динамического членства в группах с помощью общедоступной ознакомительной версии API, включая дополнения, указанные в таблице ниже.

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство **membershipRule**, содержащее правила, которые определяют членов динамической группы. |
| Дополнение        | Бета-версия        | Добавленное свойство **membershipRuleProcessingState** определяет, включено ли динамическое членство для этой группы. |
| Дополнение        | Бета-версия        | Присвойте свойству **groupTypes** значение **DynamicMembership**, чтобы включить динамическое членство для этой группы. |
| Дополнение        | бета        | Добавлено свойство **preferredLanguage**, которое указывает предпочитаемый язык для группы Office 365. |
| Дополнение        | Бета-версия        | Добавлено свойство **theme**, которое позволяет указать цветовую тему группы Office 365. |

### <a name="hybrid-deployment-support"></a>Поддержка гибридного развертывания

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Приложения могут использовать API Почты, Календаря и Контактов Outlook версии 1.0 для доступа к локальным почтовым ящикам в гибридном развертывании Exchange 2016 с накопительным пакетом обновления 3 (CU3). Дополнительные сведения о поддержке REST API см. в разделах, посвященных соответствующему [гибридному развертыванию](hybrid-rest-support.md). **Примечание.** Если вы используете эти наборы API версии 1.0, то теперь ваши приложения (включая рабочие) будут работать с локальными почтовыми ящиками, которые соответствуют требованиям для гибридных развертываний. Доступна только предварительная версия этой возможности. |

### <a name="identityriskevents"></a>IdentityRiskEvents

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | В рамках изменения схемы, при котором тип двух свойств расположений будет заменен новым сложным типом в конечной точке identityRiskEvents, в конечной точке identityRiskEvents изменены или добавлены следующие свойства:</br>**location** теперь относится не к Edm.String, а к signInLocation ComplexType;<br/>**previousLocation** теперь относится не к Edm.String, а к signInLocation ComplexType;<br/>**signInLocation** — новый элемент ComplexType, содержащий свойства city, state, countryOrRegion и geoCoordinates;<br/>**geoCoordinates** — новый элемент ComplexType, содержащий свойства latitude и longitude. |

### <a name="invitation-manager"></a>Диспетчер приглашений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Теперь API диспетчера приглашений доступны в конечной точке Microsoft Graph бета-версии. С помощью API диспетчера приглашений вы можете создать приглашение для добавления внешнего пользователя в организацию. Кроме того, при приглашении пользователя вы можете добавить его в группу Office 365. Дополнительные сведения см. в статье [о диспетчере приглашений](/graph/api/resources/invitation?view=graph-rest-beta). |

### <a name="onedrive"></a>OneDrive

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен метод **CreateUploadSession** для **driveItem**, который позволяет отправлять большие файлы и возобновлять отправку. |
| Дополнение        | v1.0        | Добавлены свойства для отслеживания идентификаторов SharePoint в элементах из SharePoint (**sharepointIds**) и свойство для идентификации корневых папок (**root**). |
| Дополнение        | 1.0        | Добавлена корневая коллекция **Shares**, которую можно использовать с идентификаторами shareId или ссылками для совместного доступа к общим элементам в OneDrive и SharePoint. Возвращает новый тип — sharedDriveItem. |
| Дополнение        | 1.0        | Добавлен метод **Invite** для driveItem, который позволяет добавлять разрешения для элементов. |
| Дополнение        | 1.0        | Добавлен метод **Search** для drive, который позволяет искать элементы на диске, а также общие элементы. |
| Дополнение        | 1.0        | Добавлено свойство **processingMetadata** для свойства quickXorHash сложного типа hashes. |
| Дополнение        | 1.0        | Добавлено свойство **quickXorHash** к сложному типу hashes. |

### <a name="outlook-calendar"></a>Календарь Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлено свойство **onlineMeetingUrl** к ресурсу [event](/graph/api/resources/event?view=graph-rest-1.0). |
| Дополнение        | Бета-версия        | Добавлено действие [forward](/graph/api/event-forward?view=graph-rest-beta) к ресурсу event. |
| Дополнение        | Бета-версия        | К ресурсу [calendar](/graph/api/resources/calendar?view=graph-rest-beta) добавлены свойства, c помощью которых можно предоставлять общий доступ к календарю: **canEdit**, **canShare**, **canViewPrivateItems**, **isShared**, **isShareWithMe** и **owner**. |

### <a name="outlook-mail"></a>Почта Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен сложный тип [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0), который включает свойства **automaticRepliesSetting**, **timeZone** и **language**. |
| Дополнение        | 1.0        | Добавлено свойство **mailboxSettings** к ресурсу [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Дополнение        | Бета-версия        | Добавлена возможность создавать, отображать, получать и удалять один или несколько экземпляров объекта [mention](/graph/api/resources/mention?view=graph-rest-beta) в сообщении. С помощью объектов mention можно привлечь внимание других пользователей в сообщении. |
| Дополнение        | Бета-версия        | Добавлена поддержка действия [getMailTips](/graph/api/user-getmailtips?view=graph-rest-beta) для получения подсказок для определенных получателей. Добавлены следующие ресурсы: [automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-beta), [mailTips](/graph/api/resources/mailtips?view=graph-rest-beta), [mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-beta). |

### <a name="query-parameters"></a>Параметры запроса

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | С 26 сентября 2016 г. поддерживаются параметры запроса без префиксов $. Префикс $ в параметрах запроса не является обязательным. Дополнительные сведения см. в записи блога [Поддержка параметров запросов без префиксов $ в Microsoft Graph](https://dev.office.com/queryparametersinMicrosoftGraph). |

### <a name="sharepoint"></a>SharePoint

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Доступ к сайтам и спискам SharePoint [по идентификатору](/graph/api/list-get?view=graph-rest-beta) или [URL-адресу](/graph/api/baseitem-getbyurl?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Возможность [отображать, создавать, получать и удалять экземпляры объектов listItem](/graph/api/resources/listitem?view=graph-rest-beta). |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлено нередактируемое свойство **refreshTokensValidFromDateTime**, которое указывает дату и время начала действия токенов обновления или токенов сеанса. Все токены, выпущенные до этого времени, недействительны, а при попытке их использования потребуется повторный вход в систему. |
| Дополнение        | Бета-версия        | Добавлено свойство **showInAddressList**, указывающее, должен ли глобальный список адресов Outlook содержать этого пользователя. |
| Дополнение        | Бета-версия        | Добавлено служебное действие **invalidateAllRefreshTokens**, которое аннулирует все токены обновления и токены сеанса пользователя, выпущенные для приложений, сбрасывая значения свойства **refreshTokensValidFromDateTime** и указывая для него текущую дату и время. |


### <a name="webhooks"></a>Веб-перехватчики

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | В веб-перехватчики добавлены корневые элементы Drive в качестве ресурса, доступного для подписки. |

## <a name="august-2016"></a>Август 2016 г.

### <a name="contacts"></a>Контакты

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | В рамках изменения схемы, при котором удаляются несколько свойств и добавляются соответствующие коллекции в конечную точку contacts, в эту конечную точку добавлены следующие свойства: _Websites Collection(ComplexType: Website)_,_Phones Collection (ComplexType: Phone)_, _PostalAddress Collection(ComplexType: PhysicalAddress)_. Дополнительные сведения см. в записи блога [Предстоящие изменения API Контактов и Людей](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/). |
| Удаление        | Бета        | В рамках изменения схемы, при котором удаляются несколько свойств и добавляются соответствующие коллекции в конечную точку contacts, из этой конечной точки удалены следующие свойства: _BusinessHomePage_,_HomePhones_, _MobilePhone1_, _BusinessPhones_, _HomeAddress_, _BusinessAddress_, _OtherAddress_. Дополнительные сведения см. в записи блога [Предстоящие изменения API Контактов и Людей](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/). |

### <a name="excel-apis"></a>API Excel

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | REST API Excel стал общедоступным в Microsoft Graph. Теперь вы можете обеспечить глубокую и сложную интеграцию с книгами Excel в Office 365. Дополнительные сведения см. в записи блога [Настройка использования REST API для Excel в приложениях с помощью Microsoft Graph](https://developer.microsoft.com/office/blogs/power-your-apps-with-the-new-excel-rest-api/). |

### <a name="people"></a>Люди

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | Свойство _WebSite_ переименовано на _Websites_. Дополнительные сведения см. в записи [Предстоящие изменения API Контактов и Людей](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/). |

### <a name="privileged-identity-management"></a>Управление привилегированными пользователями (PIM)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Теперь REST API управления привилегированными пользователями доступны в конечной точке Microsoft Graph (бета-версия). [Управление привилегированными пользователями](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) обеспечивает активацию "точно в срок" для привилегированных ролей в организации Azure AD, например ролей глобального администратора, администратора выставления счетов и т. д. C помощью опубликованных API разработчики могут создавать приложения, которые получают и обновляют привилегированные роли и активируют роли для пользователей. Дополнительные сведения см. в статьях [Microsoft Graph: доступна бета-версия API для Azure AD Privileged Identity Management](https://developer.microsoft.com/office/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta/) и [Azure AD Privileged Identity Management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta). |

## <a name="july-2016"></a>Июль 2016 г.

### <a name="administrative-units"></a>Административные единицы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Представлен новый API Administrative Units (предварительная версия). Административные единицы позволяют организациям делить Azure Active Directory на подразделения и делегировать административные обязанности этим подразделениям. Подразделения могут представлять регионы, отделы, места возникновения затрат и т. д. Теперь ими можно управлять с помощью API Microsoft Graph. |

## <a name="june-2016"></a>Июнь 2016 г.

### <a name="identityriskevents"></a>IdentityRiskEvents

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|Представлен новый API IdentityRiskEvents (предварительная версия). Этот API работает в сочетании с защитой идентификации Azure Active Directory. Его можно использовать для запрашивания событий рисков, созданных функцией защиты идентификации. Дополнительные сведения см. в статье [Знакомство с предварительной версией нового API в Microsoft Graph: IdentityRiskEvents](https://developer.microsoft.com/office/blogs/identityriskevents-api-preview/).

### <a name="subscriptions"></a>Подписки

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Области, предназначенные только для приложений, теперь поддерживаются для подписок _mail_ и _contacts_. |

## <a name="may-2016"></a>Май 2016 г.

### <a name="calendar"></a>Календарь

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Существенные изменения|Бета|Изменения в API findMeetingTimes. Дополнительные сведения см. в записи блога [Обновление API findMeetingTimes в Microsoft Graph](https://dev.office.com/microsoft-graph-findmeetingtimes-api-update). Это изменение вступило в силу 19 мая 2016 г.

### <a name="contact"></a>Контакт

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен абстрактный тип _extensions_ для поддержки открытого типа openTypeExtension в OData версии 4. |

### <a name="directory"></a>Каталог

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Существенные изменения | Бета        | Свойство _settingTemplateId_ теперь называется _templateId_. Это изменение вступило в силу 19 мая 2016 г. |

### <a name="event"></a>Событие

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен абстрактный тип _extensions_ для поддержки открытого типа openTypeExtension в OData версии 4. |

### <a name="eventmessages"></a>EventMessages

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлены типы _inferenceClassification_ и _extensions_ к объекту _eventMessages_. |
| Дополнение        | Бета-версия        | Добавлено свойство _responseRequested_ к _eventMessageRequest_. |

### <a name="messages"></a>Сообщения

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлены типы _inferenceClassification_ и _extensions_ к объекту _message_. |
| Дополнение        | Бета-версия        | Добавлено свойство _wellknownname_ для объекта _contactFolder_. |

### <a name="post"></a>Запись

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен абстрактный тип _extensions_ для поддержки открытого типа openTypeExtension в OData версии 4. |

### <a name="user"></a>User

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен тип ресурса _inferenceClassification_. |
| Дополнение        | Бета-версия        | Добавлено свойство _timeZone_ к типу _mailboxsettings_.   |
| Дополнение        | Бета-версия        | Добавлен API _findMeetingTimes_ для объекта _user_.   |

## <a name="april-2016"></a>Апрель 2016 г.

### <a name="general"></a>Общие

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Теперь _Accept-Encoding:gzip_ может учитываться. |
| Дополнение        | v1.0          | Добавлена поддержка сегмента приведения для пути с указанием expand. Пример: "https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event". |
| Дополнение        | Бета          | Добавлена поддержка запроса PATCH для структурных свойств. Например: "PATCH /me/mailboxSettings" |
| Дополнение        | Бета          | Теперь Azure Active Directory используется в качестве резервного ресурса для запросов /beta/users/id/photo, когда приложению Outlook не удается обслужить запрос (например, когда у пользователя нет лицензии на почтовый ящик или у клиента нет подписки на Exchange Online). ПРИМЕЧАНИЕ. Этот резервный ресурс доступен и для запросов GET, и для запросов PATCH. |
| Дополнение        | Бета          | Добавлена поддержка сегмента приведения для пути с указанием expand. Пример: "https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event". |

### <a name="onedrive"></a>OneDrive

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Исправление             | v1.0        | Устранена неисправность, из-за которой при выполнении запросов createLink в OneDrive возникала ошибка 500: "Неподдерживаемый тип свойства расширения". |

## <a name="march-2016"></a>Март 2016 г.

### <a name="calendar"></a>Календарь

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_. |
| Дополнение        | Бета-версия        | Добавлено свойство _suggestionHint_ к _meetingTimeCandidate_. |
| Дополнение        | Бета-версия        | Добавлено свойство _locationUri_ к _location_. |
| Дополнение        | Бета-версия        | Добавлены свойства _type_ и _postOfficeBox_ к _physicalAddress_. |
| Изменение          | Бета-версия        | У метода _findMeetingTimes_ появился новый параметр _ReturnSuggestionHints_. |
| Изменение          | Бета-версия        | Метод _findMeetingTimes_ теперь возвращает коллекцию объектов _meetingTimeCandidate_. |

### <a name="drive"></a>Drive

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлена функция _recent_ для вывода списка элементов, которые недавно использовал пользователь, вошедший в систему. Этот список включает элементы, находящиеся на диске пользователя, а также элементы на других дисках, к которым у пользователя есть доступ. Пример: GET /me/drive/recent. |
| Дополнение        | 1.0 и бета-версия | Добавлена функция _sharedWithMe_ для вывода списка элементов, доступ к которым предоставлен текущему пользователю. Пример: GET /me/drive/sharedWithMe. |

### <a name="driveitem"></a>DriveItem

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлен тип _remoteItem_, который позволяет предоставить ссылку на элемент на другом диске. |
| Дополнение        | 1.0 и бета-версия | Добавлен тип _sharingInvitation_, который позволяет предоставить сведения о приглашении к совместному использованию, связанном с этим разрешением. |
| Дополнение        | 1.0 и бета-версия | Добавлена функция _delta_, чтобы отслеживать изменения элементов на диске. Пример: GET /me/drive/items/{item-id}/delta |
| Дополнение        | 1.0 и бета-версия | Добавлен метод _copy_, который создает копию _driveItem_ (в том числе всех дочерних элементов) в новом родительском элементе или с новым именем. Пример: POST /me/drive/items/{item-id}/copy |
| Дополнение        | 1.0 и бета-версия | Атрибуты экземпляра _conflictBehavior_ теперь можно применять к _driveItem_. |
|Дополнение|Бета|Добавлена функция _invite_, которая позволяет отправить приглашение к совместному использованию для существующего элемента. Приглашение к совместному использованию создает уникальную ссылку для совместного доступа и отправляет ее получателю приглашения. Пример: POST /drive/items/{item-id}/invite

### <a name="event"></a>Событие

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены новое свойство _onlineMeetingUrl_ и новый метод _cancel_. |

### <a name="event-messages"></a>Сообщения о событиях

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены свойства _startDateTime_, _endDateTime_, _location_, _type_, _recurrence_, _isOutOfDate_, _conversationIndex_, _unsubscribe_, _unsubscribeData_, _unsubscribeEnabled_ и _flag_ к объекту _eventmessage_. |
| Дополнение        | Бета-версия        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_. |
| Дополнение        | Бета-версия        | Добавлен новый метод _unsubscribe_.          |

### <a name="excel"></a>Excel

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Мы добавляем новые REST API Excel, которые позволяют считывать и изменять данные в рабочей книге Excel. Теперь вы можете создавать интеллектуальные приложения, с помощью которых пользователи смогут эффективно анализировать содержимое, хранящееся в рабочих книгах Excel. Используйте аналитические функции Excel, создавайте таблицы и визуально привлекательные диаграммы в своем приложении. Дополнительные сведения см. в статье [Работа с Excel в Microsoft Graph](/graph/api/resources/excel?view=graph-rest-beta). |

### <a name="general"></a>Общие

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Улучшено сообщение об ошибке при сопоставлении псевдонима клиента и отклоненных токенов JWT (AAD). |
| Дополнение        | 1.0 и бета-версия | Сведения о расположении конечной точки службы авторизации теперь возвращаются в заголовке _www-authenticate_ при получении запроса с пустым токеном носителя. |
| Дополнение        | 1.0 и бета-версия | Исправлена возможность фильтрации по свойству id объекта. Пример: GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>Ранее в запросах POST требовалось добавлять microsoft.graph перед именем функции или действия. Пример: POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups.<br/>Теперь не требуется указывать префикс (хотя его по-прежнему можно указывать). Такой запрос тоже возможен: POST https://graph.microsoft.com/v1.0/me/getMemberGroups. |
| Изменение          | Бета          | Удалены имена свойств подписок.  |
| Дополнение        | Бета          | Мы добавили возможность находить (с помощью _directorySettingTemplates_) и переопределять поведение по умолчанию (путем создания _setting_ на основе шаблона) для объектов и связанных с ними функций. Изначально для управления поведением групп Office использовался только этот шаблон. |

### <a name="mail-folder"></a>Папка почты

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены свойства _wellKnownName_ и _userConfigurations_. |
| Дополнение        | Бета-версия        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_. |

### <a name="messages"></a>Сообщения

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Добавлено свойство _mobilePhone_.            |
| Дополнение        | 1.0 и бета | Добавлено свойство _internetMessageId_. Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). |
| Изменение          | Бета-версия          | Свойство _mobilePhone1_ теперь называется _mobilePhone_. |
| Изменение          | бета          | У методов _createReply_ и _createReplyAll_ появились новые параметры — _Message_ и _comment_. |
| Изменение          | Бета-версия          | У метода _createForward_ появились новые параметры — _Message_, _ToRecipients_ и _comment_. |
| Изменение          | Бета-версия          | У методов _reply_, _replyAll_ и _forward_ появился новый параметр — _Message_. |

### <a name="permission"></a>Разрешение

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлено свойство _sharingInvitation_ для предоставления сведений о приглашении к совместному использованию, связанном с этим разрешением. |

### <a name="person"></a>Человек

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены новые свойства: _birthday_, _personNotes_, _isFavorite_, _phones_, _permission_, _postalAddresses_, _websites_, _yomiCompany_, _department_, _profession_, _mailboxType_ и _personType_. |
| Дополнение        | Бета-версия        | Добавлены новые типы перечислений: _physicalAddressType_, _webSite_, _phone_ и _webSiteType_. |

### <a name="reference-attachment"></a>Вложение в виде ссылки

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены новые свойства: _sourceUrl_, _providerType_, _thumbnailUrl_, _previewUrl_, _permission_ и _isFolder_. |
| Дополнение        | Бета-версия        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_. |
| Дополнение        | Бета-версия        | Добавлены новые типы перечислений — _referenceAttachmentProvider_ и _referenceAttachmentPermission_. |

### <a name="subscriptions"></a>Подписки

| **Тип изменения** | **Конечная точка** | **Описание**                          |
| :-------------- | :----------- | :--------------------------------------- |
| Дополнение        | 1.0         | Веб-перехватчики теперь доступны для ресурса _/Subscriptions_ в конечной точке версии 1.0. Создавайте, просматривайте, продлевайте и удаляйте подписки на уведомления о данных из чатов в Outlook и группах Office 365. |

### <a name="user"></a>Пользователь

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство _mailboxSettings_ и соответствующие типы. |

## <a name="february-2016"></a>Февраль 2016 г.

### <a name="driveitem"></a>DriveItem

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Новое свойство _remoteItem_ для driveItem для учетных записей Майкрософт. |

### <a name="general"></a>Общие

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Конструкция-_/me/drive_ теперь работает как для учетных записей Майкрософт, так и для рабочих и учебных учетных записей. |
| Изменение          | 1.0 и бета-версия | Запросы Drive для учетных записей, хранилища OneDrive которых подготовлены по запросу, работают более надежно и в большем количестве сценариев, где для используемых по умолчанию сайтов SharePoint клиента применяются нестандартные имена. |
| Удаление        | Бета          | Из бета-версии схемы удалены различные нереализованные типы для более точного соответствия схеме версии 1.0. |

### <a name="subscriptions"></a>Подписки

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Проверка notificationUrl на создание подписок. Дополнительные сведения см. в статье [Обновление веб-перехватчиков Microsoft Graph — январь 2016 г.](https://developer.microsoft.com/office/blogs/Microsoft-Graph-WebHooks-Update-January-2016/) |
| Дополнение        | Бета-версия        | Теперь можно удалять объекты подписки. Соответствующий запрос: DELETE https://graph.microsoft.com/beta/subscriptions/. |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Теперь для учетных записей Майкрософт возвращается _displayName_. |

## <a name="january-2016"></a>Январь 2016 г.

### <a name="contacts"></a>Контакты

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | В набор объектов личных контактов добавлено свойство mobilePhone. |

### <a name="directoryobjects"></a>directoryObjects

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Исправление             | 1.0 и бета-версия | Исправлены действия вызовов, привязанные к directoryObjects, при которых возникали сбои со следующим сообщением об ошибке:  Тип значения, возвращаемого в результате операции, невозможен для заданного набора объектов. Это относится к следующим действиям: _microsoft.graph.checkMemberObjects_, _microsoft.graph.getMemberObjects_, _microsoft.graph.checkMemberGroups_, _microsoft.graph.assignLicense_, _microsoft.graph.changePassword_. |

## <a name="december-2015"></a>Декабрь 2015 г.

### <a name="contacts"></a>Контакты

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | В набор объектов личных контактов добавлено свойство mobilePhone. |

### <a name="general"></a>Общие

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Исправление             | 1.0 и бета-версия | Исправлены запросы, в которых используются выражения $filter, указанные для одного и того же свойства несколько раз, при выполнении которых возникали сбои с кодом 500 и отображалось следующее сообщение об ошибке: "Элемент с тем же ключом уже был добавлен". |
| Исправление             | 1.0 и бета-версия | Исправлена ошибка, при которой не учитывался регистр имен и значений параметров действий. |
| Исправление             | 1.0 и бета-версия | Исправлена обработка запросов для полезных нагрузок, содержащих значения null для некоторых внедренных сложных свойств, при которых возникал сбой из-за ссылки на значение null. |
| Дополнение        | 1.0 и бета-версия | Добавлена возможность сортировать и фильтровать свойства сложных типов. |
| Дополнение        | 1.0 и бета-версия | Добавлено свойство authorization_uri в заголовок www-authenticate ответа 401. Вы можете использовать этот универсальный код ресурса для запуска потока получения токена. |
| Дополнение        | 1.0 и бета-версия | Улучшены сообщения об ошибках для пользователей и групп. |

### <a name="groups"></a>Группы

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Исправление             | 1.0 и бета-версия | Исправлен вызов следующих действий групп: _microsoft.graph.addFavorite_, _microsoft.graph.removeFavorite_ и _microsoft.graph.resetUnseenCount_. |

### <a name="messages"></a>Сообщения

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | К типу eventMessage добавлен подтип для свойств eventMessageRequest eventMessage, startDateTime, endDateTime, location, type, recurrence и isOutOfDate. |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Исправление             | 1.0 и бета | Исправлена возможность выбирать определенные свойства другого пользователя, когда на него ссылаются по имени участника-пользователя. Пример: https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe |
| Исправление             | 1.0 и бета-версия | Исправлен вызов функции _microsoft.graph.reminderView_, привязанной к пользователю, при котором возникал сбой и отображалось следующее сообщение об ошибке: "Не удалось найти свойство с именем businessPhones в типе Microsoft.OutlookServices.Reminder". |
| Исправление             | 1.0 и бета-версия | Устранена проблема, из-за которой при создании и обновлении пользователей (POST/PATCH /v1.0/users) возникала ошибка 400. |
