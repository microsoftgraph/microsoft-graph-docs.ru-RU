---
title: Журнал изменений Microsoft Graph
description: Этот журнал содержит сведения об изменениях Microsoft Graph, в том числе API Microsoft Graph для конечных точек версии 1.0 и бета-версии.
author: MSGraphDocsVteam
localization_priority: Priority
ms.openlocfilehash: f9901df5724cc701bcaab0138ab15fc20cf9c563
ms.sourcegitcommit: c25828c596b7e0939fa164a3d7754722943152c2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2019
ms.locfileid: "38756879"
---
# <a name="changelog-for-microsoft-graph"></a>Журнал изменений Microsoft Graph

Этот журнал содержит сведения об изменениях API Microsoft Graph, в том числе API Microsoft Graph для конечных точек версии 1.0 и бета-версии.

Дополнительные сведения об известных проблемах с API Microsoft Graph см. в статье [Известные проблемы](known-issues.md).

## <a name="november-2019"></a>Ноябрь 2019 г.

### <a name="calendar--place"></a>Календарь | Место

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение        | Бета  | Добавлена возможность [обновления помещения или списка помещений](/graph/api/resources/place-get?view=graph-rest-beta).|

### <a name="cloud-communications-calls-and-online-meetings"></a>Облачные коммуникации (звонки и собрания по сети)

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Изменение        | Бета-версия        | Изменен возвращаемый тип для методов [mute](/graph/api/call-mute?view=graph-rest-beta) и [mute participant](/graph/api/participant-mute?view=graph-rest-beta) с [commsOperation](/graph/api/resources/commsoperation?view=graph-rest-beta) на [muteParticipantOperation](/graph/api/resources/muteparticipantoperation?view=graph-rest-beta). | 
| Изменение        | Бета-версия        | Изменен возвращаемый тип для метода [unmute](/graph/api/call-unmute?view=graph-rest-beta) с [commsOperation](/graph/api/resources/commsoperation?view=graph-rest-beta) на [unmuteParticipantOperation](/graph/api/resources/unmuteparticipantoperation?view=graph-rest-beta). | 

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[complianceManagementPartner](/graph/api/resources/intune-onboarding-compliancemanagementpartner?view=graph-rest-beta)<br/>[macOSCustomAppConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomappconfiguration?view=graph-rest-beta)<br/>[macOSWiredNetworkConfiguration](/graph/api/resources/intune-deviceconfig-macoswirednetworkconfiguration?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[companyPortalBlockedAction](/graph/api/resources/intune-shared-companyportalblockedaction?view=graph-rest-beta)<br/>[complianceManagementPartnerAssignment](/graph/api/resources/intune-onboarding-compliancemanagementpartnerassignment?view=graph-rest-beta)<br/>[deviceManagementPartnerAssignment](/graph/api/resources/intune-onboarding-devicemanagementpartnerassignment?view=graph-rest-beta)<br/>[roleScopeTagInfo](/graph/api/resources/intune-auditing-rolescopetaginfo?view=graph-rest-beta)<br/>[rotateBitLockerKeysDeviceActionResult](/graph/api/resources/intune-devices-rotatebitlockerkeysdeviceactionresult?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[companyPortalAction](/graph/api/resources/intune-shared-companyportalaction?view=graph-rest-beta)<br/>[easServices](/graph/api/resources/intune-deviceconfig-easservices?view=graph-rest-beta)<br/>[managedBrowserType](/graph/api/resources/intune-mam-managedbrowsertype?view=graph-rest-beta)<br/>[wiredNetworkInterface](/graph/api/resources/intune-deviceconfig-wirednetworkinterface?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлено действие [updateDeviceProperties](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-updatedeviceproperties?view=graph-rest-beta) для объекта [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) |
|Дополнение|Бета|Добавлено действие [updateDefinitionValues](/graph/api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues?view=graph-rest-beta) для объекта [groupPolicyConfiguration](/graph/api/resources/intune-grouppolicy-grouppolicyconfiguration?view=graph-rest-beta) |
|Дополнение|Бета|Добавлено действие [getPolicyNonComplianceMetadata](/graph/api/intune-reporting-devicemanagementreports-getpolicynoncompliancemetadata?view=graph-rest-beta) для объекта [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) |
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**scopeTagInfo**<br/>|
|Удаление|Бета|Удалено действие [getDeviceNoncomplianceReports](/graph/api/intune-reporting-devicemanagementreports-getdevicenoncompliancereports?view=graph-rest-beta) из объекта [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) |
|Удаление|Бета|Удалено действие [getPolicyNoncomplianceReports](/graph/api/intune-reporting-devicemanagementreports-getpolicynoncompliancereports?view=graph-rest-beta) из объекта [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) |
|Изменение|Бета|Изменены следующие свойства объекта [androidDeviceOwnerCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androiddeviceownercertificateprofilebase?view=graph-rest-beta):<br/>свойство **subjectAlternativeNameType** преобразовано из требуемого в необязательное.<br/>|
|Дополнение|Бета|Добавлено свойство **googleAccountsBlocked** для объекта [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **keyboardsRestricted** и **approvedKeyboards** для объекта [androidManagedAppProtection](/graph/api/resources/intune-shared-androidmanagedappprotection?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **thirdPartyKeyboardsBlocked** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **roleScopeTagIds** для объекта [deviceCategory](/graph/api/resources/intune-shared-devicecategory?view=graph-rest-beta)|
|Удаление|Бета|Удалено свойство **orderBy** из объекта [deviceManagementExportJob](/graph/api/resources/intune-reporting-devicemanagementexportjob?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **groupsRequiringPartnerEnrollment** для объекта [deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **roleScopeTagIds** для объекта [groupPolicyConfiguration](/graph/api/resources/intune-grouppolicy-grouppolicyconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **companyPortalBlockedActions**, **showAzureADEnterpriseApps** и **showOfficeWebApps** для объекта [intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **easServices** и **easServicesUserOverrideEnabled** для объекта [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)|
|Удаление|Бета|Удалено свойство **siriDisableServerLogging** из объекта [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **thirdPartyKeyboardsBlocked** для объекта [iosManagedAppProtection](/graph/api/resources/intune-shared-iosmanagedappprotection?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **managedBrowser** для объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **ethernetMacAddress** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **displayName** для объекта [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство навигации **managedDeviceCertificateStates** для объекта [androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta)|
|Изменение|Бета|Изменен тип следующих свойств объекта [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta):<br/>вместо **assignments** из коллекции [deviceManagementScriptAssignment](/graph/api/resources/intune-devices-devicemanagementscriptassignment?view=graph-rest-beta) теперь используется коллекция [deviceHealthScriptAssignment](/graph/api/resources/intune-devices-devicehealthscriptassignment?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлено свойство навигации **complianceManagementPartners** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **userRoleScopeTags** для сложного типа [auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta)|
|Удаление|Бета|Удалено свойство **scopeTags** из сложного типа [auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta)|
|Изменение|Бета|Изменены следующие свойства сложного типа [credentialSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-credentialsinglesignonextension?view=graph-rest-beta):<br/>**teamIdentifier** больше не обязательно указывать<br/>|
|Дополнение|Бета|Добавлены свойства **companyPortalBlockedActions**, **showAzureADEnterpriseApps** и **showOfficeWebApps** для сложного типа [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta)|

### <a name="education"></a>Образование

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета | Добавлено свойство [classSettings](/graph/api/resources/teamclasssettings?view=graph-rest-beta) для ресурса [team](/graph/api/resources/team?view=graph-rest-beta), чтобы разрешить вызывающим получать параметры, относящиеся к ресурсу team типа Class.|

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение | 1.0 | Добавлен новый тип объекта: [application](/graph/api/resources/application?view=graph-rest-1.0).|
| Дополнение | 1.0 | Добавлены новые делегированные разрешения: [Application.Read.All](/graph/permissions-reference#application-resource-permissions), [Application.ReadWrite.All](/graph/permissions-reference#application-resource-permissions).|
| Дополнение | 1.0 | Добавлено новое разрешение приложений [Application.Read.All](/graph/permissions-reference#application-resource-permissions).|
| Дополнение | 1.0 | Добавлены новые разрешения приложений и делегированные разрешения  [GroupMember.Read.All](permissions-reference.md#group-permissions)  и  [GroupMember.ReadWrite.All](permissions-reference.md#group-permissions)  для получения и обновления ресурса  [group](/graph/api/resources/group?view=graph-rest-1.0) .
| Дополнение | 1.0 | Добавлено новое разрешение приложений [Group.Create](permissions-reference.md#group-permissions) для создания ресурса **group** .
| Дополнение | Бета-версия и версия 1.0 | Добавлено свойство **creationType** для ресурса [user](/graph/api/resources/user?view=graph-rest-1.0).|
| Дополнение | 1.0 | Добавлена операция [checkMemberObjects](/graph/api/device-checkmemberobjects?view=graph-rest-1.0) для ресурса [device](/graph/api/resources/device?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлена операция [checkMemberObjects](/graph/api/group-checkmemberobjects?view=graph-rest-1.0) для ресурса [group](/graph/api/resources/group?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлена операция [checkMemberObjects](/graph/api/user-checkmemberobjects?view=graph-rest-1.0) для ресурса [user](/graph/api/resources/user?view=graph-rest-1.0). |

### <a name="identity-and-access-information-protection"></a>Удостоверения и доступ (защита информации)

| **Тип изменения** | **Версия** | **Описание**              |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлено новое делегированное разрешение [ThreatAssessment.ReadWrite.All](permissions-reference.md#threat-assessment-permissions) и разрешение приложений [ThreatAssessment.Read.All](permissions-reference.md#threat-assessment-permissions) для чтения и записи запросов на оценку угроз |

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета | Добавлена поддержка делегированного разрешения [Mail.ReadBasic](/graph/permissions-reference#mail-permissions) и разрешения приложений [Mail.ReadBasic.All](/graph/permissions-reference#mail-permissions) для [создания](/graph/api/subscription-post-subscriptions?view=graph-rest-beta), [получения](/graph/api/subscription-get?view=graph-rest-beta), [обновления](/graph/api/subscription-update?view=graph-rest-beta) и [удаления](/graph/api/subscription-delete?view=graph-rest-beta) подписок на уведомления об изменении сообщения. |
| Дополнение | 1.0 | Добавлена поддержка делегированного разрешения Mail.ReadBasic и разрешения приложений Mail.ReadBasic.All для следующего:<br />- [Перечисление сообщений](/graph/api/user-list-messages?view=graph-rest-1.0)<br />- [Получение сообщения](/graph/api/message-get?view=graph-rest-1.0) <br />- [Перечисление папок почты](/graph/api/user-list-mailfolders?view=graph-rest-1.0)<br />- [Получение папки почты](/graph/api/mailfolder-get?view=graph-rest-1.0)<br />- [Перечисление дочерних папок](/graph/api/mailfolder-list-childfolders?view=graph-rest-1.0)<br />- [Перечисление сообщений в папке](/graph/api/mailfolder-list-childfolders?view=graph-rest-1.0)<br />- [Получение дельты сообщения](/graph/api/message-delta?view=graph-rest-1.0)<br />- [Получение дельты папки почты](/graph/api/mailfolder-delta?view=graph-rest-1.0) <br />- [Создание](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0), [получение](/graph/api/subscription-get?view=graph-rest-1.0), [обновление](/graph/api/subscription-update?view=graph-rest-1.0) и [удаление](/graph/api/subscription-delete?view=graph-rest-1.0) подписок на уведомления об изменениях сообщения|

### <a name="identity-and-access-azure-ad--conditional-access"></a>Удостоверение и доступ (Azure AD) | Условный доступ

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение | Бета | Добавлено разрешение уровня приложения Policy.Read.All для операций чтения в политиках условного доступа и именованных расположениях.|

### <a name="people-and-workplace-intelligence"></a>Люди и рабочая аналитика

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение | бета | Добавлен [API профилей](/graph/api/resources/profile?view=graph-rest-beta) и связанные с ним методы. |

### <a name="search"></a>Поиск

Теперь в Поиске (Майкрософт) доступен способ поиска и индексирования данных в Microsoft Graph.

| **Тип изменения** | **Версия** | **Описание**                              |
|:----------------|:------------|:---------------------------------------------|
| Дополнение        | Бета        | Добавлен [API Поиска (Майкрософт)](search-concept-overview.md), предоставляющий возможности [отправки запросов](/graph/api/search-query?view=graph-rest-beta) и [индексирования](/graph/api/resource/indexing-api-overview?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлено действие [query](/graph/api/search-query?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлены сложные типы [searchRequest](/graph/api/resource/searchrequest?view=graph-rest-beta), [searchQuery](/graph/api/resource/searchquery?view=graph-rest-beta), [searchQueryString](/graph/api/resource/searchquerystring?view=graph-rest-beta),[searchResponse](/graph/api/resource/searchresponse?view=graph-rest-beta), [searchHitsContainer](/graph/api/resource/searchhitscontainer?view=graph-rest-beta) и [searchHit](/graph/api/resource/searchhit?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлены объекты [externalConnection](/graph/api/resource/externalconnection?view=graph-rest-beta), [schema](/graph/api/resource/schema?view=graph-rest-beta), [externalItem](/graph/api/resource/externalitem?view=graph-rest-beta) и [externalFile](/graph/api/resource/externalfile?view=graph-rest-beta), а также методы, доступные в этих объектах. |

## <a name="october-2019"></a>Октябрь 2019 г.

### <a name="calendar"></a>Календарь

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета-версия | Добавлено свойство **allowNewTimeProposals** для объектов [event](/graph/api/resources/event?view=graph-rest-beta) и [eventMessageRequest](/graph/api/resources/eventmessagerequest?view=graph-rest-beta). |
| Дополнение | Бета-версия | Добавлен необязательный параметр **proposedNewTime** для методов [tentativelyAccept](/graph/api/event-tentativelyaccept?view=graph-rest-beta) и [decline](/graph/api/event-decline?view=graph-rest-beta) объекта **event**. |
| Дополнение | Бета-версия | Добавлен объект [eventMessageResponse](/graph/api/resources/eventmessageresponse?view=graph-rest-beta), основанный на объекте [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-beta) и дополнительно содержащий свойства **proposedNewTime** и **responseType**. |
| Дополнение | Бета-версия | Добавлено свойство **proposedNewTime** для сложного типа [attendee](/graph/api/resources/attendee?view=graph-rest-beta). |
|Дополнение | бета | Добавлен новый объект [calendarPermission](/graph/api/resources/calendarpermission?view=graph-rest-beta). |
|Дополнение | бета | Добавлены API [get](/graph/api/calendarpermission-get?view=graph-rest-beta), [update](/graph/api/calendarpermission-update?view=graph-rest-beta) и [delete](/graph/api/calendarpermission-delete?view=graph-rest-beta) для управления ресурсами [calendarPermission](/graph/api/resources/calendarpermission?view=graph-rest-beta) в объекте [calendar](/graph/api/resources/calendar?view=graph-rest-beta). |
|Дополнение | бета | Добавлен новый сложный тип [onlineMeetingInfo](/graph/api/resources/onlinemeetinginfo?view=graph-rest-beta). |
| Дополнение | бета | Добавлены свойства **isOnlineMeeting**, **onlineMeetingProvider** и **onlineMeeting** для объекта [event](/graph/api/resources/event?view=graph-rest-beta). **isOnlineMeeting** и **onlineMeetingProvider** — это необязательные параметры методов [create](/graph/api/user-post-events?view=graph-rest-beta) и [update](/graph/api/event-update?view=graph-rest-beta) объекта **event**. |
| Дополнение | бета | Добавлены свойства **defaultOnlineMeetingProviders** и **allowedOnlineMeetingProviders** для объекта [calendar](/graph/api/resources/calendar?view=graph-rest-beta). |
| Дополнение | бета | Добавлено свойство **isTallyingResponses** для объекта [calendar](/graph/api/resources/calendar?view=graph-rest-beta). |
| Дополнение | бета | Добавлено свойство **isRemovable** для объекта [calendar](/graph/api/resources/calendar?view=graph-rest-beta). |
| Дополнение | бета | Добавлено свойство **delegateMeetingMessageDeliveryOptions** для объекта [mailboxSettings](/graph/api/resources/mailboxSettings?view=graph-rest-beta). |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[deviceHealthScriptAssignment](/graph/api/resources/intune-devices-devicehealthscriptassignment?view=graph-rest-beta)<br/>[deviceHealthScriptDeviceState](/graph/api/resources/intune-devices-devicehealthscriptdevicestate?view=graph-rest-beta)<br/>[deviceHealthScriptRunSummary](/graph/api/resources/intune-devices-devicehealthscriptrunsummary?view=graph-rest-beta)<br/>[deviceManagementCachedReportConfiguration](/graph/api/resources/intune-reporting-devicemanagementcachedreportconfiguration?view=graph-rest-beta)<br/>[deviceManagementExportJob](/graph/api/resources/intune-reporting-devicemanagementexportjob?view=graph-rest-beta)<br/>[deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta)<br/>[deviceManagementReportSchedule](/graph/api/resources/intune-reporting-devicemanagementreportschedule?view=graph-rest-beta)<br/>[groupPolicyMigrationReport](/graph/api/resources/intune-gpanalyticsservice-grouppolicymigrationreport?view=graph-rest-beta)<br/>[groupPolicySettingMapping](/graph/api/resources/intune-gpanalyticsservice-grouppolicysettingmapping?view=graph-rest-beta)<br/>[macOSMicrosoftEdgeApp](/graph/api/resources/intune-apps-macosmicrosoftedgeapp?view=graph-rest-beta)<br/>[macOSPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-macospkcscertificateprofile?view=graph-rest-beta)<br/>[userExperienceAnalyticsDevicePerformance](/graph/api/resources/intune-devices-userexperienceanalyticsdeviceperformance?view=graph-rest-beta)<br/>[userExperienceAnalyticsDeviceStartupHistory](/graph/api/resources/intune-devices-userexperienceanalyticsdevicestartuphistory?view=graph-rest-beta)<br/>[userExperienceAnalyticsRegressionSummary](/graph/api/resources/intune-devices-userexperienceanalyticsregressionsummary?view=graph-rest-beta)<br/>[windowsDefenderApplicationControlSupplementalPolicy](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy?view=graph-rest-beta)<br/>[windowsDefenderApplicationControlSupplementalPolicyAssignment](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment?view=graph-rest-beta)<br/>[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus?view=graph-rest-beta)<br/>[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary?view=graph-rest-beta)<br/>[windowsMicrosoftEdgeApp](/graph/api/resources/intune-apps-windowsmicrosoftedgeapp?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[androidDeviceOwnerGlobalProxy](/graph/api/resources/intune-deviceconfig-androiddeviceownerglobalproxy?view=graph-rest-beta)<br/>[androidDeviceOwnerGlobalProxyAutoConfig](/graph/api/resources/intune-deviceconfig-androiddeviceownerglobalproxyautoconfig?view=graph-rest-beta)<br/>[androidDeviceOwnerGlobalProxyDirect](/graph/api/resources/intune-deviceconfig-androiddeviceownerglobalproxydirect?view=graph-rest-beta)<br/>[groupPolicyObjectFile](/graph/api/resources/intune-gpanalyticsservice-grouppolicyobjectfile?view=graph-rest-beta)<br/>[mobileAppInstallTimeSettings](/graph/api/resources/intune-shared-mobileappinstalltimesettings?view=graph-rest-beta)<br/>[scopeTagInfo](/graph/api/resources/intune-auditing-scopetaginfo?view=graph-rest-beta)<br/>[win32LobAppRestartSettings](/graph/api/resources/intune-shared-win32lobapprestartsettings?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[deviceManagementReportFileFormat](/graph/api/resources/intune-reporting-devicemanagementreportfileformat?view=graph-rest-beta)<br/>[deviceManagementReportStatus](/graph/api/resources/intune-reporting-devicemanagementreportstatus?view=graph-rest-beta)<br/>[deviceManagementScheduledReportRecurrence](/graph/api/resources/intune-reporting-devicemanagementscheduledreportrecurrence?view=graph-rest-beta)<br/>[diskType](/graph/api/resources/intune-devices-disktype?view=graph-rest-beta)<br/>[groupPolicyMigrationReadiness](/graph/api/resources/intune-gpanalyticsservice-grouppolicymigrationreadiness?view=graph-rest-beta)<br/>[groupPolicySettingScope](/graph/api/resources/intune-gpanalyticsservice-grouppolicysettingscope?view=graph-rest-beta)<br/>[groupPolicySettingType](/graph/api/resources/intune-gpanalyticsservice-grouppolicysettingtype?view=graph-rest-beta)<br/>[managedAppDeviceThreatLevel](/graph/api/resources/intune-mam-managedappdevicethreatlevel?view=graph-rest-beta)<br/>[microsoftEdgeChannel](/graph/api/resources/intune-apps-microsoftedgechannel?view=graph-rest-beta)<br/>[remediationState](/graph/api/resources/intune-devices-remediationstate?view=graph-rest-beta)<br/>[userExperienceAnalyticsSummarizedBy](/graph/api/resources/intune-devices-userexperienceanalyticssummarizedby?view=graph-rest-beta)<br/>[win32LobAppRestartBehavior](/graph/api/resources/intune-apps-win32lobapprestartbehavior?view=graph-rest-beta)<br/>[windowsDefenderApplicationControlSupplementalPolicyStatuses](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлено действие [approveApps](/graph/api/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-approveapps?view=graph-rest-beta) для ресурса [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [executeAction](/graph/api/api/intune-devices-manageddevice-executeaction?view=graph-rest-beta) для коллекции [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Дополнение|Бета|Добавлено действие [assign](/graph/api/intune-devices-devicehealthscript-assign?view=graph-rest-beta) для объекта [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [createMigrationReport](/graph/api/intune-gpanalyticsservice-grouppolicymigrationreport-createmigrationreport?view=graph-rest-beta) для коллекции [groupPolicyMigrationReport](/graph/api/resources/intune-gpanalyticsservice-grouppolicymigrationreport?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [getDeviceNoncomplianceReports](/graph/api/intune-reporting-devicemanagementreports-getdevicenoncompliancereports?view=graph-rest-beta) для объекта [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [getPolicyNoncomplianceReports](/graph/api/intune-reporting-devicemanagementreports-getpolicynoncompliancereports?view=graph-rest-beta) для объекта [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [getDeviceNonComplianceReport](/graph/api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport?view=graph-rest-beta) для объекта [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) |
|Дополнение|Бета|Добавлено действие [getPolicyNonComplianceReport](/graph/api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport?view=graph-rest-beta) для объекта [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [getHistoricalReport](/graph/api/intune-reporting-devicemanagementreports-gethistoricalreport?view=graph-rest-beta) для объекта [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [getCachedReport](/graph/api/intune-reporting-devicemanagementreports-getcachedreport?view=graph-rest-beta) для объекта [deviceManagementReports](/graph/api/resources/intune-reporting-devicemanagementreports?view=graph-rest-beta) |
|Дополнение|Бета|Добавлено действие [assign](/graph/api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-assign?view=graph-rest-beta) для объекта [windowsDefenderApplicationControlSupplementalPolicy](/graph/api/resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [summarizeDevicePerformanceDevices](/graph/api/intune-devices-userexperienceanalyticsdeviceperformance-summarizedeviceperformancedevices?view=graph-rest-beta) для коллекции [userExperienceAnalyticsDevicePerformance](/graph/api/resources/intune-devices-userexperienceanalyticsdeviceperformance?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [summarizeDeviceRegressionPerformance](/graph/api/intune-devices-userexperienceanalyticsregressionsummary-summarizedeviceregressionperformance?view=graph-rest-beta) для объекта [userExperienceAnalyticsRegressionSummary](/graph/api/resources/intune-devices-userexperienceanalyticsregressionsummary?view=graph-rest-beta) |
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**deviceHealthScriptComplianceRule**<br/>|
|Удаление|бета|Удалены следующие типы перечисления:<br/>**deviceHealthScriptComplianceRuleOperator**<br/>**deviceHealthScriptDetectionType**<br/>|
|Удаление|бета|Добавлено действие [executeAction](/graph/api/intune-devices-manageddevice-executeaction?view=graph-rest-beta) для коллекции [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Дополнение|бета|Добавлено свойство **globalProxy** для объекта [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **workProfileBlockPersonalAppInstallsFromUnknownSources** для объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **minimumRequiredCompanyPortalVersion**, **minimumWarningCompanyPortalVersion** и **minimumWipeCompanyPortalVersion** для объекта [androidManagedAppProtection](/graph/api/resources/intune-shared-androidmanagedappprotection?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **workProfileBlockPersonalAppInstallsFromUnknownSources** для объекта [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **remediation** для объекта [appVulnerabilityTask](/graph/api/resources/intune-partnerintegration-appvulnerabilitytask?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **minimumRequiredCompanyPortalVersion**, **minimumWarningCompanyPortalVersion** и **minimumWipeCompanyPortalVersion** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **configurationWebUrl** для объекта [depEnrollmentBaseProfile](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **source** и **sourceId** для объекта [deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **publisher**, **version**, **displayName**, **description**, **detectionScriptContent**, **createdDateTime**, **lastModifiedDateTime**, **runAsAccount**, **enforceSignatureCheck**, **runAs32Bit** и **roleScopeTagIds** для объекта [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **complianceRule** из объекта [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **groupPolicyObjectFiles** для объекта [deviceManagement](/graph/api/resources/intune-gpanalyticsservice-devicemanagement?view=graph-rest-beta)|
|Удаление|Бета|Удалено свойство **runSchedule** из объекта [deviceManagementScript](/graph/api/resources/intune-shared-devicemanagementscript?view=graph-rest-beta)|
|Удаление|Бета|Удалены свойства **lastSyncDateTime**, **preRemediationDetectionScriptOutput**, **remediationScriptError** и **postRemediationDetectionScriptOutput** из объекта [deviceManagementScriptDeviceState](/graph/api/resources/intune-devices-devicemanagementscriptdevicestate?view=graph-rest-beta)|
|Удаление|бета|Удалены свойства **compliantDeviceCount**, **notCompliantDeviceCount** и **pendingDeviceCount** из объекта [deviceManagementScriptRunSummary](/graph/api/resources/intune-devices-devicemanagementscriptrunsummary?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **platformType** для объекта [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **source** и **sourceId** для объекта [enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **mdmAppId** и **securityIdentifier** для объекта [group](/graph/api/resources/group?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **isDeleted** для объекта [importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **filesNetworkDriveAccessBlocked**, **filesUsbDriveAccessBlocked** и **wifiPowerOnForced** для объекта [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Удаление|Бета|Удалено свойство **wiFiBlockPowerModification** из объекта [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **previousPinBlockCount**, **maximumAllowedDeviceThreatLevel** и **mobileThreatDefenseRemediationAction** для объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **source** и **sourceId** для объекта [mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **androidMobileApplicationManagementEnabled** и **iosMobileApplicationManagementEnabled** для объекта [mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta)|
|Изменение|бета|Изменены следующие свойства объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta):<br/>**energySaverOnBatteryThresholdPercentage** преобразовано из обязательного в необязательное<br/>**energySaverPluggedInThresholdPercentage** преобразовано из обязательного в необязательное<br/>|
|Дополнение|бета|Добавлены свойства **source** и **sourceId** для объекта [windowsAutopilotDeploymentProfileAssignment](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofileassignment?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **filesFolder** для объекта [channel](/graph/api/resources/channel?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **wdacSupplementalPolicies** для объекта [deviceAppManagement](/graph/api/resources/intune-unlock-deviceappmanagement?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства навигации **assignments**, **runSummary** и **deviceRunStates** для объекта [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства навигации **deviceHealthScripts**, **userExperienceAnalyticsDevicePerformance**, **userExperienceAnalyticsRegressionSummary**, **userExperienceAnalyticsDeviceStartupHistory**, **groupPolicyMigrationReports** и **reports** для объекта [deviceManagement](/graph/api/resources/intune-devices-devicemanagement?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство навигации **singleSignOnExtensionPkinitCertificate** для объекта [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **singleSignOnExtensionPkinitCertificate** для объекта [macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **scopeTags** для сложного типа [auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **androidDedicatedCount**, **androidDeviceAdminCount**, **androidFullyManagedCount** и **androidWorkProfileCount** для сложного типа [deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **restartSettings** и **installTimeSettings** для сложного типа [win32LobAppAssignmentSettings](/graph/api/resources/intune-shared-win32lobappassignmentsettings?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **deviceRestartBehavior** для сложного типа [win32LobAppInstallExperience](/graph/api/resources/intune-apps-win32lobappinstallexperience?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **customPassword** для типа перечисления [androidDeviceOwnerRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype?view=graph-rest-beta)|
|Удаление|Бета|Удален элемент **appleUserEnrollmentWithAzureAD** из типа перечисления [deviceEnrollmentType](/graph/api/resources/intune-shared-deviceenrollmenttype?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены элементы **microsoftEdgeSecurityBaseline** и **microsoftOffice365ProPlusSecurityBaseline** для типа перечисления [deviceManagementTemplateType](/graph/api/resources/intune-deviceintent-devicemanagementtemplatetype?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **setDeviceName** для типа перечисления [managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены элементы **scriptError** и **notApplicable** для типа перечисления [runState](/graph/api/resources/intune-shared-runstate?view=graph-rest-beta)|
|Удаление|Бета|Удален элемент **error** из типа перечисления [runState](/graph/api/resources/intune-shared-runstate?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **userExperienceAnalytics** для типа перечисления [windowsHealthMonitoringScope](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringscope?view=graph-rest-beta)|

### <a name="education"></a>Образование

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Удаление | Бета | Удалены [объявленные ранее](https://developer.microsoft.com/onenote/blogs/breaking-change-education-api-updates-in-microsoft-graph-beta) устаревшие свойства **grade** и **feedback** из [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta). Доступ к оценкам и отзывам предоставляется только с помощью объекта [educationOutcome](/graph/api/educationsubmission-list-outcomes?view=graph-rest-beta).|

### <a name="groups"></a>Группы

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | Бета-версия          |Для управления видимостью группы в пользовательском интерфейсе Outlook в объект [группы](/graph/api/resources/group?view=graph-rest-beta) добавлены свойства**hideFromAddressLists** и **hideFromOutlookClients**.|
| Дополнение | Бета-версия | Добавлен метод [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta), который можно использовать для добавления и удаления лицензий для пользователей в [группе](/graph/api/resources/group?view=graph-rest-beta). |

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение | бета | Добавлены новые объекты: <br/>[authenticationDetail](/graph/api/authenticationDetail?view=graph-rest-beta)<br/>[keyValue](/graph/api/keyValue?view=graph-rest-beta)<br/>[networkLocationDetail](/graph/api/networkLocationDetail?view=graph-rest-beta)|
| Дополнение | бета | Добавлены свойства **alternateSignInName**, **ServicePrincipalId**, **ServicePrincipalName** и **authenticationProcessingDetails** ресурса [signIn](/graph/api/resources/signin?view=graph-rest-beta). |
| Удаление | бета | Ссылка на [mfaDetail](/graph/api/resources/mfadetail?view=graph-rest-beta) перемещена из [signIn](/graph/api/resources/signin?view=graph-rest-beta) в [authenticationDetail](/graph/api/authenticationDetail?view=graph-rest-beta). |
| Дополнение | бета | Добавлено свойство **signInActivity** для ресурса [user](/graph/api/resources/user?view=graph-rest-beta). |
| Дополнение | Бета-версия | Добавлен новый тип объекта: [Trustframeworkkeyset](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta) |
| Дополнение | бета | Добавлен новый тип объекта: [Identityuserflow](/graph/api/resources/identityuserflow?view=graph-rest-beta) |
| Дополнение | бета | Добавлены новые ресурсы для [управления правами](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta). |
| Дополнение | бета | Добавлен метод [removePassword](/graph/api/application-removepassword?view=graph-rest-beta) для ресурса [application](/graph/resources/application?view=graph-rest-beta). |
| Дополнение | бета | Добавлено свойство **addIns** для объекта [application](/graph/resources/application?view=graph-rest-beta). |
| Дополнение | бета | Добавлены методы [addPassword](/graph/api/serviceprincipal-addpassword?view=graph-rest-beta) и [removePassword](/graph/api/serviceprincipal-removepassword?view=graph-rest-beta) для ресурса [serviceprincipal](/graph/resources/serviceprincipal?view=graph-rest-beta). |
| Дополнение | Бета-версия и версия 1.0 | Добавлены свойства **onPremisesDomainName**, **onPremisesNetBiosName** и **onPremisesSamAccountName** для объекта [group](/graph/api/resources/group?view=graph-rest-1.0). |
| Дополнение | Бета-версия и версия 1.0 | Добавлено свойство **securityIdentifier** для ресурса [group](/graph/api/resources/group?view=graph-rest-1.0). |
| Дополнение | Бета-версия и версия 1.0 | Добавлено свойство **mdmAppId** для ресурса [device](/graph/api/resources/group?view=graph-rest-1.0). |
| Дополнение | Бета-версия и версия 1.0 | Добавлены свойства **manufacturer** и **model** для объекта [device](/graph/api/resources/device?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлен новый ресурс [orgContact](/graph/api/resources/orgcontact?view=graph-rest-1.0). Эти контакты управляются организацией и отличаются от [личных контактов](outlook-contacts-concept-overview.md)|
| Дополнение | 1.0 | Добавлен новый ресурс [physicalOfficeAddress](/graph/api/resources/physicalOfficeAddress?view=graph-rest-1.0). |
| Дополнение | Версия 1.0 | Добавлен новый объект [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлен новый сложный тип [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлено новое отношение для ресурса **certificateBasedAuthConfiguration** в ресурсе [organization](/graph/api/resources/organization?view=graph-rest-1.0). Это обеспечивает [проверку подлинности на основе сертификата в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).|

### <a name="identity-and-access-azure-ad--conditional-access"></a>Удостоверение и доступ (Azure AD) | Условный доступ

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение | бета | Добавлены новые типы объектов:<br/>[conditionalAccessPolicy](/graph/api/resources/conditionalAccessPolicy)<br/>
| Дополнение | бета | Добавлены новые сложные типы:<br/>[conditionalAccessSessionControl](/graph/api/resources/conditionalAccessSessionControl)<br/>[applicationEnforcedRestrictionsSessionControl](/graph/api/resources/applicationEnforcedRestrictionsSessionControl)<br/>[cloudAppSecuritySessionControl](/graph/api/resources/cloudAppSecuritySessionControl)<br/>[signInFrequencySessionControl](/graph/api/resources/signInFrequencySessionControl)<br/>[persistentBrowserSessionControl](/graph/api/resources/persistentBrowserSessionControl)<br/>[conditionalAccessSessionControls](/graph/api/resources/conditionalAccessSessionControls)<br/>[conditionalAccessApplications](/graph/api/resources/conditionalAccessApplications)<br/>[conditionalAccessUsers](/graph/api/resources/conditionalAccessUsers)<br/>[conditionalAccessPlatforms](/graph/api/resources/conditionalAccessPlatforms)<br/>[conditionalAccessLocations](/graph/api/resources/conditionalAccessLocations)<br/>[conditionalAccessDeviceStates](/graph/api/resources/conditionalAccessDeviceStates)<br/>[conditionalAccessConditionSet](/graph/api/resources/conditionalAccessConditionSet)<br/>[conditionalAccessGrantControls](/graph/api/resources/conditionalAccessGrantControls)<br/>|
| Дополнение | бета | Добавлен [API namedLocation](/graph/api/resources/namedLocation?view=graph-rest-beta), представляющий именованные расположения в функции условного доступа Azure AD. |

### <a name="identity-and-access--information-protection"></a>Удостоверения и доступ | Защита информации

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | Бета          | Имя объекта **detectedSensitiveContent** изменено на [classificationResult](/graph/api/resources/classificationresult?view=graph-rest-beta).  | 
| Удаление        | Бета          | Удалены свойства **displayName**, **uniqueCount** и **matches** объекта [classificationResult](/graph/api/resources/classificationresult?view=graph-rest-beta).  | 
| Изменение          | бета          | Свойство **id** объекта [classificationResult](/graph/api/resources/classificationresult?view=graph-rest-beta) заменено на **sensitiveTypeId**.   | 
| Изменение          | бета          | Свойство **confidence** объекта [classificationResult](/graph/api/resources/classificationresult?view=graph-rest-beta) заменено на **confidenceLevel**.   | 
| Дополнение        | Бета          | Добавлено свойство **count** для объекта [classificationResult](/graph/api/resources/classificationresult?view=graph-rest-beta).  | 
| Удаление        | Бета          | Удалено свойство **actionSource** объекта [labelingOptions](/graph/api/resources/labelingoptions?view=graph-rest-beta). | 
| Удаление        | Бета          | Удален объект **auditInfo**. | 
| Изменение          | бета          | Свойство **protectByDoNotForwardAction** заменено на [protectDoNotForwardAction](/graph/api/resources/protectdonotforwardaction?view=graph-rest-beta). | 
| Дополнение        | бета          | Добавлено свойство **alignment** для объекта [addContentHeaderAction](/graph/api/resources/addcontentheaderaction?view=graph-rest-beta). | 
| Изменение          | Бета          | Свойство **labelId** объекта [recommendLabelAction](/graph/api/resources/recommendedlabelaction?view=graph-rest-beta) заменено на **label**. |
| Изменение          | бета          | Свойство **classificationIds** объекта [recommendLabelAction](/graph/api/resources/recommendedlabelaction?view=graph-rest-beta) заменено на **responsibleSensitivityTypeIds**. |
| Дополнение        | Бета          | Добавлено свойство **actionSource** объекта [recommendLabelAction](/graph/api/resources/recommendedlabelaction?view=graph-rest-beta). |
| Изменение          | Бета          | Свойство **labelId** объекта [applyLabelAction](/graph/api/resources/applylabelaction?view=graph-rest-beta) заменено на **label**. |
| Изменение          | Бета          | Свойство **classificationIds** объекта [applyLabelAction](/graph/api/resources/applylabelaction?view=graph-rest-beta) заменено на **responsibleSensitivityTypeIds**. |
| Дополнение        | бета          | Добавлено свойство **actionSource** объекта [applyLabelAction](/graph/api/resources/applylabelaction?view=graph-rest-beta). |
| Изменение          | Бета          | Значение перечисления [contentFormat](/graph/api/resources/enums?view=graph-rest-beta) изменено с **file** на **default**. | 
| Удаление        | бета          | Удалено значение **mandatory** из перечисления [actionSource](/graph/api/resources/enums?view=graph-rest-beta)). |
| Изменение          | Бета          | Значение перечисления [actionSource](/graph/api/resources/enums?view=graph-rest-beta) изменено с **policyDefault** на **default**. |
| Удаление        | бета          | Удален объект **auditMetadataKey**. |
| Изменение          | Бета          | API **applyLabel** изменен на [evaluateApplication](/graph/api/informationprotectionlabel-evaluateapplication?view=graph-rest-beta). |
| Изменение          | Бета          | API **applyLabelFromClassification** изменен на [evaluateClassificationResults](/graph/api/informationprotectionlabel-evaluateclassificationresults?view=graph-rest-beta). |
| Изменение          | бета          | API **removeLabel** изменен на [evaluateRemoval](/graph/api/informationprotectionlabel-evaluateremoval?view=graph-rest-beta). |
| Удаление        | бета          | Удалено свойство **auditInfo** объекта [extractLabel](/graph/api/informationprotectionlabel-extractlabel?view=graph-rest-beta). |

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | Бета-версия          | [Добавление файловых вложений размером до 150 МБ](outlook-large-attachments.md) для экземпляра [сообщения](/graph/api/resources/message?view=graph-rest-beta). |
| Дополнение        | бета          | Сложный тип [attachmentItem](/graph/api/resources/attachmentitem?view=graph-rest-beta), действие [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-beta) для объекта [attachment](/graph/api/resources/attachment?view=graph-rest-beta) и перечисление **attachmentType**. |
| Изменение         | бета          | Применение существующего объекта [uploadSession](/graph/api/resources/uploadsession?view=graph-rest-beta), использовавшегося объектом [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta), расширено также для объекта **attachment**. |

### <a name="notifications"></a>Уведомления

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение      | бета          |Добавлен API [создания и отправки уведомлений](/graph/api/user-post-notifications?view=graph-rest-beta) для работы с определенными пользователями без управления маркерами "от имени". |
| Дополнение        | бета          | Добавлено свойство **targetPolicy** ресурса [notification](/graph/api/resources/projectrome-notification?view=graph-rest-beta) для обращения к конечным точкам в Интернете с помощью Web Push. |
| Дополнение      | бета          |  Добавлено свойство **fallbackPolicy** ресурса [notification](/graph/api/resources/projectrome-notification?view=graph-rest-beta), обеспечивающее гарантированную доставку в iOS для уведомлений высокого приоритета. |

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета-версия | Добавлены методы [Получение фотографии команды](/graph/api/team-get-photo?view=graph-rest-beta) и[Обновление фото команды](/graph/api/team-update-photo?view=graph-rest-beta). |
| Дополнение | Бета | Метод [Чтение изображений в сообщениях](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta) теперь поддерживает разрешения приложений. |

### <a name="users"></a>Пользователи
| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение | 1.0 | Добавлено новое свойство **lastPasswordChangeDateTime** для ресурса [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Дополнение | Бета | Добавлен [API user: reprocessLicenseAssignment](/graph/api-reference/beta/api/user-reprocesslicense?view=graph-rest-beta), с помощью которого можно переработать все групповые назначения лицензий для [пользователя](/graph/api/resources/user?view=graph-rest-beta). |

### <a name="users--outlook-settings"></a>Пользователи | Параметры Outlook

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение        | 1.0        | Свойства **dateFormat** и **timeFormat** к ресурсу [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0). Свойства представляют собой предпочитаемые пользователем форматы даты и времени.|

## <a name="september-2019"></a>Сентябрь 2019 г.

### <a name="calendar-mail-groups"></a>Календарь, почта, группы

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Добавлена возможность [получения необработанного содержимого вложенного файла или элемента](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment) для события, сообщения или записи группы. |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidDeviceOwnerScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile)<br/>[androidManagedStoreWebApp](/graph/api/resources/intune-apps-androidmanagedstorewebapp)<br/>[appleEnrollmentProfileAssignment](/graph/api/resources/intune-enrollment-appleenrollmentprofileassignment)<br/>[appleUserInitiatedEnrollmentProfile](/graph/api/resources/intune-enrollment-appleuserinitiatedenrollmentprofile)<br/>[deviceCompliancePolicyPolicySetItem](/graph/api/resources/intune-policyset-devicecompliancepolicypolicysetitem)<br/>[deviceConfigurationPolicySetItem](/graph/api/resources/intune-policyset-deviceconfigurationpolicysetitem)<br/>[deviceManagementAutopilotEvent](/graph/api/resources/intune-troubleshooting-devicemanagementautopilotevent)<br/>[deviceManagementScriptPolicySetItem](/graph/api/resources/intune-policyset-devicemanagementscriptpolicysetitem)<br/>[enrollmentRestrictionsConfigurationPolicySetItem](/graph/api/resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem)<br/>[iosLobAppProvisioningConfigurationPolicySetItem](/graph/api/resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem)<br/>[macManagedAppProtection](/graph/api/resources/intune-policyset-macmanagedappprotection)<br/>[managedAppProtectionPolicySetItem](/graph/api/resources/intune-policyset-managedappprotectionpolicysetitem)<br/>[managedDeviceMobileAppConfigurationPolicySetItem](/graph/api/resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem)<br/>[mdmWindowsInformationProtectionPolicyPolicySetItem](/graph/api/resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem)<br/>[mobileAppPolicySetItem](/graph/api/resources/intune-policyset-mobileapppolicysetitem)<br/>[policySet](/graph/api/resources/intune-policyset-policyset)<br/>[policySetAssignment](/graph/api/resources/intune-policyset-policysetassignment)<br/>[policySetItem](/graph/api/resources/intune-policyset-policysetitem)<br/>[targetedManagedAppConfigurationPolicySetItem](/graph/api/resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem)<br/>[windows10EnrollmentCompletionPageConfigurationPolicySetItem](/graph/api/resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem)<br/>[windowsAutopilotDeploymentProfilePolicySetItem](/graph/api/resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem)<br/>[windowsFeatureUpdateProfile](/graph/api/resources/intune-softwareupdate-windowsfeatureupdateprofile)<br/>[windowsFeatureUpdateProfileAssignment](/graph/api/resources/intune-softwareupdate-windowsfeatureupdateprofileassignment)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[appleOwnerTypeEnrollmentType](/graph/api/resources/intune-enrollment-appleownertypeenrollmenttype)<br/>[configurationManagerAction](/graph/api/resources/intune-devices-configurationmanageraction)<br/>[credentialSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-credentialsinglesignonextension)<br/>[hasPayloadLinkResultItem](/graph/api/resources/intune-policyset-haspayloadlinkresultitem)<br/>[iosKerberosSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-ioskerberossinglesignonextension)<br/>[kerberosSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-kerberossinglesignonextension)<br/>[keyBooleanValuePair](/graph/api/resources/intune-deviceconfig-keybooleanvaluepair)<br/>[keyIntegerValuePair](/graph/api/resources/intune-deviceconfig-keyintegervaluepair)<br/>[keyRealValuePair](/graph/api/resources/intune-deviceconfig-keyrealvaluepair)<br/>[keyStringValuePair](/graph/api/resources/intune-deviceconfig-keystringvaluepair)<br/>[keyTypedValuePair](/graph/api/resources/intune-deviceconfig-keytypedvaluepair)<br/>[macOSKerberosSingleSignOnExtension](/graph/api/resources/intune-deviceconfig-macoskerberossinglesignonextension)<br/>[singleSignOnExtension](/graph/api/resources/intune-deviceconfig-singlesignonextension)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[appleUserInitiatedEnrollmentType](/graph/api/resources/intune-enrollment-appleuserinitiatedenrollmenttype)<br/>[bitLockerRecoveryPasswordRotationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype)<br/>[configurationManagerActionType](/graph/api/resources/intune-devices-configurationmanageractiontype)<br/>[deviceAndAppManagementAssignmentSource](/graph/api/resources/intune-shared-deviceandappmanagementassignmentsource)<br/>[errorCode](/graph/api/resources/intune-policyset-errorcode)<br/>[logLevel](/graph/api/resources/intune-troubleshooting-loglevel)<br/>[policySetStatus](/graph/api/resources/intune-policyset-policysetstatus)<br/>[userExperienceAnalyticsHealthState](/graph/api/resources/intune-devices-userexperienceanalyticshealthstate)<br/>[userExperienceAnalyticsInsightSeverity](/graph/api/resources/intune-devices-userexperienceanalyticsinsightseverity)<br/>[windowsAutopilotDeploymentState](/graph/api/resources/intune-troubleshooting-windowsautopilotdeploymentstate)<br/>[windowsAutopilotEnrollmentType](/graph/api/resources/intune-troubleshooting-windowsautopilotenrollmenttype)<br/>|
|Дополнение|Бета-версия|Добавлено действие [update](/graph/api/intune-policyset-policyset-update.md) для объекта [policySet](/graph/api/resources/intune-policyset-policyset) |
|Дополнение|Бета|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-mobileapp-haspayloadlinks.md) для коллекции [mobileApp](/graph/api/resources/intune-apps-mobileapp) |
|Дополнение|Бета|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-targetedmanagedappconfiguration-haspayloadlinks.md) для коллекции [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration) |
|Дополнение|Бета|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-ioslobappprovisioningconfiguration-haspayloadlinks.md) для коллекции [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection) |
|Дополнение|Бета-версия|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-androidmanagedappprotection-haspayloadlinks.md) для коллекции [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection) |
|Дополнение|Бета|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-macmanagedappprotection-haspayloadlinks.md) для коллекции [macManagedAppProtection](/graph/api/resources/intune-policyset-macmanagedappprotection) |
|Дополнение|Бета|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-mdmwindowsinformationprotectionpolicy-haspayloadlinks.md) для коллекции [mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam-mdmwindowsinformationprotectionpolicy) |
|Дополнение|Бета|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-ioslobappprovisioningconfiguration-haspayloadlinks.md) для коллекции [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration) |
|Дополнение|Бета|Добавлено действие [getPolicySets](/graph/api/intune-policyset-policyset-getpolicysets.md) для коллекции [policySet](/graph/api/resources/intune-policyset-policyset) |
|Дополнение|Бета|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-devicemanagementscript-haspayloadlinks.md) для коллекции [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript) |
|Дополнение|Бета-версия|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-deviceconfiguration-haspayloadlinks.md) для коллекции [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration) |
|Дополнение|Бета|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-devicecompliancepolicy-haspayloadlinks.md) для коллекции [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy) |
|Дополнение|Бета|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-windowsautopilotdeploymentprofile-haspayloadlinks.md) для коллекции [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile) |
|Дополнение|Бета-версия|Добавлено действие [hasPayloadLinks](/graph/api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md) для коллекции [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration) |
|Дополнение|Бета|Добавлено действие [triggerConfigurationManagerAction](/graph/api/intune-devices-manageddevice-triggerconfigurationmanageraction.md) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice) |
|Дополнение|Бета|Добавлено действие [setPriority](/graph/api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md) для объекта [appleUserInitiatedEnrollmentProfile](/graph/api/resources/intune-enrollment-appleuserinitiatedenrollmentprofile) |
|Дополнение|Бета|Добавлено действие [assign](/graph/api/intune-softwareupdate-windowsfeatureupdateprofile-assign.md) для объекта [windowsFeatureUpdateProfile](/graph/api/resources/intune-softwareupdate-windowsfeatureupdateprofile) |
|Дополнение|Бета-версия|Добавлена функция [getExpiringVppTokenCount](o:getExpiringVppTokenCount:Collection(microsoft.graph.depOnboardingSetting)) для коллекции [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting) |
|Дополнение|Бета-версия|Добавлены свойства **deviceThreatProtectionEnabled**, **deviceThreatProtectionRequiredSecurityLevel**, **securityRequireSafetyNetAttestationBasicIntegrity** и **securityRequireSafetyNetAttestationCertifiedDevice** для объекта [androidDeviceOwnerCompliancePolicy](/graph/api/resources/intune-deviceconfig-androiddeviceownercompliancepolicy)|
|Дополнение|Бета|Добавлено свойство **workProfileAllowWidgets** для объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration)|
|Дополнение|Бета|Добавлены свойства **isPrivate** и **isSystemApp** для объекта [androidManagedStoreApp](/graph/api/resources/intune-apps-androidmanagedstoreapp)|
|Дополнение|Бета|Добавлено свойство **workProfileAllowWidgets** для объекта [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration)|
|Дополнение|Бета|Добавлено свойство **screenTimeScreenDisabled** для объекта [depEnrollmentBaseProfile](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile)|
|Дополнение|Бета|Добавлены свойства **appearanceScreenDisabled**, **expressLanguageScreenDisabled**, **preferredLanguageScreenDisabled**, **deviceToDeviceMigrationDisabled** и **welcomeScreenDisabled** для объекта [depIOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depiosenrollmentprofile)|
|Удаление|Бета|Удалено свойство **screenTimeScreenDisabled** из объекта [depIOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depiosenrollmentprofile)|
|Дополнение|Бета|Добавлены свойства **source** и **sourceId** для объекта [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment)|
|Удаление|Бета|Удалено свойство **runRemediationScript** из объекта [deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript)|
|Дополнение|Бета|Добавлено свойство **singleSignOnExtension** для объекта [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration)|
|Дополнение|Бета|Добавлены свойства **kioskModeEnableVoiceControl** и **kioskModeAllowVoiceControlModification** для объекта [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration)|
|Дополнение|Бета-версия|Добавлены свойства **associatedDomains** и **singleSignOnExtension** для объекта [macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration)|
|Дополнение|Бета|Добавлены свойства **source** и **sourceId** для объекта [targetedManagedAppPolicyAssignment](/graph/api/resources/intune-mam-targetedmanagedapppolicyassignment)|
|Дополнение|Бета|Добавлено свойство **roleScopeTagIds** для объекта [termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions)|
|Дополнение|Бета-версия|Добавлены свойства **isBuiltIn** и **createdDateTime** для объекта [userExperienceAnalyticsBaseline](/graph/api/resources/intune-devices-userexperienceanalyticsbaseline)|
|Удаление|Бета|Удалены свойства **overallScore** и **overallRegressionThreshold** из объекта [userExperienceAnalyticsBaseline](/graph/api/resources/intune-devices-userexperienceanalyticsbaseline)|
|Удаление|Бета|Удалены свойства **displayName** и **overallScore** из объекта [userExperienceAnalyticsCategory](/graph/api/resources/intune-devices-userexperienceanalyticscategory)|
|Удаление|Бета|Удалено свойство **displayName** из объекта [userExperienceAnalyticsMetric](/graph/api/resources/intune-devices-userexperienceanalyticsmetric)|
|Удаление|Бета|Удалены свойства **overallScore**, **deviceBootPerformanceOverallScore** и **bestPracticesOverallScore** из объекта [userExperienceAnalyticsOverview](/graph/api/resources/intune-devices-userexperienceanalyticsoverview)|
|Дополнение|Бета|Добавлены свойства **attackSurfaceReductionRules** и **bitLockerRecoveryPasswordRotation** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration)|
|Дополнение|Бета-версия|Добавлены свойства **trackInstallProgressForAutopilotOnly** и **disableUserStatusTrackingAfterFirstUser** для объекта [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration)|
|Дополнение|Бета|Добавлено свойство навигации **policySets** для объекта [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement)|
|Дополнение|Бета|Добавлены свойства навигации **appleUserInitiatedEnrollmentProfiles**, **autopilotEvents** и **windowsFeatureUpdateProfiles** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement)|
|Дополнение|Бета|Добавлено свойство **value** для сложного типа [insightValueDouble](/graph/api/resources/intune-devices-insightvaluedouble)|
|Дополнение|Бета|Добавлено свойство **value** для сложного типа [insightValueInt](/graph/api/resources/intune-devices-insightvalueint)|
|Дополнение|Бета|Добавлено свойство **v13_0** для сложного типа [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem)|
|Дополнение|Бета-версия|Добавлены свойства **v10_14** и **v10_15** для сложного типа [macOSMinimumOperatingSystem](/graph/api/resources/intune-apps-macosminimumoperatingsystem)|
|Дополнение|Бета|Добавлены свойства **values** и **severity** для сложного типа [userExperienceAnalyticsInsight](/graph/api/resources/intune-devices-userexperienceanalyticsinsight)|
|Удаление|Бета|Удалено свойство **value** из сложного типа [userExperienceAnalyticsInsight](/graph/api/resources/intune-devices-userexperienceanalyticsinsight)|
|Дополнение|Бета|Добавлены элементы **appleUserEnrollment**, **appleUserEnrollmentWithServiceAccount** и **appleUserEnrollmentWithAzureAD** для типа перечисления [deviceEnrollmentType](/graph/api/resources/intune-shared-deviceenrollmenttype)|
|Дополнение|Бета|Добавлен элемент **securityTemplate** для типа перечисления [deviceManagementTemplateType](/graph/api/resources/intune-deviceintent-devicemanagementtemplatetype)|
|Дополнение|Бета-версия|Добавлен элемент **rebootNow** для типа перечисления [managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction)|
|Дополнение|Бета-версия|Добавлен элемент **rotateBitLockerKeys** для типа перечисления [remoteAction](/graph/api/resources/intune-devices-remoteaction)|
| Дополнение | Бета-версия | Добавлена поддержка разрешений приложений для операций записи: DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementRBAC.ReadWrite.All, DeviceManagementServiceConfig.ReadWrite.All |
| Дополнение | 1.0 | Добавлено свойство **v13_0** для сложного типа [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem). |

### <a name="education"></a>Образование

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета | Добавлено новое свойство **closeDateTime** в [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta).|
| Изменение | Бета | В ресурсе [educationMakeCodeResource](/graph/api/resources/educationMakeCodeResource?view=graph-rest-beta) изменены названия свойств**mkcd** на**projectId** и**url** на**hostWebUrl**.|

### <a name="cloud-communications-calls-and-online-meetings"></a>Облачные коммуникации (звонки и собрания по сети)

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение        | Бета        | Добавлены API /коммуникаций/* для всех звонков и собраний по сети. Путь `/app` является устаревшим. В дальнейшем используйте путь `/communications`.|
| Удаление         | Бета        | Путь `/app` устарел.|
| Удаление        | Бета        | Удалены свойства **createdDateTime** и **lastActionDateTime** из ресурса [commsOperation](/graph/.api/resource/commsOperation?view=graph-rest-beta).|
| Удаление        | Бета        | Удалено свойство **meetingType** из ресурса [onlineMeeting](/graph/api/resources/onlineMeeting?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлено свойство **isBroadcast** для ресурса [onlineMeeting](/graph/api/resources/onlineMeeting?view=graph-rest-beta). |
| Изменение        | Бета-версия        | Свойство **resource** в ресурсе [commsNotification](/graph/api/resources/commsNotification?view=graph-rest-beta) переименовано на **resourceUrl**. |
| Изменение          | Бета        | В ресурсе [resultInfo](/graph/api/resources/resultInfo?view=graph-rest-beta) изменен тип свойств **code** и **subCode** со строчного на Int32. |
| Изменение        | Бета        | Свойство **subcode** в ресурсе [resultInfo](/graph/api/resources/resultInfo?view=graph-rest-beta) переименовано на **subCode**. | 

### <a name="files-onedrive-for-business-and-onedrive-personal"></a>Файлы (OneDrive для бизнеса и OneDrive персональный)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета-версия | Добавлены ресурсы [pendingOperations](/graph/api/resources/pendingOperations?view=graph-rest-beta) и [pendingContentUpdate](/graph/api/resources/pendingContentUpdate?view=graph-rest-beta). Ресурс **pendingOperations** применяется к ресурсу [driveItem](/graph/api/resources/driveItem?view=graph-rest-beta). |
| Дополнение | Бета-версия | Добавлено действие [restore](/graph/api/driveitem-restore?view=graph-rest-beta) для ресурса [driveItem](/graph/api/resources/driveItem?view=graph-rest-beta). |
| Дополнение | Бета-версия | Добавлено свойство **orientation** для ресурса [photo](/graph/api/resources/photo?view=graph-rest-beta). |
| Дополнение | Бета-версия | Добавлено свойство **sha256Hash** для ресурса [hashes](/graph/api/resources/hashes?view=graph-rest-beta). |

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение | Бета-версия | Добавлен ресурс [objectIdentity](/graph/api/resources/objectIdentity?view=graph-rest-beta), представляющий удостоверение, использованное для входа в учетную запись пользователя. |
| Дополнение | Бета-версия | Добавлено свойство **synchronizationJobSettings** для ресурса [synchronizationJob](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta).|
| Дополнение | Бета-версия | Добавлены новые возможные значения для свойства **reason** в ресурсе [synchronizationQuarantine](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta).|
| Дополнение | Бета-версия | Добавлена возможность управления паролем единого входа для [объекта servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta). |

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Добавлена возможность [получения содержимого MIME сообщения](outlook-get-mime-message.md). |

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |Бета| Добавлено свойство **primaryChannel** для ресурса [team](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |Бета| Добавлено свойство **allowCreatePrivateChannels** для ресурса [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-beta).|

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета-версия | Добавлено свойство **identities** для ресурса [user](/graph/api/resources/user?view=graph-rest-beta). Это свойство представляет набор удостоверений, которые пользователь может использовать для входа.|
| Дополнение        | 1.0          | Добавлен метод [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-1.0).|

### <a name="users--outlook-settings"></a>Пользователи | Параметры Outlook

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение        | бета        | Свойства **dateFormat** и **timeFormat** к ресурсу [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta). Свойства представляют собой предпочитаемые пользователем форматы даты и времени.|

## <a name="august-2019"></a>Август 2019 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidDeviceOwnerCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androiddeviceownercertificateprofilebase?view=graph-rest-beta)<br/>[androidDeviceOwnerEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidDeviceOwnerTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate?view=graph-rest-beta)<br/>[androidDeviceOwnerVpnConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownervpnconfiguration?view=graph-rest-beta)<br/>[deviceHealthScript](/graph/api/resources/intune-devices-devicehealthscript?view=graph-rest-beta)<br/>[userExperienceAnalyticsBaseline](/graph/api/resources/intune-devices-userexperienceanalyticsbaseline?view=graph-rest-beta)<br/>[userExperienceAnalyticsCategory](/graph/api/resources/intune-devices-userexperienceanalyticscategory?view=graph-rest-beta)<br/>[userExperienceAnalyticsMetric](/graph/api/resources/intune-devices-userexperienceanalyticsmetric?view=graph-rest-beta)<br/>[userExperienceAnalyticsOverview](/graph/api/resources/intune-devices-userexperienceanalyticsoverview?view=graph-rest-beta)<br/>[vpnConfiguration](/graph/api/resources/intune-deviceconfig-vpnconfiguration?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[configurationManagerClientInformation](/graph/api/resources/intune-devices-configurationmanagerclientinformation?view=graph-rest-beta)<br/>[deviceHealthScriptComplianceRule](/graph/api/resources/intune-devices-devicehealthscriptcompliancerule?view=graph-rest-beta)<br/>[insightValueDouble](/graph/api/resources/intune-devices-insightvaluedouble?view=graph-rest-beta)<br/>[insightValueInt](/graph/api/resources/intune-devices-insightvalueint?view=graph-rest-beta)<br/>[userExperienceAnalyticsInsight](/graph/api/resources/intune-devices-userexperienceanalyticsinsight?view=graph-rest-beta)<br/>[userExperienceAnalyticsInsightValue](/graph/api/resources/intune-devices-userexperienceanalyticsinsightvalue?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[androidDeviceOwnerVirtualHomeButtonType](/graph/api/resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype?view=graph-rest-beta)<br/>[deviceHealthScriptComplianceRuleOperator](/graph/api/resources/intune-devices-devicehealthscriptcomplianceruleoperator?view=graph-rest-beta)<br/>[deviceHealthScriptDetectionType](/graph/api/resources/intune-devices-devicehealthscriptdetectiontype?view=graph-rest-beta)<br/>[powerActionType](/graph/api/resources/intune-deviceconfig-poweractiontype?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлено действие [enableAndroidDeviceAdministratorEnrollment](/graph/api/intune-deviceconfig-devicemanagement-enableandroiddeviceadministratorenrollment?view=graph-rest-beta) для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие executeAction для коллекции [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено действие [sendCustomNotificationToCompanyPortal](/graph/api/intune-devices-manageddevice-sendcustomnotificationtocompanyportal?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Удаление|бета|Добавлено действие executeAction для коллекции [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Дополнение|Бета|Добавлено свойство **roleScopeTagIds** для объекта [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta)|
|Удаление|Бета|Удалено свойство **scopeTags** из объекта [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **kioskModeScreenSaverConfigurationEnabled**, **kioskModeScreenSaverImageUrl**, **kioskModeScreenSaverDisplayTimeInSeconds**, **kioskModeScreenSaverStartDelayInSeconds**, **kioskModeScreenSaverDetectMediaDisabled**, **kioskModeVirtualHomeButtonType**, **kioskModeFlashlightConfigurationEnabled** и **kioskModeMediaVolumeConfigurationEnabled** для объекта [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **lastSyncDateTime**, **preRemediationDetectionScriptOutput**, **remediationScriptError** и **postRemediationDetectionScriptOutput** для объекта [deviceManagementScriptDeviceState](/graph/api/resources/intune-devices-devicemanagementscriptdevicestate?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **compliantDeviceCount**, **notCompliantDeviceCount** и **pendingDeviceCount** для объекта [deviceManagementScriptRunSummary](/graph/api/resources/intune-devices-devicemanagementscriptrunsummary?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **isRemoveDeviceDisabled** и **isFactoryResetDisabled** для объекта [intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **continuousPathKeyboardBlocked**, **findMyDeviceInFindMyAppBlocked**, **findMyFriendsInFindMyAppBlocked**, **wiFiBlockPowerModification** и **iTunesBlocked** для объекта [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **iCloudBlockActivityContinuation** для объекта [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **configurationManagerClientInformation** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **managedDeviceId** для объекта [remoteActionAudit](/graph/api/resources/intune-devices-remoteactionaudit?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **isBuiltIn** для объекта [roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta)|
|Удаление|Бета|Удалено свойство **userRightsRegisterProcessAsService** из объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **energySaverOnBatteryThresholdPercentage**, **energySaverPluggedInThresholdPercentage**, **powerLidCloseActionOnBattery**, **powerLidCloseActionPluggedIn**, **powerButtonActionOnBattery**, **powerButtonActionPluggedIn**, **powerSleepButtonActionOnBattery**, **powerSleepButtonActionPluggedIn**, **powerHybridSleepOnBattery** и **powerHybridSleepPluggedIn** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **deadlineForFeatureUpdatesInDays**, **deadlineForQualityUpdatesInDays**, **deadlineGracePeriodInDays** и **postponeRebootUntilAfterDeadline** для объекта [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства навигации **userExperienceAnalyticsOverview**, **userExperienceAnalyticsBaselines** и **userExperienceAnalyticsCategories** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Удаление|Бета|Удалено свойство навигации **healthSummary** из объекта [windowsManagementApp](/graph/api/resources/intune-devices-windowsmanagementapp?view=graph-rest-beta)||Дополнение|Бета|Добавлено свойство **shareUserExperienceAnalyticsData** для сложного типа [adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **osBuildNumber** для сложного типа [hardwareInformation](/graph/api/resources/intune-devices-hardwareinformation?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **isRemoveDeviceDisabled** и **isFactoryResetDisabled** для сложного типа [intuneBrandingProfile](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **uninstallOnDeviceRemoval** для сложного типа [iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **uninstallOnDeviceRemoval** для сложного типа [iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **uninstallOnDeviceRemoval** для сложного типа [iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **customTextNotification** для типа перечисления [managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **setDeviceName** для типа перечисления [remoteAction](/graph/api/resources/intune-devices-remoteaction?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены элементы **error** и **pending** для типа перечисления [runState](/graph/api/resources/intune-shared-runstate?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **noScheduledScan** для типа перечисления [weeklySchedule](/graph/api/resources/intune-deviceconfig-weeklyschedule?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство навигации **derivedCredentials** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement)|

### <a name="education"></a>Образование

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета-версия | Добавлено новое свойство **grade** для объекта [educationClass](/graph/api/resources/educationClass?view=graph-rest-beta).|
| Дополнение | Бета | Добавлен новый ресурс [educationRubric](/graph/api/resources/educationRubric?view=graph-rest-beta).|
| Дополнение | Бета | Добавлены API для управления ресурсами [educationRubric](/graph/api/resources/educationRubric?view=graph-rest-beta) в [educationUser](/graph/api/resources/educationUser?view=graph-rest-beta) и [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta).|
| Дополнение | Бета | Добавлен новый ресурс [educationOutcome](/graph/api/resources/educationOutcome?view=graph-rest-beta).|
| Дополнение | Бета | Добавлены API для управления ресурсами [educationOutcome](/graph/api/resources/educationOutcome?view=graph-rest-beta) в [educationSubmission](/graph/api/resources/educationSubmission?view=graph-rest-beta).|
| Дополнение | Бета | Добавлен новый ресурс [educationMakeCodeResource](/graph/api/resources/educationMakeCodeResource?view=graph-rest-beta).|
| Дополнение    | Бета-версия    | Добавлено новое свойство **grade** для объекта [educationClass](/graph/api/resources/educationClass?view=graph-rest-beta). |

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлено действие [unfollow](/graph/api/driveitem-unfollow?view=graph-rest-beta) для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Изменение | Бета-версия | Изменено пространство имен [перечисления provisioningObjectSummary](/graph/api/resources/provisioning-object-summary-list?view=graph-rest-beta).|
| Дополнение | Бета-версия | Добавлен ресурс [roleManagement](/graph/api/resources/roleManagement?view=graph-rest-beta), обеспечивающий доступ к определениям ролей и назначениям ролей, полученным от поставщиков RBAC. |
| Дополнение | Бета-версия | Добавлен ресурс [unifiedRoleDefinition](/graph/api/resources/unifiedRoleDefinition?view=graph-rest-beta), представляющий коллекцию разрешений с перечислением допустимых операций. |
| Дополнение | Бета-версия | Добавлен ресурс [unifiedRoleAssignment](/graph/api/resources/unifiedRoleAssignment?view=graph-rest-beta), предоставляющий доступ к ресурсам. |
| Дополнение | Бета-версия | Добавлены следующие операции для поддержки ресурса unifiedRoleDefinition: <br><ul><li>[Список объектов unifiedRoleDefinition](/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta) — получение списка объектов unifiedRoleDefinition для поставщика.</li><li>[Создание объекта unifiedRoleDefinition](/graph/api/rbacapplication-post-roledefinitions?view=graph-rest-beta) — создание объекта unifiedRoleDefinition.</li><li>[Получение объекта unifiedRoleDefinition](/graph/api/unifiedroledefinition-get?view=graph-rest-beta) — извлечение свойств и связей объекта определения единой роли.</li><li>[Обновление объекта unifiedRoleDefinition](/graph/api/unifiedroledefinition-update?view=graph-rest-beta) — обновление свойств объекта unifiedRoleDefinition.</li><li>[Удаление объекта unifiedRoleDefinition](/graph/api/unifiedroledefinition-delete?view=graph-rest-beta) — удаление объекта unifiedRoleDefinition.</li></ul> |
| Дополнение | Бета-версия | Добавлены следующие операции для поддержки ресурса unifiedRoleAssignment: <br><ul><li>[Список объектов unifiedRoleAssignment](/graph/api/rbacapplication-list-roleassignments?view=graph-rest-beta) — получение списка объектов unifiedRoleAssignment для поставщика.</li><li>[Создание объекта unifiedRoleAssignment]() — создание объекта unifiedRoleAssignment.</li><li>[Получение объекта unifiedRoleAssignment](/graph/api/unifiedroleassignment-get?view=graph-rest-beta) — извлечение свойств и связей объекта unifiedRoleAssignment.</li><li>[Удаление объекта unifiedRoleAssignment](/graph/api/unifiedroleassignment-delete?view=graph-rest-beta) — удаление объекта unifiedRoleAssignment. |
| Дополнение | бета | Добавлена операция [Список объектов accessReviews](/graph/api/accessreview-list?view=graph-rest-beta). |
| Дополнение | Бета | Добавлена операция [checkMemberObjects](/graph/api/device-checkmemberobjects?view=graph-rest-beta) для ресурса [device](/graph/api/resources/device?view=graph-rest-beta). |
| Дополнение | бета | Добавлена операция [checkMemberObjects](/graph/api/directoryobject-checkmemberobjects?view=graph-rest-beta) для ресурса [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta). |
| Дополнение | бета | Добавлена операция [checkMemberObjects](/graph/api/directoryrole-checkmemberobjects?view=graph-rest-beta) для ресурса [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-beta). |
| Дополнение | бета | Добавлена операция [checkMemberObjects](/graph/api/group-checkmemberobjects?view=graph-rest-beta) для ресурса [group](/graph/api/resources/group?view=graph-rest-beta). |
| Дополнение | Бета | Добавлена операция [checkMemberObjects](/graph/api/serviceprincipal-checkmemberobjects?view=graph-rest-beta) для ресурса [servicePrincipal](/graph/api/resources/serviceprinciple?view=graph-rest-beta). |
| Дополнение | Бета-версия | Добавлена операция [checkMemberObjects](/graph/api/user-checkmemberobjects?view=graph-rest-beta) для ресурса[user](/graph/api/resources/user?view=graph-rest-beta). |
| Дополнение | Бета | Добавлены делегированные разрешения и [разрешения приложения для чтения контактов организации](permissions-reference.md#organizational-contact-permissions): OrgContact.Read.All |
| Дополнение | Бета | Добавлен новый объект [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration?view=graph-rest-beta). |
| Дополнение | Бета | Добавлен новый сложный тип [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-beta). |
| Дополнение | Бета | Добавлено новое отношение для ресурса **certificateBasedAuthConfiguration** в ресурсе [organization](/graph/api/resources/organization?view=graph-rest-beta). Это обеспечивает [аутентификацию на основе сертификата в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)|

### <a name="reports"></a>Отчеты

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение        | 1.0  | Добавлены свойства **deletedItemCount** и **deletedItemSizeInBytes** для объекта [mailboxUsageDetail](/graph/api/resources/mailboxUsageDetail?view=graph-rest-beta).|
| Дополнение        | 1.0  | Добавлено свойство **groupId** для объекта [office365GroupsActivityDetail](/graph/api/resources/office365GroupsActivityDetail?view=graph-rest-beta).|
| Дополнение        | 1.0  | Добавлено свойство **ownerPrincipalName** для объекта [oneDriveUsageAccountDetail](/graph/api/resources/oneDriveUsageAccountDetail?view=graph-rest-beta).|
| Дополнение        | 1.0  | Добавлено свойство **ownerPrincipalName** для объекта [sharePointSiteUsageDetail](/graph/api/resources/sharePointSiteUsageDetail?view=graph-rest-beta).|
| Дополнение        | 1.0  | Добавлены свойства **office365Active** и **office365Inactive** для объекта [office365ServicesUserCounts](/graph/api/resources/office365ServicesUserCounts?view=graph-rest-beta).|

### <a name="social-and-workplace-intelligence"></a>Социальная и рабочая аналитика

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение | Бета-версия | Представлен новый [API аналитики](/graph/api/resources/useranalytics?view=graph-rest-beta) для рабочих сведений, позволяющий получить аналитику о том, как пользователи тратят свое время на различные действия во время и вне работы, включая звонки, чаты (мгновенные сообщения) письма, сосредоточенную работу и собрания. |
| Дополнение | Бета-версия | Представлен новый [API параметров](/graph/api/resources/settings?view=graph-rest-beta) для рабочих сведений, представляющий текущие обязательные параметры для применения пользователем [API аналитики](/graph/api/resources/useranalytics?view=graph-rest-beta). |
| Дополнение | Бета-версия | Представлен новый тип ресурса [activityStatistics](/graph/api/resources/activitystatistics?view=graph-rest-beta) и следующие новые типы ресурсов, полученные из него: [callActivityStatistics](/graph/api/resources/callactivitystatistics?view=graph-rest-beta), [chatActivityStatistics](/graph/api/resources/chatactivitystatistics?view=graph-rest-beta),[emailActivityStatistics](/graph/api/resources/emailactivitystatistics?view=graph-rest-beta), [focusActivityStatistics](/graph/api/resources/focusactivitystatistics?view=graph-rest-beta) и [meetingActivityStatistics](/graph/api/resources/meetingactivitystatistics?view=graph-rest-beta). |

### <a name="tasks-and-plans-planner"></a>Задачи и планы (Планировщик)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлено свойство **priority** для объекта [plannerTask](/graph/api/resources/plannertask?view=graph-rest-beta).|

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета | Добавлена возможность извлечения добавочных сообщений из каналов с помощью [API запросов изменений в сообщениях канала](/graph/api/channel-messages-delta?view=graph-rest-beta).|
| Дополнение | Бета-версия | Добавлена возможность [добавления участников в закрытый канал](/graph/api/conversationmember-add?view=graph-rest-beta). |
| Дополнение | бета | Добавлена возможность [удаления участников из закрытого канала](/graph/api/conversationmember-delete?view=graph-rest-beta). |
| Дополнение | бета | Добавлена возможность [обновления роли участника в закрытом канале](/graph/api/conversationmember-update?view=graph-rest-beta). |
| Дополнение | Бета | Добавлено свойство `membershipType` для ресурса [channel](/graph/api/resources/channel?view=graph-rest-beta), чтобы демонстрировать, является ли конкретный канал закрытым или стандартным. |

## <a name="july-2019"></a>Июль 2019 г.

### <a name="calendar--place"></a>Календарь | Место

Дебютный выпуск API мест, представляющего в приложениях подробные сведения о расположениях.

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение        | Бета-версия  | Добавлен ресурс [room list](/graph/api/resources/roomlist?view=graph-rest-beta)|
| Дополнение        | Бета-версия  | Добавлен ресурс [room](/graph/api/resources/room?view=graph-rest-beta)|
| Дополнение        | Бета-версия  | Добавлен ресурс [place](/graph/api/resources/place?view=graph-rest-beta)|
|Дополнение         | Бета-версия  | Добавлены разрешения приложений и делегированные [разрешения для API мест](permissions-reference.md#places-permissions): Place.Read.All |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:----------------|:------------|:-----------------------------------------|
|Дополнение|Бета|Добавлены новые объекты:<br/>[managedAllDeviceCertificateState](/graph/api/resources/intune-deviceconfig-managedalldevicecertificatestate?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[windowsKioskForceUpdateSchedule](/graph/api/resources/intune-deviceconfig-windowskioskforceupdateschedule?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[fileVaultState](/graph/api/resources/intune-deviceconfig-filevaultstate?view=graph-rest-beta)<br/>[windowsDefenderTamperProtectionOptions](/graph/api/resources/intune-deviceconfig-windowsdefendertamperprotectionoptions?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлено действие getRoleScopeTagsById в коллекцию [roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta) |
|Дополнение|Бета|Добавлено действие [createInstance](/graph/api/intune-deviceintent-devicemanagementtemplate-createinstance?view=graph-rest-beta) для объекта [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) |
|Дополнение|Бета|Добавлена функция hasCustomRoleScopeTag в коллекцию [roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta) |
|Удаление|Бета|Удалено действие [createInstance](/graph/api/intune-deviceintent-devicemanagementtemplate-createinstance?view=graph-rest-beta) для объекта [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) |
|Удаление|Бета|Удалена функция [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) для объекта [importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) |
|Дополнение|Бета|Добавлено свойство **scopeTags** для объекта [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **nestedSchemaItems** для объекта [androidManagedStoreAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschema?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **groupTag** для объекта [importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **fileVaultStates** для объекта [managedDeviceEncryptionState](/graph/api/resources/intune-deviceconfig-manageddeviceencryptionstate?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **userRightsDenyLocalLogOn** и **windowsDefenderTamperProtection** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **localGuestAccountName** и **assessmentAppUserModelId** для объекта [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **cacheServerHostNames**, **cacheServerForegroundDownloadFallbackToHttpDelayInSeconds** и **cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds** для объекта [windowsDeliveryOptimizationConfiguration](/graph/api/resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **windowsKioskForceUpdateSchedule** для объекта [windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство навигации **deviceConfigurationsAllManagedDeviceCertificateStates** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)|
|Удаление|Бета|Удалено свойство навигации **importedWindowsAutopilotDeviceIdentityUploads** из объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство навигации **deviceUpdateStates** для объекта [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **index** и **parentIndex** для сложного типа [androidManagedStoreAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **androidDeviceAdministratorEnrollmentEnabled** для сложного типа [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **edgeTraversal** для сложного типа [windowsFirewallRule](/graph/api/resources/intune-deviceconfig-windowsfirewallrule?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **localGuestAccount** для типа перечисления [secureAssessmentAccountType](/graph/api/resources/intune-deviceconfig-secureassessmentaccounttype?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены элементы **empty** и **clientCertificateSubjectName** для типа перечисления [vpnLocalIdentifier](/graph/api/resources/intune-deviceconfig-vpnlocalidentifier?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **revision** для объекта [groupPolicyDefinitionFile](/graph/api/resources/intune-grouppolicy-grouppolicydefinitionfile?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **valuePrefix** для объекта [groupPolicyPresentationListBox](/graph/api/resources/intune-grouppolicy-grouppolicypresentationlistbox?view=graph-rest-beta)|

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены свойства **expirationDatetime** и **password** для действия [createLink](/graph/api/driveitem-createlink?view=graph-rest-beta). |

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение | 1.0 | Добавлены [новые делегированные разрешения и разрешения приложений](/graph/permissions-reference?#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для получения и обновления ресурса [organization API](/graph/api/resources/organization?view=graph-rest-1.0) и получения ресурса [subcribedSku](/graph/api/resources/subscribedSku?view=graph-rest-1.0). |
| Дополнение | Бета-версия | Добавлены [новые делегированные разрешения и разрешения приложений](/graph/permissions-reference?#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для получения и обновления ресурса [organization API](/graph/api/resources/organization?view=graph-rest-beta) и получения ресурса [subcribedSku](/graph/api/resources/subscribedSku?view=graph-rest-beta). |
| Дополнение | 1.0 | Добавлена [функция group:validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0) и [функция directoryobject:validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0) для [групп](/graph/api/group-delta?view=graph-rest-1.0), которая проверяет, соответствует ли почтовый псевдоним или отображаемое имя группы Office 365 политикам именования. |
| Дополнение | Бета-версия |Добавлены свойства version, discoveryDateTime, discoverabilities для типа ресурса [directoryDefinition](/graph/api/resources/synchronization-directorydefinition?view=graph-rest-beta).|
| Дополнение | Бета-версия |Добавлен метод [directoryDefinition: discover](/graph/api/resources/directorydefinition-discover?view=graph-rest-beta).|
| Дополнение | Бета-версия | Добавлены [новые делегированные разрешения и разрешения приложений](/graph/permissions-reference?#organization-permissions) _AdministrativeUnit.Read.All_ и _AdministrativeUnit.ReadWrite.All_ для получения и обновления ресурса [administrative unit API](/graph/api/resources/administrativeunit?view=graph-rest-beta). |
| Дополнение | 1.0 | Добавлены [новые разрешения приложений и делегированные разрешения](/graph/permissions-reference?#organization-permissions) _RoleManagement.Read.Directory_ и _RoleManagement.ReadWrite.Directory_ для получения и обновления ресурса [API ролей каталога](/graph/api/resources/directoryRole?view=graph-rest-1.0), а также получения ресурса [API шаблона для ролей каталога](/graph/api/resources/directoryRoleTemplate?view=graph-rest-1.0). |
| Дополнение | Бета-версия | Добавлено [новое разрешение приложений](/graph/permissions-reference?#accessreviews-permissions) _AccessReview.ReadWrite.Membership_ для получения, создания, обновления и удаления в [access reviews API](/graph/api/resources/accessreviews-root?view=graph-rest-beta). |
| Дополнение | Бета-версия | Добавлен новый тип ресурса [**featureRolloutPolicy**](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta) в ресурс [directory](/graph/api/resources/directory?view=graph-rest-beta). Политика развертывания функций позволяет администраторам заказчика апробировать функции на определенных группах до того, как сделать данные функции доступными для всей организации.|


### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета | Добавлена поддержка разрешения приложений Mail.ReadBasic.All в API для управления объектом mailFolder: [перечисление объектов mailfolder](/graph/api/user-list-mailfolders?view=graph-rest-beta), [получение объекта mailfolder](/graph/api/mailfolder-get?view=graph-rest-beta), [перечисление дочерних папок](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta) и [перечисление сообщений в папке почты](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta). Кроме того, добавлена поддержка Mail.ReadBasic.All в [разностном запросе для сообщения](/graph/api/message-delta?view=graph-rest-beta) и [разностном запросе для объекта mailFolder](/graph/api/mailfolder-delta?view=graph-rest-beta).|

### <a name="reports"></a>Отчеты

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение        | Бета  | Добавлено свойство **deletedItemCount** для объекта [mailboxUsageDetail](/graph/api/resources/mailboxUsageDetail?view=graph-rest-beta).|
| Дополнение        | Бета  | Добавлено свойство **deletedItemSizeInBytes** для объекта [mailboxUsageDetail](/graph/api/resources/mailboxUsageDetail?view=graph-rest-beta).|
| Дополнение        | Бета-версия  | Добавлено свойство **groupId** для объекта [office365GroupsActivityDetail](/graph/api/resources/office365GroupsActivityDetail?view=graph-rest-beta).|

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета | Добавлена поддержка для разрешений для приложений на следующие действия: [перечисление сообщений в каналах](/graph/api/channel-list-messages?view=graph-rest-beta), [получение сообщений в каналах](/graph/api/channel-get-message?view=graph-rest-beta), [перечисление ответов на сообщения](/graph/api/channel-list-messagereplies?view=graph-rest-beta), и [вывод ответов на сообщения](/graph/api/channel-get-messagereply?view=graph-rest-beta). |
| Дополнение | Бета | Добавлена поддержка разрешения для приложений на [вывод сообщений в беседах](/graph/api/chatmessage-list?view=graph-rest-beta) и [получение сообщений в беседах](/graph/api/chatmessage-get?view=graph-rest-beta). |
| Дополнение | Бета | Добавлено свойство **installedApps** для ресурса [chat](/graph/api/resources/chat?view=graph-rest-beta).|
| Дополнение | Бета | Добавлена привязка навигации для свойства **chats** ресурса [user](/graph/api/resources/user?view=graph-rest-beta).|
| Дополнение | Бета | Добавлен ресурс [teamwork](/graph/api/resources/teamwork?view=graph-rest-beta). |
| Дополнение | Бета | Добавлен ресурс [userTeamwork](/graph/api/resources/userteamwork?view=graph-rest-beta). |
| Дополнение | Бета | Добавлены новые методы для ресурса [user](/graph/api/resources/user?view=graph-rest-beta), позволяющие использовать следующие методы с личными приложениями для пользователей: <br>[Перечисление приложений, установленных для пользователя](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta) <br>[Установка приложения для пользователя](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta) <br>[Удаление приложения для пользователя](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta) <br>[Обновление приложения, установленного для пользователя](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta)|

### <a name="calls-and-online-meetings"></a>Звонки и собрания по сети

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение        | бета        | Добавлено свойство **mediaState** для ресурса [call](/api-reference/beta/resources/call.md)|
| Изменение          | бета        | Свойство **recordResourceLocation** в ресурсе [recordOperation](/api-reference/beta/resources/recordOperation.md) переименовано на **recordingLocation**|
| Изменение          | Бета-версия        | Свойство **recordResourceAccessToken** в ресурсе [recordOperation](/api-reference/beta/resources/recordOperation.md) переименовано на **recordingAccessToken**|
| Дополнение        | Бета-версия        | Добавлено свойство **capabilities** для ресурса [onlineMeeting](/api-reference/beta/resources/onlinemeeting.md) |
| Дополнение        | бета        | Добавлено свойство **videoTeleconferenceId** для ресурса [onlineMeeting](/api-reference/beta/resources/onlinemeeting.md) |
| Дополнение        | бета        | Добавлено свойство **producers** для ресурса [meetingParticipants](/api-reference/beta/resources/meetingparticipants.md) |
| Дополнение        | бета        | Добавлено свойство **contributors** для ресурса [meetingParticipants](/api-reference/beta/resources/meetingparticipants.md) |

## <a name="june-2019"></a>Июнь 2019 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[appVulnerabilityManagedDevice](/graph/api/resources/intune-partnerintegration-appvulnerabilitymanageddevice?view=graph-rest-beta)<br/>[appVulnerabilityMobileApp](/graph/api/resources/intune-partnerintegration-appvulnerabilitymobileapp?view=graph-rest-beta)<br/>[appVulnerabilityTask](/graph/api/resources/intune-partnerintegration-appvulnerabilitytask?view=graph-rest-beta)<br/>[deviceAppManagementTask](/graph/api/resources/intune-partnerintegration-deviceappmanagementtask?view=graph-rest-beta)<br/>[deviceManagementDomainJoinConnector](/graph/api/resources/intune-odj-devicemanagementdomainjoinconnector?view=graph-rest-beta)<br/>[iosikEv2VpnConfiguration](/graph/api/resources/intune-deviceconfig-iosikev2vpnconfiguration?view=graph-rest-beta)<br/>[roleScopeTagAutoAssignment](/graph/api/resources/intune-rbac-rolescopetagautoassignment?view=graph-rest-beta)<br/>[windows10DeviceFirmwareConfigurationInterface](/graph/api/resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[deviceManagementApplicabilityRuleDeviceMode](/graph/api/resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode?view=graph-rest-beta)<br/>[deviceManagementApplicabilityRuleOsEdition](/graph/api/resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition?view=graph-rest-beta)<br/>[deviceManagementApplicabilityRuleOsVersion](/graph/api/resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion?view=graph-rest-beta)<br/>[deviceManagementSettingComparison](/graph/api/resources/intune-deviceintent-devicemanagementsettingcomparison?view=graph-rest-beta)<br/>[iosVpnSecurityAssociationParameters](/graph/api/resources/intune-deviceconfig-iosvpnsecurityassociationparameters?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[appInstallControlType](/graph/api/resources/intune-deviceconfig-appinstallcontroltype?view=graph-rest-beta)<br/>[appVulnerabilityTaskMitigationType](/graph/api/resources/intune-partnerintegration-appvulnerabilitytaskmitigationtype?view=graph-rest-beta)<br/>[changeUefiSettingsPermission](/graph/api/resources/intune-deviceconfig-changeuefisettingspermission?view=graph-rest-beta)<br/>[deviceAppManagementTaskCategory](/graph/api/resources/intune-partnerintegration-deviceappmanagementtaskcategory?view=graph-rest-beta)<br/>[deviceAppManagementTaskPriority](/graph/api/resources/intune-partnerintegration-deviceappmanagementtaskpriority?view=graph-rest-beta)<br/>[deviceAppManagementTaskStatus](/graph/api/resources/intune-partnerintegration-deviceappmanagementtaskstatus?view=graph-rest-beta)<br/>[deviceManagementApplicabilityRuleType](/graph/api/resources/intune-deviceconfig-devicemanagementapplicabilityruletype?view=graph-rest-beta)<br/>[deviceManagementComparisonResult](/graph/api/resources/intune-deviceintent-devicemanagementcomparisonresult?view=graph-rest-beta)<br/>[deviceManagementDomainJoinConnectorState](/graph/api/resources/intune-odj-devicemanagementdomainjoinconnectorstate?view=graph-rest-beta)<br/>[deviceManagementTemplateType](/graph/api/resources/intune-deviceintent-devicemanagementtemplatetype?view=graph-rest-beta)<br/>[macOSFileVaultRecoveryKeyTypes](/graph/api/resources/intune-deviceconfig-macosfilevaultrecoverykeytypes?view=graph-rest-beta)<br/>[managedAppNotificationRestriction](/graph/api/resources/intune-mam-managedappnotificationrestriction?view=graph-rest-beta)<br/>[mobileAppDependencyType](/graph/api/resources/intune-apps-mobileappdependencytype?view=graph-rest-beta)<br/>[secureBootWithDMAType](/graph/api/resources/intune-deviceconfig-securebootwithdmatype?view=graph-rest-beta)<br/>[vpnClientAuthenticationType](/graph/api/resources/intune-deviceconfig-vpnclientauthenticationtype?view=graph-rest-beta)<br/>[vpnDeadPeerDetectionRate](/graph/api/resources/intune-deviceconfig-vpndeadpeerdetectionrate?view=graph-rest-beta)<br/>[vpnEncryptionAlgorithmType](/graph/api/resources/intune-deviceconfig-vpnencryptionalgorithmtype?view=graph-rest-beta)<br/>[vpnIntegrityAlgorithmType](/graph/api/resources/intune-deviceconfig-vpnintegrityalgorithmtype?view=graph-rest-beta)<br/>[vpnLocalIdentifier](/graph/api/resources/intune-deviceconfig-vpnlocalidentifier?view=graph-rest-beta)<br/>[vpnServerCertificateType](/graph/api/resources/intune-deviceconfig-vpnservercertificatetype?view=graph-rest-beta)<br/>[windows10DeviceModeType](/graph/api/resources/intune-deviceconfig-windows10devicemodetype?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлено действие [updateStatus](/graph/api/intune-partnerintegration-deviceappmanagementtask-updatestatus?view=graph-rest-beta) для объекта [deviceAppManagementTask](/graph/api/resources/intune-partnerintegration-deviceappmanagementtask?view=graph-rest-beta) |
|Дополнение|Бета|Добавлено действие [assign](/graph/api/intune-rbac-rolescopetag-assign?view=graph-rest-beta) для объекта [roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta) |
|Дополнение|Бета|Добавлена функция [compare](/graph/api/intune-deviceintent-devicemanagementtemplate-compare?view=graph-rest-beta) для объекта [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) |
|Дополнение|Бета|Добавлена функция [compare](/graph/api/intune-deviceintent-devicemanagementintent-compare?view=graph-rest-beta) для объекта [deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta) |
|Удаление|бета|Удалены следующие типы перечисления:<br/>**mobileAppDependecyType**<br/>|
|Дополнение|Бета|Добавлены свойства **deviceManagementApplicabilityRuleOsEdition**, **deviceManagementApplicabilityRuleOsVersion** и **deviceManagementApplicabilityRuleDeviceMode** для объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **securityKeyForSignIn** для объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **roleScopeTagIds** для объекта [deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **templateType** и **publishedDateTime** для объекта [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **customPrivacyMessage** для объекта [intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **fileVaultEnabled**, **fileVaultSelectedRecoveryKeyTypes**, **fileVaultInstitutionalRecoveryKeyCertificate**, **fileVaultInstitutionalRecoveryKeyCertificateFileName**, **fileVaultPersonalRecoveryKeyHelpMessage**, **fileVaultAllowDeferralUntilSignOut**, **fileVaultNumberOfTimesUserCanIgnore**, **fileVaultDisablePromptAtSignOut** и **fileVaultPersonalRecoveryKeyRotationInMonths** для объекта [macOSEndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-macosendpointprotectionconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **notificationRestriction** для объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)|
|Изменение|бета|Изменен тип следующих свойств объекта [mobileAppDependency](/graph/api/resources/intune-apps-mobileappdependency?view=graph-rest-beta):<br/>вместо **dependencyType** из [mobileAppDependecyType](/graph/api/resources/intune-apps-mobileappdependecytype?view=graph-rest-beta) теперь используется [mobileAppDependencyType](/graph/api/resources/intune-apps-mobileappdependencytype?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлено свойство **deviceGuardSecureBootWithDMA** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **smartScreenAppInstallControl** и **lockScreenActivateAppsWithVoice** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство навигации **deviceAppManagementTasks** для объекта [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство навигации **domainJoinConnectors** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство навигации **assignments** для объекта [roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **isReadOnly** для сложного типа [omaSettingInteger](/graph/api/resources/intune-deviceconfig-omasettinginteger?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены свойства **v10_1809** и **v10_1903** для сложного типа [windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **wpa2Enterprise** для типа перечисления [androidWiFiSecurityType](/graph/api/resources/intune-deviceconfig-androidwifisecuritytype?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **ikEv2** для типа перечисления [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены элементы **rotateFileVaultKey** и **getFileVaultKey** для типа перечисления [remoteAction](/graph/api/resources/intune-devices-remoteaction?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **sharedSecret** для типа перечисления [vpnAuthenticationMethod](/graph/api/resources/intune-deviceconfig-vpnauthenticationmethod?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены элементы **windows10Home**, **windows10HomeChina**, **windows10HomeN**, **windows10HomeSingleLanguage**, **windows10Mobile**, **windows10IoTCore** и **windows10IoTCoreCommercial** для типа перечисления [windows10EditionType](/graph/api/resources/intune-deviceconfig-windows10editiontype?view=graph-rest-beta).|

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение | Бета | Добавлен [riskDetection API](/graph/api/resources/riskdetection?view=graph-rest-beta), представляющий определения рисков в службе защиты идентификации Azure AD. |
| Дополнение        | бета  | Появился новый тип ресурса [applicationTemplate](/graph/api/resources/applicationtemplate.md). Этот тип поддерживает операции [instantiate](/graph/api/applicationtemplate-instantiate.md), [list](/graph/api/applicationtemplate-instantiate.md) и [get](/graph/api/applicationtemplate-get.md) с приложениями из коллекции Azure AD.|
| Дополнение | Бета|Добавлены новые ресурсы: </br> [detailsInfo](/graph/api/resources/detailsInfo?view=graph-rest-beta)</br> [initiator](/graph/api/resources/initiator?view=graph-rest-beta)</br> [modifiedProperty](/graph/api/resources/modifiedProperty?view=graph-rest-beta)</br> [provisionedIdentity](/graph/api/resources/provisionedIdentity?view=graph-rest-beta)</br> [provisioningObjectsummary](/graph/api/resources/provisioningObjectsummary?view=graph-rest-beta)</br> [provisioningStep](/graph/api/resources/provisioningStep?view=graph-rest-beta)</br> [provisioningsystemDetails](/graph/api/resources/provisioningsystemDetails?view=graph-rest-beta)</br> [statusBase](/graph/api/resources/statusBase?view=graph-rest-beta)|
| Дополнение |Бета |Добавлена операция [перечисления provisioningObjectSummary](/graph/api/resources/provisioning-object-summary-list?view=graph-rest-beta)</br>|                     |
| Дополнение | 1.0 | Добавлено свойство **signInSessionsValidFromDateTime** для ресурса [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлено действие [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) для ресурса [user](/graph/api/resources/user?view=graph-rest-1.0). |

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета | Добавлена поддержка разрешения Mail.ReadBasic в API для управления объектом mailFolder: [перечисление объектов mailfolder](/graph/api/user-list-mailfolders?view=graph-rest-beta), [получение объекта mailfolder](/graph/api/mailfolder-get?view=graph-rest-beta), [перечисление дочерних папок](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta) и [перечисление сообщений в папке почты](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta). Кроме того, добавлена поддержка Mail.ReadBasic в [разностном запросе для сообщения](/graph/api/message-delta?view=graph-rest-beta) и [разностном запросе для объекта mailFolder](/graph/api/mailfolder-delta?view=graph-rest-beta).|

### <a name="reports--identity-and-access-reports"></a>Отчеты | Отчеты об удостоверениях и доступе

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Дополнение|Бета| Добавлены новые отчеты для получения сведений о регистрации пользователей и использовании действий:<br/><ul><li>[reportroot-getcredentialusagesummary](/graph/api/reportroot-getcredentialusagesummary?view=graph-rest-beta) — создает отчет об использовании самостоятельного сброса паролей.</li><li>[reportroot-getcredentialuserregistrationcount](/graph/api/reportroot-getcredentialuserregistrationcount?view=graph-rest-beta) — создает отчет о числе регистраций для самостоятельного сброса паролей и многофакторной проверки подлинности.</li><li>[reportroot-list-credentialuserregistrationdetails](/graph/api/reportroot-list-credentialuserregistrationdetails?view=graph-rest-beta) — создает отчет об использовании самостоятельного сброса паролей и многофакторной проверки подлинности.</li><li>[reportroot-list-usercredentialusagedetails](/graph/api/resources/reportroot-list-usercredentialusagedetails?view=graph-rest-beta) — создает отчет об использовании самостоятельного сброса паролей для пользователя.</li></ul> |

### <a name="sites-and-lists-sharepoint"></a>Сайты и списки (SharePoint)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство навигации[followSite](/graph/api/follow-site?view=graph-rest-beta) в набор сущностей [user](/graph/api/resources/user?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлено свойство навигации [unfollowSite](/graph/api/unfollow-site?view=graph-rest-beta) в набор сущностей [user](/graph/api/resources/user?view=graph-rest-beta). |

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета | Добавлен ресурс [teamDiscoverySettings](/api-reference/beta/resources/teamdiscoverysettings.md) и соответствующие методы. |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство **lastPasswordChangeDateTime** для объекта [user](/graph/api/resources/user?view=graph-rest-beta). |

## <a name="may-2019"></a>Май 2019 г.

### <a name="calendar-mail-personal-contacts-outlook"></a>Календарь, почта, личные контакты (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | 1.0 и бета-версия | Для администраторов добавлена возможность ограничить приложению доступ, указав только определенные почтовые ящики, даже если ему предоставлены разрешения приложений на доступ к почте, параметрам почтового ящика, календарям и контактам. Дополнительные сведения см. в статье [Ограничение области разрешений для приложений с указанием определенных почтовых ящиков Exchange Online](auth-limit-mailbox-access.md). |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[deviceManagementDerivedCredentialSettings](/graph/api/resources/intune-deviceconfig-devicemanagementderivedcredentialsettings?view=graph-rest-beta)<br/>[iosDerivedCredentialAuthenticationConfiguration](/graph/api/resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration?view=graph-rest-beta)<br/>[securityBaselineCategoryStateSummary](/graph/api/resources/intune-deviceintent-securitybaselinecategorystatesummary?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[deviceManagementDerivedCredentialIssuer](/graph/api/resources/intune-deviceconfig-devicemanagementderivedcredentialissuer?view=graph-rest-beta)<br/>[deviceManagementDerivedCredentialNotificationType](/graph/api/resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype?view=graph-rest-beta)<br/>[emailCertificateType](/graph/api/resources/intune-deviceconfig-emailcertificatetype?view=graph-rest-beta)<br/>[mobileAppDependencyType](/graph/api/resources/intune-apps-mobileappdependencytype?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлено действие executeAction для коллекции [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Дополнение|бета|Добавлено действие [rotateFileVaultKey](/graph/api/intune-devices-manageddevice-rotatefilevaultkey?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [migrateToTemplate](/graph/api/intune-deviceintent-devicemanagementintent-migratetotemplate?view=graph-rest-beta) для объекта [deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta) |
|Дополнение|бета|Добавлена функция [getFileVaultKey](/graph/api/intune-devices-manageddevice-getfilevaultkey?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Удаление|бета|Удалены следующие типы перечисления:<br/>**mobileAppDependecyType**<br/>|
|Удаление|бета|Добавлено действие executeAction для коллекции [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Дополнение|бета|Добавлены свойства **usernameFormatString**, **passwordFormatString** и **preSharedKey** для объекта [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **customBrowserPackageId** и **customBrowserDisplayName** для объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **customBrowserProtocol**, **customBrowserPackageId** и **customBrowserDisplayName** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **thirdPartyKeyboardsBlocked** из объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Изменение|бета|Изменены следующие свойства объекта [deviceManagementAbstractComplexSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance?view=graph-rest-beta):<br/>**implementationId** теперь можно не указывать<br/>|
|Дополнение|бета|Добавлены свойства **versionInfo**, **isDeprecated** и **intentCount** для объекта [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **assignedUserPrincipalName** для объекта [importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **signingCertificateType** и **encryptionCertificateType** для объекта [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **usernameFormatString** и **passwordFormatString** для объекта [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **kioskModeBlockAutoLock**, **kioskModeBlockRingerSwitch**, **kioskModeBlockScreenRotation**, **kioskModeBlockSleepButton**, **kioskModeBlockTouchscreen**, **cellularBlockPersonalHotspotModification** и **siriDisableServerLogging** для объекта [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **customBrowserProtocol** для объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **thirdPartyKeyboardsBlocked** из объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **iCloudBlockPhotoLibrary**, **screenCaptureBlocked**, **classroomAppBlockRemoteScreenObservation**, ** classroomAppForceUnpromptedScreenObservation**, **classroomForceAutomaticallyJoinClasses**, **classroomForceRequestPermissionToLeaveClasses** и **classroomForceUnpromptedAppAndDeviceLock** для объекта [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **retireAfterDateTime** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Изменение|бета|Изменен тип следующих свойств объекта [mobileAppDependency](/graph/api/resources/intune-apps-mobileappdependency?view=graph-rest-beta):<br/>вместо **dependencyType** из [mobileAppDependecyType](/graph/api/resources/intune-apps-mobileappdependecytype?view=graph-rest-beta) теперь используется [mobileAppDependencyType](/graph/api/resources/intune-apps-mobileappdependencytype?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлено свойство **fastFirstSignIn** для объекта [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **roleScopeTagIds** для объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **configDeviceHealthMonitoringCustomScope** для объекта [windowsHealthMonitoringConfiguration](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **migratableTo** для объекта [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **derivedCredentialSettings** для объекта [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **derivedCredentialSettings** для объекта [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **derivedCredentialSettings** для объекта [iosVpnConfiguration](/graph/api/resources/intune-deviceconfig-iosvpnconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **categoryDeviceStateSummaries** для объекта [securityBaselineTemplate](/graph/api/resources/intune-deviceintent-securitybaselinetemplate?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **wpaEnterprise** для типа перечисления [androidDeviceOwnerWiFiSecurityType](/graph/api/resources/intune-deviceconfig-androiddeviceownerwifisecuritytype?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **unknown** для типа перечисления [devicePlatformType](/graph/api/resources/intune-shared-deviceplatformtype?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **derivedCredential** для типа перечисления [easAuthenticationMethod](/graph/api/resources/intune-deviceconfig-easauthenticationmethod?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **wipe** для типа перечисления [managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction?view=graph-rest-beta)|
|Изменение|бета|Изменен тип следующих свойств типа перечисления [managedDeviceRemoteAction](/graph/api/resources/intune-devices-manageddeviceremoteaction?view=graph-rest-beta):<br/>**fullScan** с 2 на 3<br/>**quickScan** с 3 на 4<br/>**signatureUpdate** с 4 на 5<br/>|
|Дополнение|бета|Добавлен элемент **derivedCredential** для типа перечисления [vpnAuthenticationMethod](/graph/api/resources/intune-deviceconfig-vpnauthenticationmethod?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **derivedCredential** для типа перечисления [wiFiAuthenticationMethod](/graph/api/resources/intune-deviceconfig-wifiauthenticationmethod?view=graph-rest-beta)|

### <a name="files-onedrive"></a>Файлы (OneDrive)
| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета-версия | Добавлен сложный тип [bundle](/graph/api/resources/bundle?view=graph-rest-beta) |
| Дополнение | Бета-версия | Добавлен сложный тип [album](/graph/api/resources/album?view=graph-rest-beta) |
| Дополнение | Бета-версия | Добавлено свойство навигации **bundles** для объекта [drive](/graph/api/resources/drive?view=graph-rest-beta) |
| Дополнение | Бета-версия | Добавлено свойство **bundle** для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |
| Дополнение | Бета-версия | Добавлено действие **grant** для объекта [permission](/graph/api/resources/permission?view=graph-rest-beta) |

### <a name="education"></a>Образование
| Тип изменения | Версия | Описание                                                                                                                                                      |
| :---------- | :------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Дополнение    | Бета    | Добавление taughtClasses к [educationUser](/graph/api/resources/educationUser?view=graph-rest-beta).                                                                  |
| Дополнение    | Бета    | Добавление [educationCourse](/graph/api/resources/educationCourse?view=graph-rest-beta) к [educationClass](/graph/api/resources/educationClass?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавление поддержки [delta](/graph/delta-query-overview) к [educationUser](/graph/api/resources/educationUser?view=graph-rest-beta).                                   |
| Дополнение    | Бета    | Добавление [delta](/graph/delta-query-overview) к [educationSchool](/graph/api/resources/educationSchool?view=graph-rest-beta).                                       |
| Дополнение    | Бета    | Добавление [delta](/graph/delta-query-overview) к [educationClass](/graph/api/resources/educationClass?view=graph-rest-beta).                                         |
| Дополнение    | Бета    | В перечисление [educationUserRole](/graph/api/resources/enums?view=graph-rest-beta#educationuserrole-values) добавлен параметр `faculty`.                              |

### <a name="groups"></a>Группы
| **Тип изменения** | **Версия** | **Описание** |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлено свойство **assignedlabels** для объекта [group](/graph/api/resources/group?view=graph-rest-beta). Это свойство представляет список пар меток конфиденциальности (идентификатор и имя метки), связанных с группой.

### <a name="identity-and-access-azure-ad--identity-protection"></a>Удостоверение и доступ (Azure AD) | Защита удостоверений

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлен объект [riskyUserHistoryItem](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta). |
| Дополнение | бета | Добавлена операция [список журнала](/graph/api/riskyuser-list-history?view=graph-rest-beta). |

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | 1.0 | Добавлен объект [mailSearchFolder](/graph/api/resources/mailsearchfolder?graph-rest-1.0), производный от объекта [mailFolder](/graph/api/resources/mailfolder?graph-rest-1.0) и поддерживающий его методы. |

### <a name="reports--office-365-usage-reports"></a>Отчеты | Отчеты об использовании Office 365

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение        | бета  | Добавлено свойство **ownerPrincipalName** для объекта [oneDriveUsageAccountDetail](/graph/api/resources/oneDriveUsageAccountDetail?view=graph-rest-beta).|
| Дополнение        | бета  | Добавлено свойство **ownerPrincipalName** для объекта [sharePointSiteUsageDetail](/graph/api/resources/sharePointSiteUsageDetail?view=graph-rest-beta).|

### <a name="security"></a>Безопасность

| **Тип изменения** | **Версия** | **Описание**              |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0       | Добавлены API оценки безопасности для [API безопасности](/graph/api/resources/securescore-api-overview?view=graph-rest-1.0), включающие следующие ресурсы и операции:<br/>[secureScore](/graph/api/resources/securescore?view=graph-rest-1.0) (и соответствующие объекты)<br/>[Перечисление объектов secureScores](/graph/api/securescores-list?view=graph-rest-1.0)<br/>[secureScoreControlProfile](/graph/api/resources/securescorecontrolprofile?view=graph-rest-1.0)<br/>[Перечисление объектов secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-list?view=graph-rest-1.0)<br/>[Обновление объектов secureScoreControlProfile](/graph/api/securescorecontrolprofiles-update?view=graph-rest-1.0) |

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение        | бета        | Добавлено свойство **urgent** для перечисления [chatMessageImportance](/graph/api/resources/chatMessageImportance?view=graph-rest-beta).|
| Дополнение        | бета        | Добавлено свойство навигации **hostedContents** для объекта [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta).|
| Дополнение        | бета        | Добавлен объект **chatMessageHostedContent** для представления контента, размещенного в Microsoft Teams и связанного с [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta). |


## <a name="april-2019"></a>Апрель 2019 г.

### <a name="change-notifications-webhooks"></a>Уведомления об изменениях (веб-перехватчики)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлены два типа уведомлений жизненного цикла (`subscriptionRemoved` и `missed`), доступные для ресурсов Outlook. Приложения, выполняющие подписку, могут принимать соответствующие меры, чтобы уменьшить влияние прерывания уведомлений. Дополнительные сведения см. в статье [Уменьшение числа пропущенных подписок и уведомлений о ресурсах Outlook (предварительная версия)](webhooks-outlook-authz.md)|

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidDeviceOwnerCompliancePolicy](/graph/api/resources/intune-deviceconfig-androiddeviceownercompliancepolicy?view=graph-rest-beta)<br/><br/>[macOSExtensionsConfiguration](/graph/api/resources/intune-deviceconfig-macosextensionsconfiguration?view=graph-rest-beta)<br/><br/>[mobileAppDependency](/graph/api/resources/intune-apps-mobileappdependency?view=graph-rest-beta)<br/><br/>[mobileAppRelationship](/graph/api/resources/intune-apps-mobileapprelationship?view=graph-rest-beta)<br/><br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[macOSKernelExtension](/graph/api/resources/intune-deviceconfig-macoskernelextension?view=graph-rest-beta)<br/><br/>[macOSLaunchItem](/graph/api/resources/intune-deviceconfig-macoslaunchitem?view=graph-rest-beta)<br/><br/>[mobileAppRelationshipState](/graph/api/resources/intune-apps-mobileapprelationshipstate?view=graph-rest-beta)<br/><br/>[win32LobAppFileSystemRequirement](/graph/api/resources/intune-apps-win32lobappfilesystemrequirement?view=graph-rest-beta)<br/><br/>[win32LobAppPowerShellScriptRequirement](/graph/api/resources/intune-apps-win32lobapppowershellscriptrequirement?view=graph-rest-beta)<br/><br/>[win32LobAppRegistryRequirement](/graph/api/resources/intune-apps-win32lobappregistryrequirement?view=graph-rest-beta)<br/><br/>[win32LobAppRequirement](/graph/api/resources/intune-apps-win32lobapprequirement?view=graph-rest-beta)<br/><br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[androidDeviceOwnerPlayStoreMode](/graph/api/resources/intune-deviceconfig-androiddeviceownerplaystoremode?view=graph-rest-beta)<br/><br/>[mobileAppDependecyType](/graph/api/resources/intune-apps-mobileappdependecytype?view=graph-rest-beta)<br/><br/>[win32LobAppPowerShellScriptDetectionType](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetectiontype?view=graph-rest-beta)<br/><br/>|
|Дополнение|Бета|Добавлено действие [updateRelationships](/graph/api/intune-apps-mobileapp-updaterelationships?view=graph-rest-beta)<br/> для [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)<br/> |
|Дополнение|Бета|Добавлено действие **import** для коллекции [importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)<br/> . |
|Дополнение|Бета|Добавлена функция [getRelatedAppStates](/graph/api/intune-apps-mobileapp-getrelatedappstates?view=graph-rest-beta)<br/> для [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)<br/> |
|Дополнение|Бета|Добавлены свойства **kioskModeBluetoothConfigurationEnabled**, **kioskModeWiFiConfigurationEnabled**, **passwordMinimumLetterCharacters**, **passwordMinimumLowerCaseCharacters**, **passwordMinimumNonLetterCharacters**, **passwordMinimumNumericCharacters**, **passwordMinimumSymbolCharacters**, **passwordMinimumUpperCaseCharacters** и **playStoreMode** для объекта [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлено свойство **subjectAlternativeNameType** для объекта [androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta)<br/> .|
|Удаление|Бета|Удалено свойство **subjectAlternativeNameType** из объекта [androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta)<br/> .|
|Удаление|Бета|Удалено свойство **subjectAlternativeNameType** из объекта [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлено свойство **subjectAlternativeNameType** для объекта [androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta)<br/> .|
|Удаление|Бета|Удалено свойство **subjectAlternativeNameType** из объекта [androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta)<br/> .|
|Удаление|Бета|Удалено свойство **subjectAlternativeNameType** из объекта [androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлено свойство **deviceNameTemplate** для объекта [depEnrollmentBaseProfile](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлено действие **import** для коллекции [importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлены свойства **autoLaunchItems**, **adminShowHostInfo**, **loginWindowText**, **authorizedUsersListHidden**, **authorizedUsersListHideLocalUsers**, **authorizedUsersListHideMobileAccounts**, **authorizedUsersListIncludeNetworkUsers**, **authorizedUsersListHideAdminUsers**, **authorizedUsersListShowOtherManagedUsers**, **shutDownDisabled**, **restartDisabled**, **sleepDisabled**, **consoleAccessDisabled**, **shutDownDisabledWhileLoggedIn**, **restartDisabledWhileLoggedIn**, **powerOffDisabledWhileLoggedIn**, **logOutDisabledWhileLoggedIn** и **screenLockDisableImmediate** для объекта [macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлено свойство **dependentAppCount** для объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлено свойство **requirementRules** для объекта [win32LobApp](/graph/api/resources/intune-apps-win32lobapp?view=graph-rest-beta)<br/> .|
|Удаление|Бета|Удалено свойство **tpmRequired** из объекта [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлено свойство **groupTag** для объекта [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлено свойство навигации **users** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлено свойство навигации **relationships** для объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлено свойство **customPrivacyMessage** для сложного типа [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлены элементы **dependencyFailedToInstall**, **dependencyWithRequirementsNotMet**, **dependencyPendingReboot**, ** dependencyWithAutoInstallDisabled**, **autoInstallDisabled**, **installingDependencies**, **powerShellScriptRequirementNotMet**, **registryRequirementNotMet** и **fileSystemRequirementNotMet** типа перечисления [resultantAppStateDetail](/graph/api/resources/intune-apps-resultantappstatedetail?view=graph-rest-beta)<br/> .|
|Дополнение|Бета|Добавлен элемент **doesNotExist** типа перечисления [win32LobAppFileSystemDetectionType](/graph/api/resources/intune-apps-win32lobappfilesystemdetectiontype?view=graph-rest-beta)<br/> .|

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[deviceManagementAbstractComplexSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementAbstractComplexSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance?view=graph-rest-beta)<br/>[deviceManagementBooleanSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementbooleansettinginstance?view=graph-rest-beta)<br/>[deviceManagementCollectionSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementcollectionsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementCollectionSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementcollectionsettinginstance?view=graph-rest-beta)<br/>[deviceManagementComplexSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementcomplexsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementComplexSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementcomplexsettinginstance?view=graph-rest-beta)<br/>[deviceManagementIntegerSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementintegersettinginstance?view=graph-rest-beta)<br/>[deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta)<br/>[deviceManagementIntentAssignment](/graph/api/resources/intune-deviceintent-devicemanagementintentassignment?view=graph-rest-beta)<br/>[deviceManagementIntentDeviceSettingStateSummary](/graph/api/resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary?view=graph-rest-beta)<br/>[deviceManagementIntentDeviceState](/graph/api/resources/intune-deviceintent-devicemanagementintentdevicestate?view=graph-rest-beta)<br/>[deviceManagementIntentDeviceStateSummary](/graph/api/resources/intune-deviceintent-devicemanagementintentdevicestatesummary?view=graph-rest-beta)<br/>[deviceManagementIntentSettingCategory](/graph/api/resources/intune-deviceintent-devicemanagementintentsettingcategory?view=graph-rest-beta)<br/>[deviceManagementIntentUserState](/graph/api/resources/intune-deviceintent-devicemanagementintentuserstate?view=graph-rest-beta)<br/>[deviceManagementIntentUserStateSummary](/graph/api/resources/intune-deviceintent-devicemanagementintentuserstatesummary?view=graph-rest-beta)<br/>[deviceManagementSettingCategory](/graph/api/resources/intune-deviceintent-devicemanagementsettingcategory?view=graph-rest-beta)<br/>[deviceManagementSettingDefinition](/graph/api/resources/intune-deviceintent-devicemanagementsettingdefinition?view=graph-rest-beta)<br/>[deviceManagementSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementsettinginstance?view=graph-rest-beta)<br/>[deviceManagementStringSettingInstance](/graph/api/resources/intune-deviceintent-devicemanagementstringsettinginstance?view=graph-rest-beta)<br/>[deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta)<br/>[deviceManagementTemplateSettingCategory](/graph/api/resources/intune-deviceintent-devicemanagementtemplatesettingcategory?view=graph-rest-beta)<br/>[securityBaselineDeviceState](/graph/api/resources/intune-deviceintent-securitybaselinedevicestate?view=graph-rest-beta)<br/>[securityBaselineSettingState](/graph/api/resources/intune-deviceintent-securitybaselinesettingstate?view=graph-rest-beta)<br/>[securityBaselineState](/graph/api/resources/intune-deviceintent-securitybaselinestate?view=graph-rest-beta)<br/>[securityBaselineStateSummary](/graph/api/resources/intune-deviceintent-securitybaselinestatesummary?view=graph-rest-beta)<br/>[securityBaselineTemplate](/graph/api/resources/intune-deviceintent-securitybaselinetemplate?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[deviceManagementConstraint](/graph/api/resources/intune-deviceintent-devicemanagementconstraint?view=graph-rest-beta)<br/>[deviceManagementEnumConstraint](/graph/api/resources/intune-deviceintent-devicemanagementenumconstraint?view=graph-rest-beta)<br/>[deviceManagementEnumValue](/graph/api/resources/intune-deviceintent-devicemanagementenumvalue?view=graph-rest-beta)<br/>[deviceManagementSettingBooleanConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingbooleanconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingDependency](/graph/api/resources/intune-deviceintent-devicemanagementsettingdependency?view=graph-rest-beta)<br/>[deviceManagementSettingIntegerConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingintegerconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingRegexConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingregexconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingStringLengthConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingstringlengthconstraint?view=graph-rest-beta)<br/>[deviceManagementSettingXmlConstraint](/graph/api/resources/intune-deviceintent-devicemanagementsettingxmlconstraint?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[deviceManangementIntentValueType](/graph/api/resources/intune-deviceintent-devicemanangementintentvaluetype?view=graph-rest-beta)<br/>[securityBaselineComplianceState](/graph/api/resources/intune-deviceintent-securitybaselinecompliancestate?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлено действие [createInstance](/graph/api/intune-deviceintent-devicemanagementtemplate-createinstance?view=graph-rest-beta) для объекта [deviceManagementTemplate](/graph/api/resources/intune-deviceintent-devicemanagementtemplate?view=graph-rest-beta) |
|Дополнение|Бета|Добавлено действие [updateSettings](/graph/api/intune-deviceintent-devicemanagementintent-updatesettings?view=graph-rest-beta) для объекта [deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta) |
|Дополнение|Бета|Добавлено действие [assign](/graph/api/intune-deviceintent-devicemanagementintent-assign?view=graph-rest-beta) для объекта [deviceManagementIntent](/graph/api/resources/intune-deviceintent-devicemanagementintent?view=graph-rest-beta) |
|Дополнение|Бета|Добавлены свойства навигации **intents**, **settingDefinitions**, **templates** и **categories** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство навигации **securityBaselineStates** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|

### <a name="files-sites-and-lists-onedrive-for-business-and-sharepoint"></a>Файлы, сайты и списки (OneDrive для бизнеса и SharePoint)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлено свойство **analytics** для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлено свойство **analytics** для объекта [site](/graph/api/resources/site?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлено свойство **analytics** для объекта [listItem](/graph/api/resources/listitem?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлена функция **getActivitiesByInterval** для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлена функция **getActivitiesByInterval** для объекта [site](/graph/api/resources/site?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлена функция **getActivitiesByInterval** для объекта [listItem](/graph/api/resources/listitem?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлен объект [itemAnalytics](/graph/api/resources/itemanalytics?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлен объект [itemActivityStat](/graph/api/resources/itemactivity?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлен сложный тип [itemActionStat](/graph/api/resources/itemactionstat?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлен сложный тип [accessAction](/graph/api/resources/accessaction?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлен сложный тип [incompleteData](/graph/api/resources/incompletedata?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлено свойство **access** для сложного типа [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлено свойство **location** для сложного типа [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta). |

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | 1.0 |  Представлены новые **API журналов аудита для Azure AD**, предоставляющие журналы действий для задач управления каталогом с помощью объекта [directoryAudit](/graph/api/resources/directoryAudit?view=graph-rest-1.0) и действий входа с помощью объекта [signIns](/graph/api/resources/signIns?view=graph-rest-1.0).|
| Дополнение | бета | Добавлены новые разрешения приложений для API **проверки доступа**: AccessReview.Read.All, ProgramControl.Read.All и ProgramControl.ReadWrite.All. Дополнительные сведения см. в статье [Справочник по API проверки доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta). |
| Дополнение | Бета | Добавлено свойство **signInSessionsValidFromDateTime** для ресурса [user](/graph/api/resources/user?view=graph-rest-beta). Это переименование свойств **refreshTokensValidFromDateTime**, но оба они будут поддерживаться, чтобы обеспечить простую миграцию для клиентов. В течение следующих нескольких месяцев старое свойство **refreshTokensValidFromDateTime** будет удалено.|
| Дополнение | Бета | Добавлено действие **revokeSignInSessions** для ресурса [user](/graph/api/resources/user?view=graph-rest-beta). Это переименование действия **invalidateAllRefreshTokens**, но оба служебных действия будут поддерживаться, чтобы обеспечить простую миграцию для клиентов. В течение следующих нескольких месяцев старое служебное действие **invalidateAllRefreshTokens** будет удалено. |
| Дополнение | Бета-версия |Добавлен новый тип ресурса [trustFrameworkPolicy](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta) для поддержки [Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/active-directory-b2c-overview). Этот тип ресурса поддерживает операции [создания](/graph/api/trustframework-post-trustframeworkpolicy?view=graph-rest-beta), [перечисления](/graph/api/trustframework-list-trustframeworkpolicies?view=graph-rest-beta), [получения](/graph/api/trustframeworkpolicy-get?view=graph-rest-beta), [обновления](/graph/api/trustframework-put-trustframeworkpolicy?view=graph-rest-beta) и [удаления](/graph/api/trustframerkpolicy-delete?view=graph-rest-beta).|

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | Бета-версия          | Добавлена поддержка нового [разрешения Mail.ReadBasic (предварительная версия)](permissions-reference.md#mail-permissions) для интерфейсов [Список сообщений](/graph/api/user-list-messages?view=graph-rest-beta) и [Получение сообщений](/graph/api/message-get?view=graph-rest-beta).            |
| Дополнение        | Бета-версия          | Добавлена возможность [получения содержимого MIME сообщения](outlook-get-mime-message.md). |
| Дополнение        | Бета          | Добавлена возможность [получения необработанного содержимого вложенного файла или элемента](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment) для события, сообщения, задачи Outlook или записи группы. |

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |1.0 | Добавлена поддержка разрешений приложений для ресурса [installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-1.0).|
|Дополнение |1.0| Добавлены свойства **email** и **webUrl** для [канала](/graph/api/resources/channel?view=graph-rest-1.0).|
|Дополнение | бета | Добавлены ресурсы [чата](/api-reference/beta/resources/chat.md) и соответствующие методы. |
|Дополнение |Бета| Добавлены API для просмотра [изображений](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta) в сообщениях.|
|Дополнение | бета | Добавлены ресурсы [участника беседы](/api-reference/beta/resources/conversationmember.md) и соответствующие методы. |


## <a name="march-2019"></a>Март 2019 г.

### <a name="calendar-outlook"></a>Календарь (Outlook)
| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение | 1.0 | Добавлено действие [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) и сложные типы [freeBusyError](/graph/api/resources/freebusyerror?view=graph-rest-1.0), [scheduleInformation](/graph/api/resources/scheduleinformation?view=graph-rest-1.0) и [scheduleItem](/graph/api/resources/scheduleitem?view=graph-rest-1.0) для поддержки [получения сведений о доступности пользователей, списков рассылки и ресурсов для указанного периода времени](outlook-get-free-busy-schedule.md). |
|Изменение | бета | Откат изменений типа, связанных с [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-beta), которые представлены в [феврале 2019 г](#february-2019). Конкретные изменения перечислены в строках ниже.|
|Изменение | Бета | Изменен тип данных для следующих параметров [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-beta): <br>**attendees**: с **attendeeDataModel** откат на [attendeeBase](/graph/api/resources/attendeebase?view=graph-rest-beta) <br>**locationConstraint**: с **locationConstraints** откат на [locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-beta) <br> **timeConstraint**: с **findMeetingTimesTimeConstraints** откат на [timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-beta)|
|Изменение | Бета | Изменен возвращаемый тип **findMeetingTimes** с **findMeetingTimesResponse** обратно на [meetingTimeSuggestionsResult](/graph/api/resources/meetingTimeSuggestionsResult?view=graph-rest-beta) |
|Изменение | бета | Изменен базовый тип [locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-beta) с **locationDataModel** обратно на [location](/graph/api/resources/location?view=graph-rest-beta) |
|Изменение | Бета | Изменены типы данных следующих параметров [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta): <br> **attendeeAvailability**: с коллекции **attendeeAvailabilityDataModel** откат на коллекцию [attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-beta) <br> **locations**: с коллекции **locationDataModel** откат на коллекцию [location](/graph/api/resources/location?view=graph-rest-beta) <br> **meetingTimeSlot**: с **meetingTimeSlotDataModel** откат на [timeSlot](/graph/api/resources/timeslot?view=graph-rest-beta) <br> **organizerAvailability**: с **availabilityStatus** откат на **freeBusyStatus** |
|Удаление | бета | Сложные типы: <br> **attendeeAvailabilityDataModel** <br> **attendeeDataModel** <br> **findMeetingTimesResponse** <br> **findMeetingTimesTimeConstraints** <br> **locationConstraints** <br> **meetingTimeSlotDataModel** <br> **searchWindowTimeSlot**|
|Удаление | бета | Перечисления: <br> **addressType** <br> **availabilityStatus** |
|Дополнение | бета | Восстановлены следующие сложные типы: <br> [attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-beta) <br> [locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-beta) <br> [meetingTimeSuggestionsResult](/graph/api/resources/meetingtimesuggestionsresult?view=graph-rest-beta) <br>[timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-beta) |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[windowsHealthMonitoringConfiguration](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringconfiguration?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[windowsFirewallRule](/graph/api/resources/intune-deviceconfig-windowsfirewallrule?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[androidManagedAppSafetyNetAppsVerificationType](/graph/api/resources/intune-mam-androidmanagedappsafetynetappsverificationtype?view=graph-rest-beta)<br/>[androidManagedAppSafetyNetDeviceAttestationType](/graph/api/resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype?view=graph-rest-beta)<br/>[windowsAutopilotDeviceType](/graph/api/resources/intune-enrollment-windowsautopilotdevicetype?view=graph-rest-beta)<br/>[windowsFirewallRuleInterfaceTypes](/graph/api/resources/intune-deviceconfig-windowsfirewallruleinterfacetypes?view=graph-rest-beta)<br/>[windowsFirewallRuleNetworkProfileTypes](/graph/api/resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes?view=graph-rest-beta)<br/>[windowsFirewallRuleTrafficDirectionType](/graph/api/resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype?view=graph-rest-beta)<br/>[windowsHealthMonitoringScope](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringscope?view=graph-rest-beta)<br/>[windowsUpdateNotificationDisplayOption](/graph/api/resources/intune-deviceconfig-windowsupdatenotificationdisplayoption?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлено действие [searchExistingIdentities](o:searchExistingIdentities:Collection(microsoft.graph.importedDeviceIdentity)) для коллекции [importedDeviceIdentity](/graph/api/resources/intune-enrollment-importeddeviceidentity?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [assignResourceAccountToDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice?view=graph-rest-beta) для объекта [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [unassignResourceAccountFromDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice?view=graph-rest-beta) для объекта [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) |
|Удаление|бета|Удалены следующие типы перечисления:<br/>**defenderScheduleScanDay**;<br/>|
|Дополнение|бета|Добавлены свойства **requiredAndroidSafetyNetDeviceAttestationType**, **appActionIfAndroidSafetyNetDeviceAttestationFailed**, **requiredAndroidSafetyNetAppsVerificationType** и **appActionIfAndroidSafetyNetAppsVerificationFailed** для объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **supportsOemConfig** для объекта [androidManagedStoreApp](/graph/api/resources/intune-apps-androidmanagedstoreapp?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **appSupportsOemConfig** для объекта [androidManagedStoreAppConfiguration](/graph/api/resources/intune-apps-androidmanagedstoreappconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **requiredAndroidSafetyNetDeviceAttestationType**, **appActionIfAndroidSafetyNetDeviceAttestationFailed**, **requiredAndroidSafetyNetAppsVerificationType** и **appActionIfAndroidSafetyNetAppsVerificationFailed** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **iCloudStorageDisabled** и **chooseYourLockScreenDisabled** для объекта [depMacOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depmacosenrollmentprofile?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **roleScopeTagIds** для объекта [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **allowedOutboundClipboardSharingExceptionLength** для объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **fastFirstSignIn** для объекта [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **fastFirstSignIn** для объекта [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **firewallRules** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **authenticationWebSignIn**, **privacyDisableLaunchExperience** и **appManagementPackageFamilyNamesToLaunchAfterLogOn** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **defenderScheduleScanDay** объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **deviceType** для объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **resourceName**, **skuNumber**, **systemFamily**, **azureActiveDirectoryDeviceId** и **managedDeviceId** для объекта [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)|
|Удаление|Бета|Удалено свойство **edgeKioskResetAfterIdleTimeInMinutes** объекта [windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **userWindowsUpdateScanAccess** и **updateNotificationLevel** для объекта [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **teams** для сложного типа [excludedApps](/graph/api/resources/intune-apps-excludedapps?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **autoLaunch** для сложного типа [windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta)|
|Дополнение|Бета|Добавлено свойство **allowAccessToDownloadsFolder** для сложного типа [windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **lowSecurityBiometric** для типа перечисления [androidDeviceOwnerRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype?view=graph-rest-beta)|
|Дополнение|бета|Добавлены элементы **androidBootloaderUnlocked** и **androidFactoryRomModified** для типа перечисления [managedAppFlaggedReason](/graph/api/resources/intune-mam-managedappflaggedreason?view=graph-rest-beta)|

### <a name="education"></a>Образование
| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавление нового ресурса [educationCategory](/graph/api/resources/educationCategory?view=graph-rest-beta).|
| Дополнение | бета | Добавление API для управления ресурсами [educationCategory](/graph/api/resources/educationCategory?view=graph-rest-beta) в [educationClass](/graph/api/resources/educationClass?view=graph-rest-beta) и [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta).|
| Дополнение | бета | Добавление нового ресурса [educationFormResource](/graph/api/resources/educationFormResource?view=graph-rest-beta).|
| Дополнение | бета | Добавление свойства **recipients** для ресурса [educationAssignmentIndividualRecipient](/graph/api/resources/educationAssignmentIndividualRecipient?view=graph-rest-beta).|

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлено свойство навигации **subscriptions** для объекта [driveItem](/graph/api/resources/driveItem?view=graph-rest-1.0) |
| Дополнение        | бета        | Добавлено свойство **expirationDateTime** для типа DateTimeOffset [driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta). |
| Дополнение        | бета        | Добавлено свойство **password** для строкового типа [driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta). |

### <a name="financials-dynamics-365-business-central"></a>Финансовые показатели (Dynamics 365 Business Central)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | бета          | Добавлены API финансовых показателей для Dynamics 365 Business Central. Дополнительные сведения см. в статье [Справочник по API финансовых показателей](/graph/api/resources/dynamics-graph-reference?view=graph-rest-1.0).|

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | 1.0 | Добавлены свойства **passwordNotificationWindowInDays** и **passwordValidityPeriodInDays** для ресурса [domain](/graph/api/resources/domain?view=graph-rest-1.0).|
| Дополнение | Бета-версия и версия 1.0 | Добавлены свойства **complianceExpirationDateTime**, **profileType** и **systemLabels** свойства для ресурса [device](/graph/api/resources/device?view=graph-rest-1.0).|
| Дополнение | Бета-версия и версия 1.0 | Добавлено свойство **isResourceAccount** для ресурса [user](/graph/api/resources/user?view=graph-rest-1.0).|

### <a name="identity-and-access--identity-protection"></a>Удостоверение и доступ | Защита удостоверений

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |бета| Появился метод [Confirm riskyUsers compromised](/graph/api/resources/riskyusers-confirmcompromised?view=graph-rest-beta), который позволяет администраторам подтверждать компрометацию пользователей в службе "Защита идентификации Azure AD". |
|Дополнение |бета| Появился метод [Dismiss riskyUsers](/graph/api/resources/riskyusers-dismiss?view=graph-rest-beta), который позволяет администраторам отменить отметку "рискованный" для пользователей в службе "Защита идентификации Azure AD". |
|Дополнение |бета| Представлено свойство **isProcessing** для ресурса [riskyUser](/graph/api/resources/riskyuser?view=graph-rest-beta). |

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Удаление |бета| Удалено свойство **deleted** из ресурса [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta). Вместо него можно использовать**deletedDateTime**. |
| Дополнение | бета | Добавлены ресурсы [schedule](/api-reference/beta/resources/schedule.md), [schedulingGroup](/api-reference/beta/resources/schedulinggroup.md), [shift](/api-reference/beta/resources/shift.md), [timeOffReason](/api-reference/beta/resources/timeoffreason.md) и [timeOff](/api-reference/beta/resources/timeoff.md), а также соответствующие методы. |


## <a name="february-2019"></a>Февраль 2019 г.

### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Изменение | Бета | Изменен тип данных для следующих параметров [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-beta): <br>**attendees**: с **attendeeBase** на [attendeeDataModel](/graph/api/resources/attendeedatamodel?view=graph-rest-beta) <br>**locationConstraint**: с **locationConstraint** на [locationConstraints](/graph/api/resources/locationconstraints?view=graph-rest-beta) <br> **timeConstraint**: с **timeConstraint** на [findMeetingTimesTimeConstraints](/graph/api/resources/findmeetingtimestimeconstraints?view=graph-rest-beta)|
|Изменение | Бета | Изменен возвращаемый тип **findMeetingTimes** с **meetingTimeSuggestionsResult** чтобы [findMeetingTimesResponse](/graph/api/resources/findmeetingtimesresponse?view=graph-rest-beta) |
|Изменение | Бета | Изменены полезные данные ответа **findMeetingTimes**, чтобы исключить **тип** каждого присутствующего, который указывает, является ли участник обязательным, необязательным или представляет ресурс |
|Изменение | бета | Изменен базовый тип [locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-beta) с [location](/graph/api/resources/location?view=graph-rest-beta) на [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) |
|Изменение | Бета | Изменены типы данных следующих параметров [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta): <br> **attendeeAvailability**: с коллекции **attendeeAvailability** на коллекцию [attendeeAvailabilityDataModel](/graph/api/resources/attendeeavailabilitydatamodel?view=graph-rest-beta) <br> **locations**: с коллекции [location](/graph/api/resources/location?view=graph-rest-beta) на коллекцию [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) <br> **meetingTimeSlot**: с[timeSlot](/graph/api/resources/timeslot?view=graph-rest-beta) на [meetingTimeSlotDataModel](/graph/api/resources/meetingtimeslotdatamodel?view=graph-rest-beta) <br> **organizerAvailability**: с **freeBusyStatus** на **availabilityStatus** |
|Дополнение | Бета | Новые сложные типы: <br> [attendeeAvailabilityDataModel](/graph/api/resources/attendeeavailabilitydatamodel?view=graph-rest-beta) <br> [attendeeDataModel](/graph/api/resources/attendeedatamodel?view=graph-rest-beta) <br> [findMeetingTimesResponse](/graph/api/resources/findmeetingtimesresponse?view=graph-rest-beta) <br> [findMeetingTimesTimeConstraints](/graph/api/resources/findmeetingtimestimeconstraints?view=graph-rest-beta) <br> [locationConstraints](/graph/api/resources/locationconstraints?view=graph-rest-beta) <br> [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) <br> [meetingTimeSlotDataModel](/graph/api/resources/meetingtimeslotdatamodel?view=graph-rest-beta) <br> [postalAddress](/graph/api/resources/postaladdress?view=graph-rest-beta) <br> [searchWindowTimeSlot](/graph/api/resources/searchwindowtimeslot?view=graph-rest-beta)|
|Дополнение | Бета | Новые перечисления: <br> **addressType** <br> **availabilityStatus** |
|Дополнение | Бета | Добавлено свойство **order** для [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta) |
|Удаление | Бета-версия | Удалены следующие сложные типы: <br> **attendeeAvailability** <br> **locationConstraint** <br> **meetingTimeSuggestionsResult** <br>**timeConstraint** |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidOmaCpConfiguration](/graph/api/resources/intune-deviceconfig-androidomacpconfiguration?view=graph-rest-beta)<br/>[managedDeviceEncryptionState](/graph/api/resources/intune-deviceconfig-manageddeviceencryptionstate?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[deliveryOptimizationBandwidth](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidth?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthAbsolute](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthabsolute?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthBusinessHoursLimit](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthHoursWithPercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthhourswithpercentage?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthPercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthpercentage?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdCustom](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidcustom?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdSource](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidsource?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdSourceOptions](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidsourceoptions?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSize](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesize?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSizeAbsolute](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesizeabsolute?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSizePercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesizepercentage?view=graph-rest-beta)<br/>[encryptionReportPolicyDetails](/graph/api/resources/intune-deviceconfig-encryptionreportpolicydetails?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[advancedBitLockerState](/graph/api/resources/intune-deviceconfig-advancedbitlockerstate?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdOptionsType](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype?view=graph-rest-beta)<br/>[deliveryOptimizationRestrictPeerSelectionByOptions](/graph/api/resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions?view=graph-rest-beta)<br/>[deviceTypes](/graph/api/resources/intune-deviceconfig-devicetypes?view=graph-rest-beta)<br/>[edgeKioskModeRestrictionType](/graph/api/resources/intune-deviceconfig-edgekioskmoderestrictiontype?view=graph-rest-beta)<br/>[encryptionReadinessState](/graph/api/resources/intune-deviceconfig-encryptionreadinessstate?view=graph-rest-beta)<br/>[encryptionState](/graph/api/resources/intune-deviceconfig-encryptionstate?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлено свойство **roleScopeTagIds** для объекта [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **autoFillForceAuthentication**, **cellularBlockPlanModification**, **classroomForceAutomaticallyJoinClasses**, **classroomForceUnpromptedAppAndDeviceLock**, **esimBlockModification**, **proximityBlockSetupToNewDevice**, **softwareUpdatesEnforcedDelayInDays** and **softwareUpdatesForceDelayed** для объекта [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **softwareUpdatesEnforcedDelayInDays**, **softwareUpdatesForceDelayed** и **contentCachingBlocked** для объекта [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **licensingType** для объекта [microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta).|
|Дополнение|бета|Добавлены свойства **defenderSecurityCenterDisableClearTpmUI**, **defenderSecurityCenterDisableNotificationAreaUI**, **defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI**, **defenderAdobeReaderLaunchChildProcess** и **defenderOfficeCommunicationAppsLaunchChildProcess** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **edgeKioskModeRestriction**, **edgeKioskResetAfterIdleTimeInMinutes**, **defenderScheduleScanEnableLowCpuPriority**, **defenderDisableCatchupQuickScan**, **defenderDisableCatchupFullScan** и **edgeBlockSearchEngineCustomization** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|
|Дополнение|бета|Добавлено свойство **enableWhiteGlove** для объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **restrictPeerSelectionBy**, **groupIdSource**, **bandwidthMode**, **backgroundDownloadFromHttpDelayInSeconds**, **foregroundDownloadFromHttpDelayInSeconds**, **minimumRamAllowedToPeerInGigabytes**, **minimumDiskSizeAllowedToPeerInGigabytes**, **minimumFileSizeToCacheInMegabytes**, **minimumBatteryPercentageAllowedToUpload**, **modifyCacheLocation**, **maximumCacheAgeInDays**, **maximumCacheSize** и **vpnPeerCaching** для объекта [windowsDeliveryOptimizationConfiguration](/graph/api/resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration?view=graph-rest-beta).|
|Дополнение|бета|Добавлено свойство **lastCheckInDateTime** для объекта [windowsInformationProtectionWipeAction](/graph/api/resources/intune-mam-windowsinformationprotectionwipeaction?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **managedDeviceEncryptionStates** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **endpointProtection** и **officeApps** для сложного типа [configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-beta)|
|Дополнение|бета|Добавлены свойства **productName** и **publisher** для сложного типа [win32LobAppMsiInformation](/graph/api/resources/intune-apps-win32lobappmsiinformation?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **warn** для типа перечисления [managedAppRemediationAction](/graph/api/resources/intune-mam-managedappremediationaction?view=graph-rest-beta)|

### <a name="education"></a>Образование

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |бета|Представлено новое свойство relatedContacts для ресурса [educationUser](/graph/api/resources/educationUser?view=graph-rest-beta).|
|Дополнение |1.0|Представлено новое свойство relatedContacts для ресурса [educationUser](/graph/api/resources/educationUser?view=graph-rest-1.0).|

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлено свойство **expirationDateTime** для типа DateTimeOffset [driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta). |
| Дополнение        | бета        | Добавлено свойство **password** для строкового типа [driveItem_invite](/graph/api/resources/driveItem_invite?view=graph-rest-beta). |

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | 1.0 | Добавлен новый тип ресурса [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-1.0). |
| Дополнение | Бета-версия и версия 1.0 | Добавлено свойство **createdDateTime** для [organization](/graph/api/resources/organization?view=graph-rest-1.0) |
| Изменение | Бета-версия и версия 1.0 | Обновлено свойство **companyName** ресурса [user](/graph/api/resources/user?view=graph-rest-1.0) для обеспечения возможности записи. |
| Изменение | бета | Тип ресурса [TargetResource](/graph/api/resources/targetresource?view=graph-rest-beta) теперь включает свойства, ранее доступные производным типам, которые больше не поддерживаются. |
| Удаление | бета | Следующие производные типы больше не поддерживаются и были удалены: **targetResourceDevice**, **targetResourceDirectory**, **targetResourceGroup**, **targetResourcePolicy**, **targetResourceRole**, **targetResourceServicePrincipal**, **targetResourceUser**, и **targetResourceOther**. |
| Дополнение |бета | Добавлены свойства **passwordNotificationWindowInDays** и **passwordValidityPeriodInDays** для ресурса [domain](/graph/api/resources/domain?view=graph-rest-beta).|

### <a name="notes-onenote"></a>Заметки (OneNote)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | Бета-версия и версия 1.0 | Добавлен метод [getNotebookFromWebUrl](/graph/api/notebook-getnotebookfromweburl?view=graph-rest-1.0). |

### <a name="security"></a>Безопасность

| **Тип изменения** | **Версия** | **Описание**              |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета       | Добавлены API индикаторов аналитики угроз (TI) для [API безопасности](/graph/api/resources/security-api-overview?view=graph-rest-beta), включающие указанные ниже ресурсы и операции:<br/>[tiindicator](/graph/api/resources/tiindicator?view=graph-rest-beta) (и связанные объекты)<br/> [Получение объекта tiIndicator](/graph/api/tiindicator-get?view=graph-rest-beta)<br/>[Создание объекта tiIndicator](/graph/api/tiindicators-post?view=graph-rest-beta)<br/>[Перечисление объектов tiIndicator](/graph/api/tiindicators-list?view=graph-rest-beta)<br/>[Обновление объекта tiIndicator](/graph/api/tiindicator-update?view=graph-rest-beta) <br/>[Удаление объекта tiIndicator](/graph/api/tiindicator-delete?view=graph-rest-beta) <br/>[deleteTiIndicators](/graph/api/tiindicator-deletetiindicators?view=graph-rest-beta) <br/>[deleteTiIndicatorsByExternalId](/graph/api/tiindicator-deletetiindicatorsbyexternalid?view=graph-rest-beta) <br/>[submitTiIndicators](/graph/api/tiindicator-submittiindicators?view=graph-rest-beta) <br/>[updateTiIndicators](/graph/api/tiindicator-updatetiindicators?view=graph-rest-beta)|
| Дополнение        | бета       | Добавлены API действия безопасности для [API безопасности](/graph/api/resources/security-api-overview?view=graph-rest-beta), включающие указанные ниже ресурсы и операции:<br/>[securityAction](/graph/api/resources/securityaction?view=graph-rest-beta) (и связанные объекты)<br/> [Получение объекта securityAction](/graph/api/securityaction-get?view=graph-rest-beta)<br/>[Создание объекта securityAction](/graph/api/securityactions-post?view=graph-rest-beta)<br/>[Перечисление объектов securityAction](/graph/api/securityactions-list?view=graph-rest-beta)<br/>[Отмена объекта securityAction](/graph/api/securityaction-cancelsecurityaction?view=graph-rest-beta)
| Дополнение        | бета        | Представлен новый сложный тип: коллекция [historyStates](/graph/api/resources/alerthistorystate?view=graph-rest-beta) для оповещений. </br>Добавлена функция [updateAlerts](/graph/api/alert-updatealerts?view=graph-rest-beta) для обновления нескольких оповещений в одном запросе. |

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |Бета-версия и версия 1.0| Добавлено свойство **internalId** для ресурса [team](/graph/api/resources/team?view=graph-rest-1.0).|
|Дополнение |Бета-версия и версия 1.0| Добавлена поддержка для настройки Word, Excel, PowerPoint, PDF и [вкладок](teams-configuring-builtin-tabs.md) библиотек документов. |
|Дополнение |бета| Представлен API [отправки сообщения в канал](/graph/api/channel-post-chatmessage?view=graph-rest-beta). |
|Дополнение |бета| Представлен API [ответа на сообщение в канале](/graph/api/channel-post-messagereply?view=graph-rest-beta). |
|Удаление |бета| Удален API POST /teams/{id}/channels/{id}/chatThreads. Вместо этого можно использовать [Создание сообщения в канале](/graph/api/channel-post-chatmessage?view=graph-rest-beta). |
|Дополнение |бета | Добавлена поддержка разрешений приложений для ресурса [installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta).|


## <a name="january-2019"></a>Январь 2019 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[appleVppTokenTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-applevpptokentroubleshootingevent?view=graph-rest-beta)<br/>[appLogCollectionRequest](/graph/api/resources/intune-devices-applogcollectionrequest?view=graph-rest-beta)<br/>[windowsUpdateState](/graph/api/resources/intune-deviceconfig-windowsupdatestate?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[appLogCollectionDownloadDetails](/graph/api/resources/intune-devices-applogcollectiondownloaddetails?view=graph-rest-beta)<br/>**deviceManagementTroubleshootingErrorDetails**<br/>[deviceManagementTroubleshootingErrorResource](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource?view=graph-rest-beta)<br/>[win32LobAppAssignmentSettings](/graph/api/resources/intune-apps-win32lobappassignmentsettings?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[appLogDecryptionAlgorithm](/graph/api/resources/intune-devices-applogdecryptionalgorithm?view=graph-rest-beta)<br/>[appLogUploadState](/graph/api/resources/intune-devices-apploguploadstate?view=graph-rest-beta)<br/>[win32LobAppNotification](/graph/api/resources/intune-apps-win32lobappnotification?view=graph-rest-beta)<br/>[windowsUpdateStatus](/graph/api/resources/intune-deviceconfig-windowsupdatestatus?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлено действие **createDownloadUrl** для объекта [appLogCollectionRequest](/graph/api/resources/intune-devices-applogcollectionrequest?view=graph-rest-beta) |
|Удаление|Бета|Удалены следующие объекты:<br/>**deviceManagementApplicabilityRuleOsEdition**<br/>**deviceManagementApplicabilityRuleOsVersion**<br/>|
|Дополнение|бета|Добавлено свойство **passwordSignInFailureCountBeforeFactoryReset** для объекта [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **passwordSignInFailureCountBeforeFactoryReset** для объекта [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **passwordSignInFailureCountBeforeFactoryReset** для объекта [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta)|
|Удаление|бета|Удалено свойство **defaultProfileDisplayName** из объекта [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **runAs32Bit** для объекта [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta).|
|Дополнение|бета|Добавлены свойства **troubleshootingErrorDetails**, **eventName** и **additionalInformation** для объекта [deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-beta)|
|Изменение|бета|Изменены следующие свойства объекта [macOSCertificateProfileBase](/graph/api/resources/intune-deviceconfig-macoscertificateprofilebase?view=graph-rest-beta):<br/>свойство **subjectAlternativeNameType** преобразовано из обязательного в необязательное<br/>|
|Дополнение|бета|Добавлены свойства **certificateStore** и **customSubjectAlternativeNames** для объекта [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **officeConfigurationXml** для объекта [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **createdDateTime** для объекта [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **bitLockerAllowStandardUserEncryption** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Удаление|бета|Удалены свойства **localSecurityOptionsEnableAdministratorAccount**, **localSecurityOptionsEnableGuestAccount** и **lanManagerWorkstationEnableInsecureGuestLogons** из объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **useSecurityKeyForSignin** для объекта [windowsIdentityProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsidentityprotectionconfiguration?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **mobileAppTroubleshootingEvents** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство навигации **appLogCollectionRequests** для объекта [mobileAppTroubleshootingEvent](/graph/api/resources/intune-devices-mobileapptroubleshootingevent?view=graph-rest-beta)|

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |1.0|С целью поддержки конфигурирования поставщика удостоверений в клиенте Azure AD B2C представлен новый тип ресурса [identityProvider](/graph/api/resources/identityprovider?view=graph-rest-1.0) и операции [create](/graph/api/identityprovider-post-identityproviders?view=graph-rest-1.0), [list](/graph/api/identityprovider-list?view=graph-rest-1.0), [get](/graph/api/identityprovider-get?view=graph-rest-1.0), [update](/graph/api/identityprovider-update?view=graph-rest-1.0) и [delete](/graph/api/identityprovider-delete?view=graph-rest-1.0).|

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | 1.0 | Добавлен новый метод transitiveMembers для объекта [groups](/graph/api/group-list-transitivemembers?view=graph-rest-1.0). Этот метод возвращает плоский список элементов, включая вложенные элементы.|
| Дополнение | 1.0 | Добавлен новый метод transitiveMemberOf для объектов [users](/graph/api/user-list-transitivemembersof?view=graph-rest-1.0), [groups](/graph/api/group-list-transitivemembersof?view=graph-rest-beta) и [devices](/graph/api/device-list-transitivemembersof?view=graph-rest-1.0).|
| Дополнение | 1.0 | Добавлены новые свойства в объект [users](/graph/api/resources/user?view=graph-rest-1.0): **employeeId**, **faxNumber**, **onPremisesDistinguishedName**, **showInAddressList** и **otherMails**.|
| Дополнение | 1.0 | Добавлено свойство **forceChangePasswordNextSignInWithMfa** в сложный тип [passwordProfile](/graph/api/resources/passwordprofile?view=graph-rest-1.0).|
| Дополнение | 1.0 | Добавлено свойство **licenseAssignmentStates** в объект [User](/graph/api/resources/user?view=graph-rest-1.0) для [лицензирования на основе групп](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|
| Дополнение | 1.0 | Добавлен ресурс **licenseAssignmentState** для [лицензирования на основе групп](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|
| Дополнение | 1.0 | Добавлены свойства **assignedLicenses**, **licenseProcessingState** и **hasMembersWithLicenseErrors** и связь **membersWithLicenseErrors** в объект [Group](/graph/api/resources/group?view=graph-rest-1.0) для [лицензирования на основе групп](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|
| Дополнение | Бета | Добавлено свойство **createdDateTime** для ресурса [user](/graph/api/resources/user?view=graph-rest-beta).|

### <a name="reports"></a>Отчеты

| **Тип изменения** | **Версия** | **Описание**                  |
|:----------------|:------------|:-----------------------------------------|
| Дополнение        | бета  | Добавлены свойства **office365Active** и **office365Inactive** для объекта [office365ServicesUserCounts](/graph/api/resources/office365ServicesUserCounts?view=graph-rest-beta).|

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |Бета| Добалены элементы educationStandard, educationClass, educationProfessionalLearningCommunity, educationStaff и unknownFutureValue в перечисление [teamSpecialization](/graph/api/resources/teamspecialization?view=graph-rest-beta).|


## <a name="december-2018"></a>Декабрь 2018 г.

### <a name="identity-and-access--data-policy-operation"></a>Удостоверение и доступ | Операция с политикой данных

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Дополнение |1.0| Добавлен новый объект [dataPolicyOperation](/graph/api/resources/datapolicyoperation?view=graph-rest-1.0). Он представляет собой отправленную операцию с политикой данных с целью отслеживания.
|Дополнение |1.0| Добавлено действие [exportPersonalData](/graph/api/user-exportpersonaldata?view=graph-rest-1.0) для [пользователей](/graph/api/resources/users?view=graph-rest-1.0). Это действие отправляет запрос на экспорт персональных данных, которые корпорация Майкрософт хранит для пользователя. |
|Дополнение |1.0| Добавлен метод [dataPolicyOperations](/graph/api/datapolicyoperation-get?view=graph-rest-1.0). Он извлекает свойства объекта dataPolicyOperation.|

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлено новое свойство `expirationDateTime` в [группы](https://docs.microsoft.com/graph/api/resources/group?view=graph-rest-beta) для [срока действия группы](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-lifecycle).|
| Дополнение | Бета | Добавлен новый тип ресурса [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).|
| Дополнение | бета | Добавлено свойство `createdDateTime` для ресурса [organization](/graph/api/resources/organization?view=graph-rest-beta).|
| Дополнение | 1.0 | Добавлен метод `memberOf` для получения сведений о непосредственном [участии](/graph/api/device-list-memberOf?view=graph-rest-1.0) для [устройств](/graph/api/resources/device?view=graph-rest-1.0). Этот метод был добавлен для получения списка участий, включая вложенные участия.|
| Изменение    | бета | Изменена структура ресурса [контактов организации](/graph/api/resources/orgcontact?view=graph-rest-beta). Свойства физических адресов (`city`, `country`, `postalCode`, `streetAddress` и `state`) и `officeLocation` теперь находятся в коллекции `addresses` (нового типа ресурса [physicalOfficeAddress](/graph/api/resources/physicalofficeaddress?view=graph-rest-beta)), а `mobilePhone`, `businessPhones` и `faxNumber` теперь находятся в коллекции `phones`. Также добавлены объекты `companyName` и `imAddresses`|

### <a name="identity-and-access--privileged-identity-management"></a>Удостоверение и доступ | Управление привилегированными пользователями (PIM)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлено свойство `registeredRoot` для объекта [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta).|
| Изменение | бета | Переименовано свойство `onboardDateTime` объекта [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) для `registeredDateTime`.|
| Дополнение | Бета | Добавлено новое действие [регистрация ресурсов](/graph/api/governanceresource-register?view=graph-rest-beta).|
| Удаление | бета | Удалено свойство`isPermanent` для объекта [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta).|
| Удаление | бета | Удалено свойство `roleAssignmentStartDateTime` для объекта [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta).|
| Удаление | бета | Удалено свойство `roleAssignmentEndDateTime` для объекта [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta).|

### <a name="security"></a>Безопасность

| **Тип изменения** | **Версия** | **Описание**              |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Представлен новый сложный тип [complianceInformation](/graph/api/complianceInformation/team?view=graph-rest-beta).|
| Дополнение        | бета        | Представлен новый сложный тип [certificationControl](/graph/api/certificationControl/team?view=graph-rest-beta).|

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |бета| Представлен новый тип ресурса [teamsTemplate](/graph/api/resources/teamstemplate?view=graph-rest-beta).|
|Дополнение |Бета| Представлен новый тип ресурса [teamSpecialization](/graph/api/resources/teamspecialization?view=graph-rest-beta).|
|Дополнение |Бета| Добавлены свойства isFavoriteByDefault, email и webUrl для [канала](/graph/api/resources/channel?view=graph-rest-beta).|
|Дополнение |Бета| Добавлено свойство displayName для [команды](/graph/api/resources/team?view=graph-rest-beta)|
|Дополнение |бета| Добавлено свойство описания для [команды](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |Бета| Добавлено свойство классификации для [команды](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |бета| Добавлено свойство [specialization](/graph/api/resources/teamspecialization?view=graph-rest-beta) для [команды](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |бета| Добавлено свойство [видимость](/graph/api/resources/teamvisibilitytype?view=graph-rest-beta) для [группы](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |бета| Добавлено свойство [шаблон](/graph/api/resources/teamstemplate?view=graph-rest-beta) для [группы](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |бета| Добавлено семейство владельцы для [группы](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение |бета| Представлен новый элемент перечисления unknownFutureValue для объекта teamVisibilityType.|
|Дополнение |бета| Представлен новый элемент перечисления unknownFutureValue для объекта giphyRatingType.|
|Дополнение |бета| Представлен новый элемент перечисления unknownFutureValue для объекта teamsAsyncOperationType.|
|Дополнение |бета| Представлен новый элемент перечисления unknownFutureValue для объекта teamsAsyncOperationStatus.|
|Дополнение |бета| Представлен новый элемент перечисления unknownFutureValue для объекта teamsAppDistributionMethod.|
|Дополнение |Бета| Представлен новый тип ресурса [/teamsTemplates](/graph/api/resources/teamstemplate?view=graph-rest-beta).|
|Дополнение | 1.0 | Добавлена поддержка разрешений администратора для операций c [командами](/graph/api/resources/team?view=graph-rest-1.0), [каналами](/graph/api/resources/channel?view=graph-rest-1.0) и [вкладками](/graph/api/resources/teamstab?view=graph-rest-1.0). |


## <a name="november-2018"></a>Ноябрь 2018 г.

### <a name="identity-and-access--data-policy-operations"></a>Удостоверение и доступ | Операции с политикой данных

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлено новое свойство **progress** для [dataPolicyOperation](/graph/api/resources/dataPolicyOperation?view=graph-rest-beta). Оно указывает ход выполнения операции.

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | 1.0 | Добавлено действие [forceDelete](/graph/api/domain-forcedelete?view=graph-rest-1.0) для объекта [domains](/graph/api/resources/domain?view=graph-rest-1.0).|
| Дополнение | бета | Добавлен новый метод transitiveMembers для объекта [groups](/graph/api/group-list-transitivemembers?view=graph-rest-beta). Этот метод возвращает плоский список элементов, включая вложенные элементы.|
| Дополнение | бета | Добавлен новый метод transitiveMemberOf для объектов [users](/graph/api/user-list-transitivemembersof?view=graph-rest-beta), [groups](/graph/api/group-list-transitivemembersof?view=graph-rest-beta), [devices](/graph/api/device-list-transitivemembersof?view=graph-rest-beta) и [service principals](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta).|
| Дополнение | бета | Добавлен метод memberOf, чтобы получить сведения о непосредственном [участии](/graph/api/device-list-members?view=graph-rest-beta) для устройств. Этот метод добавлен для получения списка участий, включая вложенные участия.|
| Дополнение | бета | Добавлены новые свойства в объект [users](/graph/api/resources/user?view=graph-rest-beta): **faxNumber**, **onPremisesDistinguishedName** и **otherMails**.|
| Дополнение | бета | Добавлено свойство **forceChangePasswordNextSignInWithMfa** в сложный тип [passwordProfile](/graph/api/resources/passwordprofile?view=graph-rest-beta).|
| Дополнение    | бета | Добавлены свойства externalUserState и externalUserStateChangeDateTime в объект [user](/graph/api/resources/user?view=graph-rest-beta).|

### <a name="reports"></a>Отчеты

| Тип изменения | Версия                                    | Описание                              |
| :---------- | :----------------------------------------- | :--------------------------------------- |
| Дополнение    | Бета-версия Microsoft Graph для Китая под управлением 21Vianet | Добавлены следующие API:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta);<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta);<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta);<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta);<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta);<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta);<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta);<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta);<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta);<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta);<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta);<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta);<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta);<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta);<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta);<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta);<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta);<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta);<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta);<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta);<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta);<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta);<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta);<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta);<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta);<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta);<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta);<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta);<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta);<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta);<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta);<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta);<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta);<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta);<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta);<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta);<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta). |

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

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
|Удаление |Бета| teamsCatalogAppDistributionMethod переименован на teamsAppDistributionMethod  |
|Дополнение |бета| Представлен объект [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta), заменяющий /teams/{id}/apps с некоторыми отличиями в полезных данных. |
|Дополнение |бета| Добавлено свойство displayName в объект [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) |
|Дополнение |бета| Добавлено свойство messageId в объект [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) |
|Дополнение |Бета| Добавлено свойство teamsApp в объект [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) |
|Дополнение |Бета| Представлен новый тип ресурса [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta).|
|Дополнение |бета| Представлен новый тип ресурса [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta).|
|Дополнение |бета| Представлен новый тип ресурса [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta).|
|Дополнение |бета| Представлен новый элемент перечисления hiddenMembership для объекта teamVisibilityType.|
|Дополнение |Бета| Представлен новый элемент перечисления createTeam для объекта teamsAsyncOperationType.|
|Дополнение |бета| Представлен новый элемент перечисления teamsAppDistributionMethod.|
|Дополнение |бета| Представлено новое действие обновления приложения в [/teams/{id}/installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta). |


## <a name="october-2018"></a>Октябрь 2018 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлено свойство **tenantLockdownRequireNetworkDuringOutOfBoxExperience** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0)|
|Дополнение|1.0|Добавлено свойство **v12_0** для сложного типа [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0)|
|Дополнение|Бета|Добавлено свойство **lastReportAggregationDateTime** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены новые объекты:<br/>[intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[deviceAndAppManagementAssignedRoleIds](/graph/api/resources/intune-rbac-deviceandappmanagementassignedroleids?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[applicationGuardEnabledOptions](/graph/api/resources/intune-deviceconfig-applicationguardenabledoptions?view=graph-rest-beta)<br/>[autoRestartNotificationDismissalMethod](/graph/api/resources/intune-deviceconfig-autorestartnotificationdismissalmethod?view=graph-rest-beta)<br/>[meteredConnectionLimitType](/graph/api/resources/intune-deviceconfig-meteredconnectionlimittype?view=graph-rest-beta)<br/>|
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

### <a name="identity-and-access--audit-logs"></a>Удостоверение и доступ | Журналы аудита

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Изменение   |бета| Свойство `conditionalAccessPolicies` переименовано на `appliedConditionalAccessPolicy`.|
|Дополнение |бета| Представлены дополнительные свойства риска в [API входа](/graph/api/resources/signin?view=graph-rest-beta), в том числе `riskDetail`, `riskLevelAggregated`, `riskLevelDuringSignIn`, `riskEventTypes` и `riskState`.|
|Дополнение |бета| Представлены дополнительные свойства входа в [API входа](/graph/api/resources/signin?view=graph-rest-beta), в том числе `authenticationProcessingDetails`, `originalRequestID`, `isInteractive`, `tokenIssuerName`, `tokenIssuerType`, `correlationId` и `processingTimeinMilliseconds`.|
|Удаление   |бета| Удалено свойство `isRisky`.|

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлен новый метод transitiveMembers для объекта [groups](/graph/api/group-list-transitivemembers?view=graph-rest-beta). Этот метод возвращает плоский список элементов, включая вложенные элементы.|
| Дополнение | бета | Добавлен новый метод transitiveMemberOf для объектов [users](/graph/api/user-list-transitivemembersof?view=graph-rest-beta), [groups](/graph/api/group-list-transitivemembersof?view=graph-rest-beta), [devices](/graph/api/device-list-transitivemembersof?view=graph-rest-beta) и [service principals](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta).|
| Дополнение | бета | Добавлен метод memberOf, чтобы получить сведения о непосредственном [участии](/graph/api/device-list-members?view=graph-rest-beta) для устройств. Этот метод добавлен для получения списка участий, включая вложенные участия.|
| Дополнение | бета | Добавлены новые свойства в объект [users](/graph/api/resources/user?view=graph-rest-beta): **faxNumber**, **onPremisesDistinguishedName** и **otherMails**.|
| Дополнение | бета | Добавлено свойство **licenseAssignmentStates** в объект [User](/graph/api/resources/user?view=graph-rest-beta) для [лицензирования на основе групп](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|
| Дополнение | бета | Добавлен ресурс **licenseAssignmentState** для [лицензирования на основе групп](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|
| Дополнение | Бета | Добавлены свойства **assignedLicenses**, **licenseProcessingState**, **hasMembersWithLicenseErrors** и **membersWithLicenseErrors** в объект [Group](/graph/api/resources/group?view=graph-rest-beta) для [лицензирования на основе групп](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|

### <a name="identity-and-access--identity-protection"></a>Удостоверение и доступ | Защита удостоверений

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение |бета| Добавлен [API riskyUsers](/graph/api/resources/riskyuser?view=graph-rest-beta), представляющий пользователей Azure AD в состоянии риска, как определено защитой идентификации Azure AD. |

### <a name="identity-and-access--privileged-identity-management"></a>Удостоверение и доступ | Управление привилегированными пользователями (PIM)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение | бета | Изменен объект [privilegedapproval](/graph/api/resources/privilegedapproval?view=graph-rest-beta).|
| Дополнение | бета | Добавлен объект [privilegedroleassignmentrequest](/graph/api/resources/privilegedroleassignmentrequest?view=graph-rest-beta), а также следующие методы и действия:<br> [Перечисление](/graph/api/privilegedroleassignmentrequest-list?view=graph-rest-beta) <br> [Create](/graph/api/privilegedroleassignmentrequest-post?view=graph-rest-beta) <br> [Cancel](/graph/api/privilegedroleassignmentrequest-cancel?view=graph-rest-beta) <br> [My](/graph/api/privilegedroleassignmentrequest-my?view=graph-rest-beta) |
| Дополнение | бета | Добавлено [Update](/graph/api/privilegedrolesettings-update?view=graph-rest-beta) для [privilegedRoleSettings](/graph/api/resources/privilegedrolesettings?view=graph-rest-beta)|
| Удаление |бета| Удалена [самостоятельная активация назначения ролей](/graph/api/privilegedrole_selfactivate?view=graph-rest-beta)|

### <a name="personal-contacts-outlook"></a>Личные контакты (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Удаление         | 1.0        | Это исправление в документации: удалено свойство **flag** из статьи по объекту [contact](/graph/api/resources/contact?view=graph-rest-1.0). Свойство никогда не было доступным в объекте **contact**.|

### <a name="reports"></a>Отчеты
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | 1.0    | Добавлено свойство **Site ID** для объекта [getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0). |

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение|бета|Добавлена поддержка разрешений приложений для API [архивации объекта команды](/graph/api/team-archive?view=graph-rest-beta) и [распаковки объекта команды](/graph/api/team-unarchive?view=graph-rest-beta).|

### <a name="track-changes"></a>Отслеживание изменений

| **Тип изменения** | **Версия** | **Описание**                  |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | бета   | Добавлена возможность [запроса изменений](delta-query-overview.md) для объекта [directoryObject](/graph/api/directoryobject-delta?view=graph-rest-beta) |
| Изменение      | 1.0 и бета  | Другое поведение при возвращении измененных свойств только в отклике JSON для объектов [users](/graph/api/user-delta?view=graph-rest-1.0) и [groups](/graph/api/group-delta?view=graph-rest-1.0). |
| Дополнение    | 1.0   | Добавлена функция [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) для [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0), чтобы поддерживать [отслеживание изменений с помощью запроса изменений](delta-query-overview.md). |


## <a name="september-2018"></a>Сентябрь 2018 г.

### <a name="calls-and-online-meetings"></a>Звонки и собрания по сети

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | бета        | Ресурс [application](/graph/api/resources/application?view=graph-rest-beta) обновлен для добавления коллекции звонков. |
| Изменение          | бета        | Ресурс [operation](/graph/api/resources/operation?view=graph-rest-beta) обновлен для поддержки API продолжительных звонков и собраний по сети. |
| Дополнение        | Бета-версия        | Добавлен ресурс [call](/graph/api/resources/call?view=graph-rest-beta) для управления голосовыми и видеозвонками (изначально в Microsoft Teams), включая API для [создания](/graph/api/application-post-calls?view=graph-rest-beta), [получения](/graph/api/call-get?view=graph-rest-beta) и [удаления (завершения) звонков](/graph/api/call-delete?view=graph-rest-beta), [ответа на звонок](/graph/api/call-answer?view=graph-rest-beta), а также [отклонения](/graph/api/call-reject?view=graph-rest-beta), [перенаправления](/graph/api/call-redirect?view=graph-rest-beta) и [передачи звонка](/graph/api/call-transfer?view=graph-rest-beta). Мы также расширили API для поддержки [сценариев IVR](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta): [воспроизведение запроса](/graph/api/call-playprompt?view=graph-rest-beta), [запись звонка](/graph/api/call-record?view=graph-rest-beta), [отмена обработки мультимедиа](/graph/api/call-cancelmediaprocessing?view=graph-rest-beta) и [подписка на тональные уведомления](/graph/api/call-subscribetotone?view=graph-rest-beta). |
| Дополнение        | бета        | Добавлен ресурс [participant](/graph/api/resources/call?view=graph-rest-beta) и API для управления участниками в голосовых и видеозвонках и собраниях, в том числе [получение объекта participant](/graph/api/participant-get?view=graph-rest-beta), [настройка звукового микшера для участника](/graph/api/participant-configuremixer?view=graph-rest-beta), отключение звука [одного](/graph/api/participant-mute?view=graph-rest-beta) или [всех](/graph/api/participant-muteall?view=graph-rest-beta) участников, [получение списка участников](/graph/api/call-list-participants?view=graph-rest-beta) в звонке или собрании и [приглашение участников](/graph/api/participant-invite?view=graph-rest-beta) в звонок или собрание. |
| Дополнение        | бета        | Добавлены API для приложений по управлению и участию в звонках и собраниях, включая возможность [делиться контентом](/graph/api/call-changescreensharingrole?view=graph-rest-beta), [самостоятельно отключать и включать звук](/graph/api/call-unmute?view=graph-rest-beta) и [обновлять метаданные, связанные со звонком](/graph/api/call-updatemetadata?view=graph-rest-beta). |
| Дополнение        | бета        | Добавлен ресурс [audio routing group](/graph/api/resources/audioroutinggroup?view=graph-rest-beta) и API для управления частными звуковыми маршрутами между участниками многосторонней беседы, включая [создание групп маршрутизации звука](/graph/api/call-post-audioroutinggroups?view=graph-rest-beta), [получение их списка](/graph/api/audioroutinggroup-get?view=graph-rest-beta), а также их [обновление](/graph/api/audioroutinggroup-update?view=graph-rest-beta) и [удаление](/graph/api/audioroutinggroup-delete?view=graph-rest-beta). |
| Дополнение        | бета        | Добавлен ресурс [online meeting](/graph/api/resources/audioroutinggroup?view=graph-rest-beta) и API для управления собраниями по сети Microsoft Teams. Изначально существует только один API для собраний по сети для [получения объекта online meeting](/graph/api/onlinemeeting-get?view=graph-rest-beta). Также был добавлен соответствующий ресурс для [сведений об аудиоконференции](/graph/api/resources/audioconferencing?view=graph-rest-beta), связанный с собранием (например, URL-адрес телефонного подключения, секретные коды и номера телефонов). |
| Дополнение        | бета        | Выполнение многих из API звонков и собраний занимает длительное время, поэтому были добавлены ресурсы для этих продолжительных операций: [операции, предназначенные для звонков](/graph/api/resources/commsoperation?view=graph-rest-beta), [воспроизведение аудио запросов](/graph/api/resources/playpromptoperation?view=graph-rest-beta) и [ запись](/graph/api/resources/recordoperation?view=graph-rest-beta).  |

### <a name="data-access-microsoft-graph-data-connect"></a>Доступ к данным (подключение к данным Microsoft Graph)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение         | Неприменимо| Представлена возможность массового доступа к данным Office 365. Подробные сведения см. в статье [Microsoft Graph Data Connect (предварительная версия)](data-connect-overview.md).|

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлено действие [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-1.0) для объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0). |
|Дополнение|Бета|Добавлены новые объекты:<br/>[officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta)<br/>[officeClientConfigurationAssignment](/graph/api/resources/intune-cirrus-officeclientconfigurationassignment?view=graph-rest-beta)<br/>[officeConfiguration](/graph/api/resources/intune-cirrus-officeconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientSecurityConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientsecurityconfiguration?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[officeClientCheckinStatus](/graph/api/resources/intune-cirrus-officeclientcheckinstatus?view=graph-rest-beta)<br/>[officeConfigurationAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationassignmenttarget?view=graph-rest-beta)<br/>[officeConfigurationGroupAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationgroupassignmenttarget?view=graph-rest-beta)<br/>[officeUserCheckinSummary](/graph/api/resources/intune-cirrus-officeusercheckinsummary?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлено действие [assign](/graph/api/intune-cirrus-officeclientconfiguration-assign?view=graph-rest-beta) для объекта [officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие **updatePrioritie** для коллекции [officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta) |
|Дополнение|Бета|Добавлены новые объекты:<br/>[deviceConfigurationConflictSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationconflictsummary?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta)<br/>[win32LobApp](/graph/api/resources/intune-apps-win32lobapp?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[deviceConfigurationTargetedUserAndDevice](/graph/api/resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice?view=graph-rest-beta)<br/>[win32LobAppDetection](/graph/api/resources/intune-apps-win32lobappdetection?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetection](/graph/api/resources/intune-apps-win32lobappfilesystemdetection?view=graph-rest-beta)<br/>[win32LobAppInstallExperience](/graph/api/resources/intune-apps-win32lobappinstallexperience?view=graph-rest-beta)<br/>[win32LobAppMsiInformation](/graph/api/resources/intune-apps-win32lobappmsiinformation?view=graph-rest-beta)<br/>[win32LobAppPowerShellScriptDetection](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetection?view=graph-rest-beta)<br/>[win32LobAppProductCodeDetection](/graph/api/resources/intune-apps-win32lobappproductcodedetection?view=graph-rest-beta)<br/>[win32LobAppRegistryDetection](/graph/api/resources/intune-apps-win32lobappregistrydetection?view=graph-rest-beta)<br/>[win32LobAppReturnCode](/graph/api/resources/intune-apps-win32lobappreturncode?view=graph-rest-beta)<br/>[windows10AppsForceUpdateSchedule](/graph/api/resources/intune-deviceconfig-windows10appsforceupdateschedule?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[administratorConfiguredDeviceComplianceState](/graph/api/resources/intune-deviceconfig-administratorconfigureddevicecompliancestate?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[microsoftStoreForBusinessPortalSelectionOptions](/graph/api/resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions?view=graph-rest-beta)<br/>[win32LobAppDetectionOperator](/graph/api/resources/intune-apps-win32lobappdetectionoperator?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetectionType](/graph/api/resources/intune-apps-win32lobappfilesystemdetectiontype?view=graph-rest-beta)<br/>[win32LobAppMsiPackageType](/graph/api/resources/intune-apps-win32lobappmsipackagetype?view=graph-rest-beta)<br/>[win32LobAppRegistryDetectionType](/graph/api/resources/intune-apps-win32lobappregistrydetectiontype?view=graph-rest-beta)<br/>[win32LobAppReturnCodeType](/graph/api/resources/intune-apps-win32lobappreturncodetype?view=graph-rest-beta)<br/>[windows10AppsUpdateRecurrence](/graph/api/resources/intune-deviceconfig-windows10appsupdaterecurrence?view=graph-rest-beta)<br/>[windowsAppStartLayoutTileSize](/graph/api/resources/intune-deviceconfig-windowsappstartlayouttilesize?view=graph-rest-beta)<br/>[windowsAutopilotProfileAssignmentDetailedStatus](/graph/api/resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus?view=graph-rest-beta)<br/>|
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

### <a name="files-sites-and-lists-onedrive-for-business-and-sharepoint"></a>Файлы, сайты и списки (OneDrive для бизнеса и SharePoint)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлен аргумент **deferCommit** для действия [createUploadSession](/graph/api/driveitem-createuploadsession?view=graph-rest-beta) в объекте [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta)|
| Дополнение        | бета        | Добавлен сложный тип [storagePlanInformation](/graph/api/resources/storageplaninformation?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **storagePlanInformation** для сложного типа [quota](/graph/api/resources/quota?view=graph-rest-beta) |
| Дополнение        | Бета-версия        | Добавлено свойство навигации **following** для объекта [drive](/graph/api/resources/drive?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено действие [follow](/graph/api/driveitem-follow?view=graph-rest-beta) для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **hasPassword** для объекта [permission](/graph/api/resources/permission?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **preventsDownload** для сложного типа [sharingLink](/graph/api/resources/sharinglink?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство навигации **permission** для объекта [sharedDriveItem](/graph/api/resources/shareddriveitem?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **geolocation** для объекта [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлен сложный тип [geolocationColumn](/graph/api/resources/geolocationcolumn?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **analytics** для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **analytics** для объекта [site](/graph/api/resources/site?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **analytics** для объекта [listItem](/graph/api/resources/listitem?view=graph-rest-beta) |
| Дополнение        | Бета-версия        | Добавлена функция **getActivitiesByInterval** для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |
| Дополнение        | Бета-версия        | Добавлена функция **getActivitiesByInterval** для объекта [site](/graph/api/resources/site?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлена функция **getActivitiesByInterval** для объекта [listItem](/graph/api/resources/listitem?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлен объект [itemAnalytics](/graph/api/resources/itemanalytics?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлен объект [itemActivityStat](/graph/api/resources/itemactivity?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлен сложный тип [itemActionStat](/graph/api/resources/itemactionstat?view=graph-rest-beta) |
| Дополнение        | Бета-версия        | Добавлен сложный тип [accessAction](/graph/api/resources/accessaction?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлен сложный тип [incompleteData](/graph/api/resources/incompletedata?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **access** для сложного типа [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) |
| Дополнение        | бета        | Добавлено свойство **location** для сложного типа [itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) |
| Дополнение        | 1.0        | Добавлено свойство **preview** для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) |
| Дополнение        | 1.0        | Добавлен сложный тип [itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-1.0) |

### <a name="financials-dynamics-365-business-central"></a>Финансовые показатели (Dynamics 365 Business Central)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | бета          | Добавлены API финансовых показателей для Dynamics 365 Business Central. Дополнительные сведения см. в статье [Справочник по API финансовых показателей](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета | Свойство **InternetMessageHeaders** объекта [message](/graph/api/resources/message?view=graph-rest-1.0) теперь доступно для записи при создании сообщения. |

### <a name="notifications-project-rome"></a>Уведомления (Project Rome)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение          | бета        | Добавлен тип ресурса [notification](/graph/api/resources/projectrome-notification?view=graph-rest-beta). |
| Дополнение          | Бета        | Добавлен API [создания и публикации уведомлений](/graph/api/projectrome_notification_post?view=graph-rest-beta).|

### <a name="security"></a>Безопасность

| **Тип изменения** | **Версия** | **Описание**              |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета       | Добавлены API оценки безопасности для [API безопасности](/graph/api/resources/securescore-api-overview?view=graph-rest-beta), включающие следующие ресурсы и операции:<br/>[secureScores](/graph/api/resources/securescores?view=graph-rest-beta) (и соответствующие объекты)<br/>[Перечисление объектов secureScores](/graph/api/securescores-list?view=graph-rest-beta)<br/>[secureScoreControlProfiles](/graph/api/resources/securescorecontrolprofiles?view=graph-rest-beta)<br/>[Перечисление объектов secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-list?view=graph-rest-beta)<br/>[Обновление secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-update?view=graph-rest-beta) |
| Дополнение        | бета        | Представлен новый сложный тип [secureScoreControlStateUpdate](/graph/api/resources/securescorecontrolstateupdate?view=graph-rest-beta) |

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение|бета|Добавлены API для [вкладок](/graph/api/resources/teamstab?view=graph-rest-beta).|
|Дополнение|бета|Добавлены API для [публикации приложений для организации](/graph/api/resources/teamsapp?view=graph-rest-beta).|
|Дополнение|бета|Добавлена поддержка разрешений приложений для [GET /teams/{id}](/graph/api/team-get?view=graph-rest-beta) |
|Дополнение|бета|Добавлена поддержка разрешений приложений для [GET /teams/{id}/channels](/graph/api/group-list-channels?view=graph-rest-beta) |
|Дополнение|бета|Добавлена поддержка разрешений приложений для [GET /teams/{id}/channels/{id}](/graph/api/channel-get?view=graph-rest-beta) |
|Дополнение|бета|Добавлена поддержка разрешений приложений для [PUT /groups/{id}/team](/graph/api/team-put-teams?view=graph-rest-beta) |
|Дополнение|Бета|Добавлена поддержка разрешений приложений для [PATCH /teams/{id}](/graph/api/team-update?view=graph-rest-beta) |
|Дополнение|бета|Добавлена поддержка разрешений приложений для [создания канала](/graph/api/channel-post?view=graph-rest-beta), [обновления канала](/graph/api/channel-patch?view=graph-rest-beta) и [удаления канала](/graph/api/channel-delete?view=graph-rest-beta). |
|Удаление|бета| Удалены свойства isBlocks и installedState из [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta).|
|Изменение| бета | Свойство context в [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta) переименовано на distributionMethod.|


## <a name="august-2018"></a>Август 2018 г.

### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлено действие [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) и сложные типы [freeBusyError](/graph/api/resources/freebusyerror?view=graph-rest-beta), [scheduleInformation](/graph/api/resources/scheduleinformation?view=graph-rest-beta) и [scheduleItem](/graph/api/resources/scheduleitem?view=graph-rest-beta) для поддержки [получения сведений о доступности пользователей, списков рассылки и ресурсов для указанного периода времени](outlook-get-free-busy-schedule.md). |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

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
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[configurationManagerClientState](/graph/api/resources/intune-devices-configurationmanagerclientstate?view=graph-rest-beta)<br/>[depTokenType](/graph/api/resources/intune-enrollment-deptokentype?view=graph-rest-beta)<br/>[discoverySource](/graph/api/resources/intune-enrollment-discoverysource?view=graph-rest-beta);<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[iTunesPairingMode](/graph/api/resources/intune-enrollment-itunespairingmode?view=graph-rest-beta)<br/>[lanManagerAuthenticationLevel](/graph/api/resources/intune-deviceconfig-lanmanagerauthenticationlevel?view=graph-rest-beta)<br/>[localSecurityOptionsMinimumSessionSecurity](/graph/api/resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity?view=graph-rest-beta)<br/>[resultantAppStateDetail](/graph/api/resources/intune-apps-resultantappstatedetail?view=graph-rest-beta)<br/>[vpnProviderType](/graph/api/resources/intune-deviceconfig-vpnprovidertype?view=graph-rest-beta)<br/>[windowsMalwareThreatState](/graph/api/resources/intune-devices-windowsmalwarethreatstate?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлено действие [uploadDepToken](/graph/api/intune-enrollment-deponboardingsetting-uploaddeptoken?view=graph-rest-beta) для [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [syncWithAppleDeviceEnrollmentProgram](/graph/api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram?view=graph-rest-beta) для [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [setDefaultProfile](/graph/api/intune-enrollment-enrollmentprofile-setdefaultprofile?view=graph-rest-beta) для объекта [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие **importAppleDeviceIdentityList** для коллекции [importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta) |
|Дополнение|бета|Добавлено действие [updateDeviceProfileAssignment](/graph/api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta) для объекта [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено действие [shareForSchoolDataSyncService](/graph/api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice?view=graph-rest-beta) для объекта [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
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
|Дополнение|Бета|Добавлено свойство **roleScopeTagIds** для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta)|
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
|Дополнение|Бета|Добавлено свойство навигации **roleScopeTags** для объекта [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta).|
|Дополнение|бета|Добавлены свойства навигации **advancedThreatProtectionOnboardingStateSummary**, **roleScopeTags** и **importedWindowsAutopilotDeviceIdentityUploads** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **supportedDeviceTypes** для сложного типа [mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta)|
|Дополнение|бета|Добавлено свойство **hideEscapeLink** для сложного типа [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)|
|Дополнение|бета|Добавлены элементы **zscalerPrivateAccess**, **f5Access2018**, **citrixSso** и **paloAltoGlobalProtectV2** для типа перечисления [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **userAbandonment** для типа перечисления [deviceEnrollmentFailureReason](/graph/api/resources/intune-troubleshooting-deviceenrollmentfailurereason?view=graph-rest-beta)|
|Дополнение|Бета|Добавлен элемент **blocked** для типа перечисления [enrollmentState](/graph/api/resources/intune-enrollment-enrollmentstate?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **microsoft365ManagedMdm** для типа перечисления [managementAgentType](/graph/api/resources/intune-devices-managementagenttype?view=graph-rest-beta)|
|Дополнение|бета|Добавлен элемент **domainNameService** для типа перечисления [subjectAlternativeNameType](/graph/api/resources/intune-deviceconfig-subjectalternativenametype?view=graph-rest-beta)|
|Дополнение|Бета|Добавлены элементы **wpa2Personal** и **wpa2Enterprise** для типа перечисления [wiFiSecurityType](/graph/api/resources/intune-deviceconfig-wifisecuritytype?view=graph-rest-beta)|
|Дополнение|бета|Добавлены элементы **enterpriseUnwantedSoftware**, **ransom** и **hipsRule** для типа перечисления [windowsMalwareCategory](/graph/api/resources/intune-devices-windowsmalwarecategory?view=graph-rest-beta)|

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | 1.0 | Добавлено свойство isMultipleDataLocationsForServicesEnabled в ресурс [Organization](/graph/api/resources/organization?view=graph-rest-beta), позволяющее приложениям проверять, включена ли для клиента поддержка нескольких регионов. Добавлено свойство preferredDataLocation в ресурсы [user](/graph/api/resources/user?view=graph-rest-beta) и [group](/graph/api/resources/group?view=graph-rest-beta), позволяющее настраивать предпочтительное расположение данных для пользователя и группы.|
| Дополнение | 1.0 | Добавлено свойство [onPremisesProvisioningErrors](/graph/api/resources/onpremisesprovisioningerror?view=graph-rest-1.0) в объекты [User](/graph/api/resources/user?view=graph-rest-1.0) и [Group](/graph/api/resources/group?view=graph-rest-1.0), представляющее ошибки синхронизации службы каталогов при синхронизации локальных каталогов с Azure Active Directory с использованием продукта синхронизации Майкрософт (включая Azure AD Connect, DirSync и MIM + соединитель).|
| Дополнение | 1.0 | Добавлено свойство [onPremisesExtensionAttributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-1.0) в объект [User](/graph/api/resources/user?view=graph-rest-1.0), содержащее 15 свойств атрибутов настраиваемых расширений. Для пользователя onPremisesSyncEnabled этот набор свойств управляется в локальной службе Active Directory, синхронизирован с Azure AD и доступен только для чтения. Для исключительно облачных пользователей (где значением для onPremisesSyncEnabled является false) эти свойства можно задать при создании или обновлении.|
|Дополнение|1.0|Добавлены свойства **onPremisesDomainName**, **onPremisesSamAccountName** и **onPremisesUserPrincipalName** для объекта [User](/graph/api/resources/user?view=graph-rest-1.0)|

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлена поддержка действия [getMailTips](/graph/api/user-getmailtips?view=graph-rest-1.0) для получения подсказок для определенных получателей. Добавлены следующие ресурсы: [automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-1.0), [mailTips](/graph/api/resources/mailtips?view=graph-rest-1.0), [mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-1.0). |

### <a name="reports"></a>Отчеты
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | 1.0    | Добавлено свойство **Activated On Shared Computer** для объекта [getoffice365activationsuserdetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0) |
| Дополнение    | 1.0    | Добавлено свойство **Shared Computer Activation** для объекта [getoffice365activationsusercounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0). |

### <a name="security"></a>Безопасность

| **Тип изменения** | **Версия** | **Описание**              |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета       | Добавлены свойства **activityGroupName**, **cloudAppStates**, **confidence** и **registryKeyStates** для объекта [alert](/graph/api/resources/alert?view=graph-rest-beta ). |
|Удаление|бета| Удалены свойства **activityGroupStates**, **applicationStates**, **malwareWasRunning**, **riskScore** и **type** из объекта [alert](/graph/api/resources/alert?view=graph-rest-beta ). |
|Изменение|бета| Тип **comments** изменен с `String` на `String collection`, а тип **severity** изменен с `String` на перечисление [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta) в объекте [alert](/graph/api/resources/alert?view=graph-rest-beta). |
| Дополнение        | бета       | Добавлены следующие типы ресурсов: <br/> [cloudAppSecurityState](/graph/api/resources/cloudappsecuritystate?view=graph-rest-beta) <br/> [fileHash](/graph/api/resources/filehash?view=graph-rest-beta) <br/> [registryKeyState](/graph/api/resources/registrykeystate?view=graph-rest-beta) |
|Удаление|бета| Удалены следующие типы ресурсов: <br/> **activityGroupState**  <br/> **applicationSecurityState** |
| Дополнение        | Бета       | Добавлены следующие перечисления: <br/> [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta) <br/> [connectionDirection](/graph/api/resources/connectiondirectionenumtype?view=graph-rest-beta) <br/> [connectionStatus](/graph/api/resources/connectionstatusenumtype?view=graph-rest-beta) <br/> [emailRole](/graph/api/resources/emailroleenumtype?view=graph-rest-beta) <br/> [fileHashType](/graph/api/resources/filehashtypeenumtype?view=graph-rest-beta) <br/> [registryHive](/graph/api/resources/registryhiveenumtype?view=graph-rest-beta)  <br/> [registryOperation](/graph/api/resources/registryoperationenumtype?view=graph-rest-beta) <br/> [registryValueType](/graph/api/resources/registryvaluetypeenumtype?view=graph-rest-beta)|
|Удаление|бета| Удалены следующие типы перечисления: <br/> **alertType** <br/> **applicationPermissionsRequired** |
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
|Удаление|Бета| Удалено свойство **name** из объекта [vulnerabilityState](/graph/api/resources/vulnerabilitystate?view=graph-rest-beta). |

### <a name="track-changes"></a>Отслеживание изменений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлена возможность [запроса изменений](delta-query-overview.md) для следующих объектов в Azure AD:<br/>[application](/graph/api/application-delta?view=graph-rest-beta)<br/>[directoryRole](/graph/api/directoryrole-delta?view=graph-rest-beta)<br/>[servicePrincipal](/graph/api/serviceprincipal-delta?view=graph-rest-beta) |


## <a name="july-2018"></a>Июль 2018 г.

### <a name="change-notifications-webhooks"></a>Уведомления об изменениях (веб-перехватчики)
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Критическое изменение | Бета-версия и версия 1.0 | Сокращен до 3 дней [максимальный период действия подписки](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type) с использованием [веб-перехватчиков](/graph/api/resources/webhooks?view=graph-rest-1.0) для элементов в корне диска. |

### <a name="identity-and-access"></a>Удостоверение и доступ

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | API [application](/graph/api/resources/application?view=graph-rest-beta) и [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) будут обновлены в предварительной (бета) версии. Первый набор изменений будет применен 16 мая 2018 г. Изменения включают в себя переименование и реструктуризацию свойств. Большинство существующих свойств будут доступны только после применения изменений. Будут добавлены новые свойства. Прежде чем выйдет версия 1.0 с изменениями, будет выпущена бета-версия. |

### <a name="identity-and-access--synchronization"></a>Удостоверение и доступ | Синхронизация

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлено свойство **progress** для объекта [sychronizationStatus](/graph/api/resources/synchronization-synchronizationstatus?view=graph-rest-beta), чтобы разрешить клиентам наблюдать за ходом выполнения задания синхронизации.|

### <a name="personal-contacts-outlook"></a>Личные контакты (Outlook)
| **Тип изменения** | **Версия**   | **Описание**                          |
|:--------------- |:------------- |:---------------------------------------- |
|Дополнение |Бета-версия | Добавлен сложный тип [typedEmailAddress](/graph/api/resources/typedemailaddress?view=graph-rest-beta). |
|Изменение | Бета-версия | Изменен тип свойства **emailAddresses** для ресурса [contact](/graph/api/resources/contact?view=graph-rest-beta). Теперь это коллекция экземпляров **typedEmailAddress**.|

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Изменение|бета|Обновлен ресурс [chatmessage](/graph/api/resources/chatmessage?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлен тип ресурса [вложения для чата](/graph/api/resources/chatmessageattachment?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлен тип ресурса [упоминания для чата](/graph/api/resources/chatmessageattachment?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлен тип ресурса [реакции для чата](/graph/api/resources/chatmessageattachment?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлен [API получения всех сообщений в канале](/graph/api/channel-list-messages?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения API сообщений в канале](/graph/api/channel-get-message?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения всех API ответов на сообщения](/graph/api/channel-list-messagereplies?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения ответа для API сообщений](/graph/api/channel-get-messagereply?view=graph-rest-beta) |
|Дополнение|бета|Добавлена поддержка разрешений приложений для [/users/{id}/joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлен [API получения всех сообщений в канале](/graph/api/channel-list-messages?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения API сообщений в канале](/graph/api/channel-get-message?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения всех API ответов на сообщения](/graph/api/channel-list-messagereplies?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлена возможность [получения ответа для API сообщений](/graph/api/channel-get-messagereply?view=graph-rest-beta) |
|Дополнение|Бета-версия|Добавлен тип ресурса [вложения для чата](/graph/api/resources/chatmessageattachment?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлен тип ресурса [упоминания для чата](/graph/api/resources/chatmessageattachment?view=graph-rest-beta)|
|Дополнение|Бета-версия|Добавлен тип ресурса [реакции для чата](/graph/api/resources/chatmessageattachment?view=graph-rest-beta)|
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
|Удаление|бета|Удален GET /groups/{id}/channels, используйте GET /teams/{id}/channels. |
|Удаление|Бета-версия|Удален POST /groups/{id}/team/channels, используйте POST /teams/{id}/channels. |
|Удаление|бета|Удален GET /groups/{id}/team, используйте GET /teams/{id}. |
|Удаление|Бета-версия|Удален PATCH /groups/{id}/team, используйте PATCH /teams/{id}. |
|Дополнение|Бета-версия|Добавлен API для [перечисления всех групп в организации](teams-list-all-teams.md). |


## <a name="june-2018"></a>Июнь 2018 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Для сущности [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0) добавлено свойство **connectorServerName**.|
|Дополнение|1.0|Для сущности [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0) добавлены свойства **firewallEnabled**, **firewallBlockAllIncoming** и **firewallEnableStealthMode**|
|Дополнение|1.0|Для типа перечисления [iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-1.0) добавлен элемент **unknown**.|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidDeviceOwnerWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownerwificonfiguration?view=graph-rest-beta)<br/>[iosVppAppAssignedDeviceLicense](/graph/api/resources/intune-apps-iosvppappassigneddevicelicense?view=graph-rest-beta)<br/>[iosVppAppAssignedLicense](/graph/api/resources/intune-apps-iosvppappassignedlicense?view=graph-rest-beta)<br/>[iosVppAppAssignedUserLicense](/graph/api/resources/intune-apps-iosvppappassigneduserlicense?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationState](/graph/api/resources/intune-deviceconfig-manageddevicemobileappconfigurationstate?view=graph-rest-beta)<br/>[userPFXCertificate](/graph/api/resources/intune-raimportcerts-userpfxcertificate?view=graph-rest-beta)<br/>[vppTokenLicenseSummary](/graph/api/resources/intune-onboarding-vpptokenlicensesummary?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[iosVppAppRevokeLicensesActionResult](/graph/api/resources/intune-apps-iosvppapprevokelicensesactionresult?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[androidDeviceOwnerSystemUpdateInstallType](/graph/api/resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype?view=graph-rest-beta)<br/>[androidDeviceOwnerWiFiSecurityType](/graph/api/resources/intune-deviceconfig-androiddeviceownerwifisecuritytype?view=graph-rest-beta)<br/>[userPfxIntendedPurpose](/graph/api/resources/intune-raimportcerts-userpfxintendedpurpose?view=graph-rest-beta)<br/>[userPfxPaddingScheme](/graph/api/resources/intune-raimportcerts-userpfxpaddingscheme?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Для ресурса [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) добавлено действие [completeSignup](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken?view=graph-rest-beta). |
|Дополнение|Бета|Для ресурса [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) добавлено действие [revokeAllLicenses](/graph/api/intune-apps-iosvppapp-revokealllicenses?view=graph-rest-beta) |
|Дополнение|Бета|Для ресурса [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) добавлено действие [revokeUserLicense](/graph/api/intune-apps-iosvppapp-revokeuserlicense?view=graph-rest-beta) |
|Дополнение|Бета|Для ресурса [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) добавлено действие [revokeDeviceLicense](/graph/api/intune-apps-iosvppapp-revokedevicelicense?view=graph-rest-beta) |
|Дополнение|Бета|Для ресурса [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) добавлено действие [sendCustomNotificationToCompanyPortal](/graph/api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal?view=graph-rest-beta) |
|Дополнение|Бета|Для семейства [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) добавлена функция **getLicensesForApp** |
|Удаление|бета|Удалены следующие типы перечисления:<br/>**windowsUpdateInsiderBuildControl**<br/>|
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

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | бета | Добавлена функция [получения доступа к проверкам](/graph/api/resources/accessreviews-root?view=graph-rest-beta) в [Azure AD](/graph/api/resources/azure-ad-overview?view=graph-rest-beta). |

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Все | Новые разрешения приложений _Application.ReadWrite.All_ и _Application.ReadWrite.OwnedBy_, позволяющие клиентскому приложению создавать, читать, обновлять и удалять приложения и субъекты-службы, как описано в [статье о разрешениях](permissions-reference.md#application-resource-permissions). |
| Дополнение | 1.0 | Добавлены свойства **ageGroup**, **legalAgeGroupClassification** и **ConsentRequiredForMinor** для ресурса [user](/graph/api/resources/user?view=graph-rest-1.0)

### <a name="identity-and-access--privileged-identity-management"></a>Удостоверение и доступ | Управление привилегированными пользователями (PIM)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение | Бета | Добавлена сущность [privilegedAccess](/graph/api/resources/privilegedaccess?view=graph-rest-beta).|
| Дополнение | Бета | Добавлен объект [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta), а также следующие методы и действия: <br> [Список](/graph/api/governanceresource-list?view=graph-rest-beta) <br> [Получение](/graph/api/governanceresource-get?view=graph-rest-beta)<br>|
| Дополнение | Бета | Добавлена сущность [governanceSubject](/graph/api/resources/governancesubject?view=graph-rest-beta).|
| Дополнение | Бета | Добавлена сущность [governanceRoleDefinition](/graph/api/resources/governanceroledefinition?view=graph-rest-beta), а также следующие методы и действия:<br> [Список](/graph/api/governanceroledefinition-list?view=graph-rest-beta) <br> [Получение](/graph/api/governanceroledefinition-get?view=graph-rest-beta) |
| Дополнение | Бета | Добавлена сущность [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta), а также следующие методы и действия:<br> [Список](/graph/api/governanceroleassignment-list?view=graph-rest-beta) <br> [Получение](/graph/api/governanceroleassignment-get?view=graph-rest-beta) <br> [Экспорт](/graph/api/governanceroleassignment-export?view=graph-rest-beta) |
| Дополнение | Бета | Добавлена сущность [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta), а также следующие методы и действия:<br> [Перечисление](/graph/api/governanceroleassignmentrequest-list?view=graph-rest-beta) <br> [Получение](/graph/api/governanceroleassignmentrequest-get?view=graph-rest-beta) <br> [Создание](/graph/api/governanceroleassignmentrequest-post?view=graph-rest-beta) <br> [Отмена](/graph/api/governanceroleassignmentrequest-cancel?view=graph-rest-beta) <br> [Обновление](/graph/api/governanceroleassignmentrequest-update?view=graph-rest-beta) |
| Дополнение | Бета | Добавлена сущность [governanceRoleSetting](/graph/api/resources/governancerolesetting?view=graph-rest-beta), а также следующие методы и действия:<br> [Список](/graph/api/governancerolesetting-list?view=graph-rest-beta) <br> [Получение](/graph/api/governancerolesetting-get?view=graph-rest-beta) <br> [Обновление](/graph/api/governancerolesetting-update?view=graph-rest-beta) |
| Дополнение | Бета | Добавлены следующие сложные типы: <br> [governancePermission](/graph/api/resources/governancepermission?view=graph-rest-beta) <br> [governanceRoleAssignmentRequestStatus](/graph/api/resources/governanceroleassignmentrequeststatus?view=graph-rest-beta) <br> [governanceRuleSetting](/graph/api/resources/governancerulesetting?view=graph-rest-beta) <br> [governanceSchedule](/graph/api/resources/governanceschedule?view=graph-rest-beta)|

### <a name="security"></a>Безопасность

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | бета        | Добавлены новые типы перечисления:<br/>[alertFeedback](/graph/api/resources/alertfeedbackenumtype?view=graph-rest-beta)<br/>[alertStatus](/graph/api/resources/alertstatusenumtype?view=graph-rest-beta)<br/>[alertType](/graph/api/resources/alerttypeenumtype?view=graph-rest-beta)<br/>[applicationPermissionsRequired](/graph/api/resources/applicationpermissionsrequiredenumtype?view=graph-rest-beta)<br/>[logonType](/graph/api/resources/logontypeenumtype?view=graph-rest-beta)<br/>[processIntegrityLevel](/graph/api/resources/processintegritylevelenumtype?view=graph-rest-beta)<br/>[securityNetworkProtocol](/graph/api/resources/securitynetworkprotocolenumtype?view=graph-rest-beta)<br/>[userAccountSecurityType](/graph/api/resources/useraccountsecuritytypeenumtype?view=graph-rest-beta)<br/>


### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)
| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Дополнение         | Бета          | Добавлены API [архивирования](/graph/api/team-archive?view=graph-rest-beta) и [разархивирования](/graph/api/team-unarchive?view=graph-rest-beta) команды.|
|Дополнение         | Бета          | Добавлена операция [клонирования](/graph/api/team-clone?view=graph-rest-beta) команды. |
|Дополнение         | Бета          | Добавлены интерфейсы API для добавления [приложений](/graph/api/resources/teamsapp?view=graph-rest-beta) в группы и удаления из них. |
|Изменение|Бета|Обновлен путь к сущности [команды](/graph/api/resources/team?view=graph-rest-beta).|
|Изменение|бета|Обновлен путь к объекту [channel](/graph/api/resources/channel?view=graph-rest-beta).|


## <a name="may-2018"></a>Май 2018 г.

### <a name="customer-booking-microsoft-bookings"></a>Резервирование для пользователей (Microsoft Bookings)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | бета          | Добавлены объект [bookingBusiness](/graph/api/resources/bookingbusiness?view=graph-rest-beta) и следующие методы и действия CRUD: <br> [перечисление](/graph/api/bookingbusiness-list?view=graph-rest-beta); <br> [создание](/graph/api/bookingbusiness-post-bookingbusinesses?view=graph-rest-beta); <br> [получение](/graph/api/bookingbusiness-get?view=graph-rest-beta); <br> [Обновление](/graph/api/bookingbusiness-update?view=graph-rest-beta) <br> [удаление](/graph/api/bookingbusiness-delete?view=graph-rest-beta); <br> [публикация](/graph/api/bookingbusiness-publish?view=graph-rest-beta); <br> [отмена публикации](/graph/api/bookingbusiness-unpublish?view=graph-rest-beta). <br> Узнайте больше об интеграции с [API Microsoft Bookings](booking-concept-overview.md). |
| Дополнение        | бета          | Добавлены объект [bookingAppointment](/graph/api/resources/bookingappointment?view=graph-rest-beta) и следующие методы и действие CRUD: <br> [перечисление](/graph/api/bookingbusiness-list-appointments?view=graph-rest-beta); <br> [создание](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta); <br> [получение](/graph/api/bookingappointment-get?view=graph-rest-beta); <br> [Обновление](/graph/api/bookingappointment-update?view=graph-rest-beta) <br> [удаление](/graph/api/bookingappointment-delete?view=graph-rest-beta); <br> [отмена](/graph/api/bookingappointment-cancel?view=graph-rest-beta). |
| Дополнение        | Бета          | Добавлены объект [bookingCurrency](/graph/api/resources/bookingcurrency?view=graph-rest-beta) и следующие методы: <br> [перечисление](/graph/api/bookingcurrency-list?view=graph-rest-beta); <br> [получение](/graph/api/bookingcurrency-get?view=graph-rest-beta). |
| Дополнение        | Бета          | Добавлены объект [bookingCustomer](/graph/api/resources/bookingcustomer?view=graph-rest-beta) и следующие методы CRUD: <br> [List](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta) <br> [создание](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta); <br> [получение](/graph/api/bookingcustomer-get?view=graph-rest-beta); <br> [обновление](/graph/api/bookingcustomer-update?view=graph-rest-beta); <br> [удаление](/graph/api/bookingcustomer-delete?view=graph-rest-beta).|
| Дополнение        | Бета          | Добавлены объект [bookingService](/graph/api/resources/bookingservice?view=graph-rest-beta) и следующие методы CRUD: <br> [перечисление](/graph/api/bookingbusiness-list-services?view=graph-rest-beta); <br> [создание](/graph/api/bookingbusiness-post-services?view=graph-rest-beta); <br> [получение](/graph/api/bookingservice-get?view=graph-rest-beta); <br> [обновление](/graph/api/bookingservice-update?view=graph-rest-beta); <br> [удаление](/graph/api/bookingservice-delete?view=graph-rest-beta).|
| Дополнение        | Бета          | Добавлены объект [bookingStaffMember](/graph/api/resources/bookingstaffmember?view=graph-rest-beta) и следующие методы CRUD: <br> [перечисление](/graph/api/bookingbusiness-list-staffmembers?view=graph-rest-beta); <br> [создание](/graph/api/bookingbusiness-post-staffmembers?view=graph-rest-beta); <br> [получение](/graph/api/bookingstaffmember-get?view=graph-rest-beta); <br> [обновление](/graph/api/bookingstaffmember-update?view=graph-rest-beta); <br> [удаление](/graph/api/bookingstaffmember-delete?view=graph-rest-beta).|
| Дополнение        | Бета          | Добавлены следующие сложные типы: <br> [bookingNamedEntity](/graph/api/resources/bookingnamedentity?view=graph-rest-beta); <br> [bookingPerson](/graph/api/resources/bookingperson?view=graph-rest-beta); <br> [bookingReminder](/graph/api/resources/bookingreminder?view=graph-rest-beta); <br> [bookingWorkHours](/graph/api/resources/bookingworkhours?view=graph-rest-beta); <br> [bookingWorkTimeSlot](/graph/api/resources/bookingworktimeslot?view=graph-rest-beta).|

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta);<br/>[easEmailProfileConfigurationBase](/graph/api/resources/intune-deviceconfig-easemailprofileconfigurationbase?view=graph-rest-beta);<br/>[mobileAppIntentAndState](/graph/api/resources/intune-troubleshooting-mobileappintentandstate?view=graph-rest-beta);<br/>[mobileAppTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingevent?view=graph-rest-beta);<br/>[unsupportedDeviceConfiguration](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfiguration?view=graph-rest-beta);<br/>[windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta).<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[managedDeviceCleanupSettings](/graph/api/resources/intune-devices-manageddevicecleanupsettings?view=graph-rest-beta);<br/>[mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta);<br/>[mobileAppTroubleshootingAppPolicyCreationHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapppolicycreationhistory?view=graph-rest-beta);<br/>[mobileAppTroubleshootingAppStateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappstatehistory?view=graph-rest-beta);<br/>[mobileAppTroubleshootingAppTargetHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapptargethistory?view=graph-rest-beta);<br/>[mobileAppTroubleshootingAppUpdateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappupdatehistory?view=graph-rest-beta);<br/>[mobileAppTroubleshootingDeviceCheckinHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingdevicecheckinhistory?view=graph-rest-beta);<br/>[mobileAppTroubleshootingHistoryItem](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem?view=graph-rest-beta);<br/>[unsupportedDeviceConfigurationDetail](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail?view=graph-rest-beta);<br/>**windowsAutoPilotEnrollmentSettings**;<br/>[windowsKioskActiveDirectoryGroup](/graph/api/resources/intune-deviceconfig-windowskioskactivedirectorygroup?view=graph-rest-beta);<br/>[windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta);<br/>[windowsKioskAppConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskappconfiguration?view=graph-rest-beta);<br/>[windowsKioskAutologon](/graph/api/resources/intune-deviceconfig-windowskioskautologon?view=graph-rest-beta);<br/>[windowsKioskAzureADGroup](/graph/api/resources/intune-deviceconfig-windowskioskazureadgroup?view=graph-rest-beta);<br/>[windowsKioskAzureADUser](/graph/api/resources/intune-deviceconfig-windowskioskazureaduser?view=graph-rest-beta);<br/>[windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta);<br/>[windowsKioskLocalGroup](/graph/api/resources/intune-deviceconfig-windowskiosklocalgroup?view=graph-rest-beta);<br/>[windowsKioskLocalUser](/graph/api/resources/intune-deviceconfig-windowskiosklocaluser?view=graph-rest-beta);<br/>[windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta);<br/>[windowsKioskProfile](/graph/api/resources/intune-deviceconfig-windowskioskprofile?view=graph-rest-beta);<br/>[windowsKioskSingleUWPApp](/graph/api/resources/intune-deviceconfig-windowskiosksingleuwpapp?view=graph-rest-beta);<br/>[windowsKioskUser](/graph/api/resources/intune-deviceconfig-windowskioskuser?view=graph-rest-beta);<br/>[windowsKioskUWPApp](/graph/api/resources/intune-deviceconfig-windowskioskuwpapp?view=graph-rest-beta);<br/>[windowsKioskVisitor](/graph/api/resources/intune-deviceconfig-windowskioskvisitor?view=graph-rest-beta).<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[defenderScheduleScanDay](/graph/api/resources/intune-deviceconfig-defenderschedulescanday?view=graph-rest-beta);<br/>[defenderSubmitSamplesConsentType](/graph/api/resources/intune-deviceconfig-defendersubmitsamplesconsenttype?view=graph-rest-beta);<br/>[domainNameSource](/graph/api/resources/intune-deviceconfig-domainnamesource?view=graph-rest-beta);<br/>[localSecurityOptionsSmartCardRemovalBehaviorType](/graph/api/resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype?view=graph-rest-beta);<br/>[mobileAppActionType](/graph/api/resources/intune-troubleshooting-mobileappactiontype?view=graph-rest-beta);<br/>[mobileAppIntent](/graph/api/resources/intune-troubleshooting-mobileappintent?view=graph-rest-beta);<br/>[roleAssignmentScopeType](/graph/api/resources/intune-rbac-roleassignmentscopetype?view=graph-rest-beta);<br/>[usernameSource](/graph/api/resources/intune-deviceconfig-usernamesource?view=graph-rest-beta);<br/>[windowsDeviceUsageType](/graph/api/resources/intune-enrollment-windowsdeviceusagetype?view=graph-rest-beta).<br/>|
|Дополнение|Бета-версия|Добавлено действие [setDeviceName](/graph/api/intune-devices-manageddevice-setdevicename?view=graph-rest-beta)<br/>для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Удаление|Бета|Удалены следующие объекты:<br/>**depEnrollmentProfile**;<br/>**enrollmentProfile**;<br/>**importedAppleDeviceIdentity**<br/>**importedAppleDeviceIdentityResult**.<br/>|
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**managementCertificateWithThumbprint**.<br/>|
|Удаление|бета|Удалены следующие типы перечисления:<br/>**depTokenType**;<br/>**discoverySource**;<br/>**iTunesPairingMode**.<br/>|
|Удаление|Бета-версия|Удалено действие importAppleDeviceIdentityList для коллекции [importedAppleDeviceIdentity](/graph/api/resources/intune-corpenrollment-importedappledeviceidentity?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалено действие [updateDeviceProfileAssignment](/graph/api/intune-corpenrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta) для объекта [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалено действие setDefaultProfile для объекта [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалено действие shareForSchoolDataSyncService для объекта [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалено действие unshareForSchoolDataSyncService для объекта [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
|Удаление|бета|Удалена функция exportMobileConfig](/graph/api/intune_corpenrollment_enrollmentprofile_exportmobileconfig?view=graph-rest-beta) для объекта [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) |
|Дополнение|Бета|Добавлены свойства **userDomainNameSource** и **customDomainName** объекта [androidEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-androideasemailprofileconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **workProfileBlockCamera** и **workProfileBlockCrossProfileContactsSearch** объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **workProfileBlockCamera** и **workProfileBlockCrossProfileContactsSearch** объекта [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **thirdPartyKeyboardsBlocked** и **filterOpenInToOnlyManagedApps** объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **conflictCount** объекта [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **conflictCount** объекта [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **managedDeviceCleanupSettings** объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалено свойство **usernameSource** объекта [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **thirdPartyKeyboardsBlocked** и **filterOpenInToOnlyManagedApps** объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **ignoreVersionDetection** объекта [macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **pinRequiredOnLaunchInsteadOfBiometric** и **pinRequiredInsteadOfBiometricTimeout** объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **autopilotEnrolled**, **requireUserEnrollmentApproval**, **iccid** и **udid** объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Удаление|бета|Удалено свойство **isAutopilotEnrolled** объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Дополнение|бета|Добавлены свойства **notApplicablePlatformCount** и **conflictCount** объекта [managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **conflictCount** для объекта [managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **scopeType** объекта [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалено свойство **usernameSource** объекта [windows10EasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windows10easemailprofileconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees**, **localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers**, **localSecurityOptionsDisableServerDigitallySignCommunicationsAlways**, **localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees**, **localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares**, **localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts**, **localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares**, **localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange** и **localSecurityOptionsSmartCardRemovalBehavior** объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **showInstallationProgress**, **blockDeviceSetupRetryByUser**, **allowDeviceResetOnInstallFailure**, **allowLogCollectionOnInstallFailure**, **customErrorMessage**, **installProgressTimeoutInMinutes** и **allowDeviceUseOnInstallFailure** объекта [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалены свойства **title**, **bodyText**, **moreInfoUrl** и **moreInfoText** объекта [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta).|
|Дополнение|бета|Добавлены свойства **defenderBlockOnAccessProtection**, **defenderScheduleScanDay** и **defenderSubmitSamplesConsentType** объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства **language** и **enrollmentSettings** объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta).|
|Дополнение|бета|Добавлено свойство **useDeviceContext** объекта [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалено свойство **usernameSource** объекта [windowsPhoneEASEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалено свойство навигации **localActions** объекта [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta).|
|Удаление|Бета-версия|Удалены свойства навигации **enrollmentProfiles** и **importedAppleDeviceIdentities** объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства навигации **mobileAppIntentAndStates** и **mobileAppTroubleshootingEvents** объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta).|
|Дополнение|бета|Добавлены свойства **deviceUsageType** и **skipKeyboardSelectionPage** к сложному типу [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta).|
|Удаление|Бета-версия|Удален элемент **paloAltoGlobalProtect** из типа перечисления [androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены элементы **samAccountName** и **primarySmtpAddress** к типу перечисления [androidUsernameSource](/graph/api/resources/intune-deviceconfig-androidusernamesource?view=graph-rest-beta).|
|Удаление|Бета-версия|Удален элемент **paloAltoGlobalProtect** из типа перечисления [androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлен элемент **paloAltoGlobalProtect** к типу перечисления [windows10VpnConnectionType](/graph/api/resources/intune-deviceconfig-windows10vpnconnectiontype?view=graph-rest-beta).|

### <a name="education"></a>Образование

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Разрешение **Members.Read.Hidden** необходимо для чтения или обновления коллекции **Members** в объекте [educationClass](/graph/api/resources/educationclass?view=graph-rest-1.0) с помощью маркеров только для приложения. |
|Изменение           |Бета-версия           |Обновлены возможные значения типа **educationSubmissionStatus** в свойстве status объекта [educationsubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|
|Изменение           |Бета-версия           |Добавлен сложный тип **educationAssignmentIndividualRecipient** к свойству assignTo объекта [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta).|
|Изменение           |Бета-версия           |Добавлены свойства **unsubmittedBy**, **unsubmittedDate**, **returnedBy**, **returnedDate** объекта [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|
|Дополнение         |Бета-версия           |Добавлены действия [return](/graph/api/educationsubmission-return?view=graph-rest-beta) и [unsubmit](/graph/api/educationsubmission-unsubmit?view=graph-rest-beta) для объекта [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|
|Изменение           |Бета-версия           |Удалены действия release и recall для объекта [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|

### <a name="groups"></a>Группы

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета | Добавлено свойство **importance** в объект [post](/graph/api/resources/post?view=graph-rest-1.0). |

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение           | Бета          | Свойство **creatorUserId** сущности [subscription](/graph/api/resources/subscription?view=graph-rest-beta) переименовано в **creatorId** для лучшего отражения смысла. |

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлено действие [перечисления удаленных элементов, принадлежащих пользователю,](/graph/api/directory-deleteditems-user-owned?view=graph-rest-1.0) для ресурса [каталог (удаленные элементы)](/graph/api/resources/directory?view=graph-rest-1.0). |
| Дополнение | Бета | В ресурс [directory](/graph/api/resources/directory?view=graph-rest-beta) добавлена функция [getUserOwnedObjects](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta) для перечисления удаленных групп, принадлежащих определенному пользователю. |

### <a name="social-and-workplace-intelligence--insights"></a>Социальная и рабочая аналитика | Аналитические сведения

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | Бета          | Добавлены объект [settings](/graph/api/resources/user-settings?view=graph-rest-beta) и следующие методы CRUD: <br> [получение](/graph/api/user-get-settings?view=graph-rest-beta); <br> [обновление](/graph/api/user-update-settings?view=graph-rest-beta). |


## <a name="april-2018"></a>Апрель 2018 г.

### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Добавлено свойство **locations** для объекта [event](/graph/api/resources/event?view=graph-rest-1.0), позволяющее организовать событие, в котором могут участвовать пользователи из нескольких мест. |
| Дополнение        | 1.0          | Добавлено свойство **locationType** для сложного типа [location](/graph/api/resources/location?view=graph-rest-1.0). |
| Дополнение        | 1.0          | Добавлены свойства **uniqueId** и **uniqueIdType** для сложного типа [location](/graph/api/resources/location?view=graph-rest-1.0). В настоящее время эти свойства предназначены только для внутреннего использования. |

### <a name="cross-device-experiences-project-rome"></a>Решения для нескольких устройств (Project Rome)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение | 1.0 | Добавлен [API для получения последних действий](/graph/api/projectrome-get-recent-activities?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлен [API для получения действий](/graph/api/projectrome-get-activities?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлена операция [создания или замены действия](/graph/api/projectrome-put-activity?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлена операция [создания или замены элемента журнала](/graph/api/projectrome-put-historyitem?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлена операция [удаления действия](/graph/api/projectrome-delete-activity?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлена операция [создания или замены элемента журнала](/graph/api/projectrome-delete-historyitem?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлен тип ресурса [activity](/graph/api/resources/projectrome-activity?view=graph-rest-1.0). |
| Дополнение | Версия 10 | Добавлен тип ресурса [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлен тип ресурса [visualInfo](/graph/api/resources/projectrome-visualinfo?view=graph-rest-1.0). |
| Дополнение | 1.0 | Добавлен тип ресурса [imageInfo](/graph/api/resources/projectrome-imageinfo?view=graph-rest-1.0). |
| Дополнение | Версия 10 | Добавлен [обзор Project Rome](/graph/api/resources/project-rome-overview?view=graph-rest-1.0). |
| Изменение | Бета | Добавлена документация по глубокой вставке для [создания или замены действия](/graph/api/projectrome-put-activity?view=graph-rest-beta). |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлены новые объекты:<br/>[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-1.0).<br/>|
|Дополнение|1.0|Добавлены новые типы перечисления:<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-1.0).<br/>|
|Дополнение|1.0|Добавлено свойство **managedDeviceOwnerType** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0).|
|Дополнение|1.0|Добавлено свойство навигации **deviceStatuses** для объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0).|
|Дополнение|1.0|Добавлен элемент **androidWorkProfile** для типа перечисления [policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-1.0).|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilecustomconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofileeasemailprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate?view=graph-rest-beta)<br/>[androidWorkProfileVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilewificonfiguration?view=graph-rest-beta)<br/>[restrictedAppsViolation](/graph/api/resources/intune-deviceconfig-restrictedappsviolation?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfileAssignment](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofileassignment?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[managedDeviceModelsAndManufacturers](/graph/api/resources/intune-devices-manageddevicemodelsandmanufacturers?view=graph-rest-beta)<br/>[managedDeviceReportedApp](/graph/api/resources/intune-devices-manageddevicereportedapp?view=graph-rest-beta)<br/>[windowsEnrollmentStatusScreenSettings](/graph/api/resources/intune-enrollment-windowsenrollmentstatusscreensettings?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые типы перечисления:<br/>[androidWorkProfileCrossProfileDataSharingType](/graph/api/resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype?view=graph-rest-beta)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](/graph/api/resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype?view=graph-rest-beta)<br/>[androidWorkProfileRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype?view=graph-rest-beta)<br/>[androidWorkProfileVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconnectiontype?view=graph-rest-beta)<br/>[bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta)<br/>[localSecurityOptionsInformationShownOnLockScreenType](/graph/api/resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype?view=graph-rest-beta)<br/>[managedAppRemediationAction](/graph/api/resources/intune-mam-managedappremediationaction?view=graph-rest-beta)<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-beta)<br/>[restrictedAppsState](/graph/api/resources/intune-deviceconfig-restrictedappsstate?view=graph-rest-beta)<br/>[windows10VpnProfileTarget](/graph/api/resources/intune-deviceconfig-windows10vpnprofiletarget?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлено действие [playLostModeSound](/graph/api/intune-devices-manageddevice-playlostmodesound?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Удаление|бета|Удалены следующие типы перечисления:<br/>**bitLockerRecoveryinformationType**<br/>**windowsUpdateRestartMode**<br/>|
|Дополнение|Бета|Добавлены свойства **workProfileBlockScreenCapture** и **workProfileBlockCrossProfileCallerId** для объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **minimumWipePatchVersion**, **allowedAndroidDeviceManufacturers** и **appActionIfAndroidDeviceManufacturerNotAllowed** для объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **minimumWipeSdkVersion**, **minimumWipePatchVersion**, **allowedIosDeviceModels**, **appActionIfIosDeviceModelNotAllowed**, **allowedAndroidDeviceManufacturers** и **appActionIfAndroidDeviceManufacturerNotAllowed** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **notApplicablePlatformCount** и **conflictCount** для объекта [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **notApplicablePlatformCount** и **conflictCount** для объекта [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **accountMoveCompletionDateTime** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **minimumWipeSdkVersion**, **allowedIosDeviceModels** и **appActionIfIosDeviceModelNotAllowed** для объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **minimumWipeOsVersion**, **minimumWipeAppVersion**, **appActionIfDeviceComplianceRequired** и **appActionIfMaximumPinRetriesExceeded** для объекта [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **managedDeviceOwnerType**, **preferMdmOverGroupPolicyAppliedDateTime**, **isAutopilotEnrolled** и **requestUserEnrollmentApproval** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **managedDeviceModelsAndManufacturers** для объекта [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **localSecurityOptionsMachineInactivityLimitInMinutes**, **localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool**, **localSecurityOptionsInformationShownOnLockScreen**, **defenderSecurityCenterDisableAccountUI**, **defenderSecurityCenterDisableHardwareUI**, **defenderSecurityCenterDisableRansomwareUI**, **defenderSecurityCenterDisableSecureBootUI** и **defenderSecurityCenterDisableTroubleshootingUI** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **printerNames**, **printerDefaultName**, **printerBlockAddition** и **searchBlockWebResults** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены свойства **profileTarget**, **enableAlwaysOn** и **enableDeviceTunnel** для объекта [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **enrollmentStatusScreenSettings** для объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство навигации **deviceConfigurationRestrictedAppsViolations** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство навигации **assignments** для объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство навигации **networkAccessConfigurations** для объекта [windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta).|
|Удаление|бета|Удалено свойство **permissions** из сложного типа [auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta).|
|Изменение|Бета|Изменен тип следующих свойств сложного типа [bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta):<br/>**recoveryInformationToStore** с [bitLockerRecoveryinformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta) на [bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta).<br/>|
|Дополнение|Бета|Добавлено свойство **deviceInactivityBeforeRetirementInDay** для сложного типа [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta).|
|Дополнение|Бета|Добавлено свойство **landingPageCustomizedImage** для сложного типа [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta).|
|Удаление|Бета|Удалено свойство **ipAddressOrFqdn** из сложного типа [vpnServer](/graph/api/resources/intune-deviceconfig-vpnserver?view=graph-rest-beta).|
|Удаление|Бета|Удалено свойство **restartMode** из сложного типа [windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta).|
|Дополнение|Бета|Добавлен элемент **paloAltoGlobalProtect** для типа перечисления [androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta).|
|Дополнение|бета|Добавлен элемент **paloAltoGlobalProtect** для типа перечисления [androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta).|
|Дополнение|Бета|Добавлен элемент **paloAltoGlobalProtect** для типа перечисления [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta).|
|Дополнение|Бета|Добавлен элемент **androidWorkProfile** для типа перечисления [policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-beta).|

### <a name="education"></a>Образование

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Изменение|Бета-версия|Добавлено свойство reportableIdentifier объекта [educationsynchronizationerror](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta).|
|Изменение|бета|Обновлены варианты ответа для API [uploadUrl](/graph/api/educationsynchronizationprofile-uploadurl?view=graph-rest-beta).|
|Изменение|Бета-версия|Обновлен текст описания типа ресурса [educationSynchronizationError](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta).|
|Изменение|Бета-версия|Обновлен текст описания для API [получения ошибок синхронизации](/graph/api/educationsynchronizationerrors-get?view=graph-rest-beta).|

### <a name="identity-and-access--audit-logs"></a>Удостоверение и доступ | Журналы аудита

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены объекты [directoryAudit](/graph/api/resources/directoryaudit?view=graph-rest-beta) и [signIn](/graph/api/resources/signin?view=graph-rest-beta) для поддержки нового API журнала аудита. |
|Дополнение|Бета|Добавлены следующие ресурсы для поддержки API журнала аудита: [appIndentity](/graph/api/resources/appidentity?view=graph-rest-beta), [auditActivityInitiator](/graph/api/resources/auditactivityinitiator?view=graph-rest-beta), [conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta), [deviceDetail](/graph/api/resources/devicedetail?view=graph-rest-beta), [mfaDetail](/graph/api/resources/mfadetail?view=graph-rest-beta), [modifiedProperty](/graph/api/resources/modifiedproperty?view=graph-rest-beta), [signinLocation](/graph/api/resources/signinlocation?view=graph-rest-beta), [signinStatus](/graph/api/resources/signinstatus?view=graph-rest-beta), [targetResource](/graph/api/resources/targetresource?view=graph-rest-beta), [targetResourceApp](/graph/api/resources/targetresourceapp?view=graph-rest-beta), [targetResourceDevice](/graph/api/resources/targetresourcedevice?view=graph-rest-beta), [targetResourceDirectory](/graph/api/resources/targetresourcedirectory?view=graph-rest-beta), [targetResourceGroup](/graph/api/resources/targetresourcegroup?view=graph-rest-beta), [targetResourceOther](/graph/api/resources/targetresourceother?view=graph-rest-beta), [targetResourcePolicy](/graph/api/resources/targetresourcepolicy?view=graph-rest-beta), [targetResourceRole](/graph/api/resources/targetresourcerole?view=graph-rest-beta), [targetResourceServicePrincipal](/graph/api/resources/targetresourceserviceprincipal?view=graph-rest-beta), [targetResourceUser](/graph/api/resources/targetresourceuser?view=graph-rest-beta), [userIdentity](/graph/api/resources/useridentity?view=graph-rest-beta) |

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен сложный тип **privacyProfile** для объекта [organization](/graph/api/resources/organization?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлен сложный тип **legalAgeGroup, ageGroup and consentProvidedForMinor** для объекта [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлена поддержка пользователей и групп для подписок на уведомления [веб-перехватчика](/graph/api/resources/webhooks?view=graph-rest-1.0). |
| Дополнение        | Бета        | Добавлено действие [перечисления удаленных элементов, принадлежащих пользователю,](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta) для ресурса [каталог (удаленные элементы)](/graph/api/resources/directory?view=graph-rest-beta). |

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0          | Добавлено свойство **flag** для объекта [message](/graph/api/resources/message?view=graph-rest-1.0). Добавлен общий сложный тип [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0).|
| Дополнение        | 1.0        | Добавлено свойство **internetMessageHeaders** для объекта [message](/graph/api/resources/message?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлен сложный тип [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлено свойство навигации **messageRules** для объекта [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0). **messageRules** — это набор экземпляров [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлены объект [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0) и сложные типы [messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-1.0), [messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-1.0) и [sizeRange](/graph/api/resources/sizerange?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлены следующие операции CRUD для правил обработки сообщений: [создание](/graph/api/mailfolder-post-messagerules?view=graph-rest-1.0), [перечисление](/graph/api/mailfolder-list-messagerules?view=graph-rest-1.0), [получение](/graph/api/messagerule-get?view=graph-rest-1.0), [обновление](/graph/api/messagerule-update?view=graph-rest-1.0) и [удаление](/graph/api/messagerule-delete?view=graph-rest-1.0). |
| Дополнение | Бета | Добавлен объект [mailSearchFolder](/graph/api/resources/mailsearchfolder?view=graph-rest-beta). |
| Дополнение | Бета | Добавлены следующие API для папки поиска почты: [API создания](/graph/api/mailsearchfolder-post?view=graph-rest-beta), [API обновления](/graph/api/mailsearchfolder-update?view=graph-rest-beta). |
| Изменение | Бета-версия | Для папки поиска почты добавлена поддержка [удаления объекта mailFolder](/graph/api/mailfolder-delete?view=graph-rest-beta), [получения объекта mailFolder](/graph/api/mailfolder-get?view=graph-rest-beta) и [перечисления дочерних папок](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta). |

### <a name="personal-contacts-outlook"></a>Личные контакты (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0          | Добавлено свойство **flag** для объекта [contact](/graph/api/resources/contact?view=graph-rest-1.0). Добавлен общий сложный тип [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0).|

### <a name="reports"></a>Отчеты
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета| Добавлена поддержка делегированного доступа. |
|Дополнение|1.0| Добавлена поддержка делегированного доступа. |

### <a name="security"></a>Безопасность

| **Тип изменения** | **Версия** | **Описание**              |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия       | Добавлен [API безопасности](/graph/api/resources/security-api-overview?view=graph-rest-beta), включающий следующие ресурсы и операции:<br/>[оповещение](/graph/api/resources/alert?view=graph-rest-beta) (и соответствующие объекты);<br/>[получение оповещения](/graph/api/alert-get?view=graph-rest-beta);<br/>[перечисление оповещений](/graph/api/alert-list?view=graph-rest-beta);<br/>[обновление оповещения](/graph/api/alert-update?view=graph-rest-beta).<br/><br/>Добавлена следующая вспомогательная документация:<br/>[сведения об ошибках](/graph/api/resources/security-error-codes?view=graph-rest-beta);<br/>[Интеграция решений по обеспечению безопасности с помощью Microsoft Graph Security API](security-integration.md)

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета-версия|Добавлен новый объект [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлен новый объект [teamGuestSettings](/graph/api/resources/teamguestsettings?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлен новый объект [teamMessagingSettings](/graph/api/resources/teammessagingsettings?view=graph-rest-beta).|
|Дополнение|Бета|Добавлен новый объект [teamFunSettings](/graph/api/resources/teamfunsettings?view=graph-rest-beta).|
|Дополнение|Бета|Добавлена новая операция [удаления канала](/graph/api/channel-delete?view=graph-rest-beta).|
|Дополнение|Бета|Добавлена новая операция [исправления канала](/graph/api/channel-patch?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено новое свойство webUrl для ресурса [команды](/graph/api/resources/team?view=graph-rest-beta).|
|Изменение|бета|Обновлен путь к объекту [channel](/graph/api/resources/channel?view=graph-rest-beta).|

### <a name="users--outlook-settings"></a>Пользователи | Параметры Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлено новое свойство навигации **masterCategories** для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0). **masterCategories** — это коллекция объектов [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлен объект [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлены следующие операции CRUD для объекта [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0): [create](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0), [get](/graph/api/outlookcategory-get?view=graph-rest-1.0), [update](/graph/api/outlookcategory-update?view=graph-rest-1.0) и [delete](/graph/api/outlookcategory-delete?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлена новая функция [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-1.0) для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Добавлена новая функция [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-1.0) для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0). |
|Дополнение | 1.0 | Добавлено новое свойство **workingHours** для объекта [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0). Сведения о поддерживаемых вариантах использования см. в описании [типа ресурса workingHours](/graph/api/resources/workinghours?view=graph-rest-1.0).|
|Дополнение | 1.0 | Добавлены следующие сложные типы: <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-1.0) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-1.0) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-1.0) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-1.0) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-1.0)|


## <a name="march-2018"></a>Март 2018 г.

### <a name="cross-device-experiences-project-rome"></a>Решения для нескольких устройств (Project Rome)

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

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлены новые объекты:<br/>[iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-1.0);<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0).<br/>|
|Дополнение|1.0|Добавлены новые сложные типы:<br/>[appConfigurationSettingItem](/graph/api/resources/intune-apps-appconfigurationsettingitem?view=graph-rest-1.0).<br/>|
|Дополнение|1.0|Добавлено действие [syncLicenses](/graph/api/intune-onboarding-vpptoken-synclicenses?view=graph-rest-1.0) для объекта [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлено свойство навигации **vppTokens** для объекта [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0).|
|Дополнение|Бета-версия|Добавлено свойство **managementCertificateExpirationDate** объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлено свойство **enhancedJailBreak** для сложного типа [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta).|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta);<br/>[androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta);<br/>[androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta);<br/>[androidManagedStoreAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschema?view=graph-rest-beta);<br/>[dataSharingConsent](/graph/api/resources/intune-devices-datasharingconsent?view=graph-rest-beta);<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta);<br/>[macOSEndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-macosendpointprotectionconfiguration?view=graph-rest-beta);<br/>[macOSImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-macosimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta);<br/>[managedEBookCategory](/graph/api/resources/intune-books-managedebookcategory?view=graph-rest-beta);<br/>[microsoftStoreForBusinessContainedApp](/graph/api/resources/intune-apps-microsoftstoreforbusinesscontainedapp?view=graph-rest-beta);<br/>[mobileContainedApp](/graph/api/resources/intune-apps-mobilecontainedapp?view=graph-rest-beta);<br/>[windowsUniversalAppXContainedApp](/graph/api/resources/intune-apps-windowsuniversalappxcontainedapp?view=graph-rest-beta).<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[androidManagedStoreAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem?view=graph-rest-beta);<br/>[deviceAndAppManagementData](/graph/api/resources/intune-onboarding-deviceandappmanagementdata?view=graph-rest-beta);<br/>[loggedOnUser](/graph/api/resources/intune-devices-loggedonuser?view=graph-rest-beta);<br/>[macOSFirewallApplication](/graph/api/resources/intune-deviceconfig-macosfirewallapplication?view=graph-rest-beta);<br/>[macOSLobChildApp](/graph/api/resources/intune-apps-macoslobchildapp?view=graph-rest-beta);<br/>[macOSMinimumOperatingSystem](/graph/api/resources/intune-apps-macosminimumoperatingsystem?view=graph-rest-beta);<br/>[windowsAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsappxappassignmentsettings?view=graph-rest-beta);<br/>[windowsUniversalAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsuniversalappxappassignmentsettings?view=graph-rest-beta).<br/>|
|Дополнение|Бета|Для ресурса [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) добавлено действие [requestSignupUrl](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl?view=graph-rest-beta). |
|Дополнение|бета|Для ресурса [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) добавлено действие [completeSignup](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup?view=graph-rest-beta). |
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

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлены новые объекты:<br/>[baseItemVersion](/graph/api/resources/baseitemversion?view=graph-rest-1.0);<br/>[driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0);<br/>[listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0).<br/> |
|Дополнение|1.0|Добавлены новые сложные типы:<br/>[publicationFacet](/graph/api/resources/publicationfacet?view=graph-rest-1.0).<br/> |
|Дополнение|1.0|Добавлено свойство <b>publication</b> для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлено свойство навигации <b>versions</b> для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлено свойство навигации <b>versions</b> для объекта [listItem](/graph/api/resources/listitem?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлено свойство <b>root</b> для объекта [siteCollection](/graph/api/resources/sitecollection?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлено действие [restoreVersion](/graph/api/driveitemversion-restore?view=graph-rest-1.0) для объекта [driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлено действие [restoreVersion](/graph/api/listitemversion-restore?view=graph-rest-1.0) для объекта [listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0). |
|Дополнение|бета|Добавлен новый сложный тип:<br/>[itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-beta).<br/> |
|Дополнение|Бета|Добавлено свойство <b>name</b> для сложного типа [contentTypeInfo](/graph/api/resources/contenttypeinfo?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено свойство <b>objectType</b> для сложного типа [deleteAction](/graph/api/resources/deleteaction?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено свойство <b>newName</b> для сложного типа [renameAction](/graph/api/resources/renameaction?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено свойство <b>tenantId</b> для сложного типа [sharepointIds](/graph/api/resources/renameaction?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено свойство <b>lastRecordedDateTime</b> для сложного типа [itemActivityTimeSet](/graph/api/resources/itemactivitytimeset?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено свойство [preview](/graph/api/driveitem-preview?view=graph-rest-beta) для объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta). |

### <a name="groups"></a>Группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен объект [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-1.0) |
| Дополнение        | 1.0        | Для политики жизненного цикла группы добавлены API [создания](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-1.0), [перечисления](/graph/api/grouplifecyclepolicy-list?view=graph-rest-1.0), [получения](/graph/api/grouplifecyclepolicy-get?view=graph-rest-1.0), [обновления](/graph/api/grouplifecyclepolicy-update?view=graph-rest-1.0), [удаления](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-1.0), [добавления группы](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-1.0), [удаления группы](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-1.0) |
| Дополнение        | 1.0        | Добавлена функция [перечисления groupLifecyclePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-1.0) для [group](/graph/api/resources/group?view=graph-rest-1.0) |
| Изменение | 1.0 | Добавлено свойство renewedDateTime и [renew](/graph/api/group-renew?view=graph-rest-1.0) для [group](/graph/api/resources/group?view=graph-rest-1.0). |

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Изменение|Бета|Добавлены свойства **applicationID** и **creatorUserID** ресурса [subscription](/graph/api/resources/subscription?view=graph-rest-beta). |
|Изменение|Бета-версия|Добавлена операция [list](/graph/api/subscription-list?view=graph-rest-beta) для объекта [subscription](/graph/api/resources/subscription?view=graph-rest-beta). |

### <a name="identity-and-access--data-policy-operations"></a>Удостоверение и доступ | Операции с политикой данных

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлен новый объект [dataPolicyOperation](/graph/api/resources/datapolicyoperation?view=graph-rest-beta). Он представляет собой отправленную операцию с политикой данных с целью отслеживания.
| Дополнение        | Бета        | Добавлено действие [exportPersonalData](/graph/api/user-exportpersonaldata?view=graph-rest-beta) для [пользователей](/graph/api/resources/users?view=graph-rest-beta). Это действие отправляет запрос на экспорт персональных данных, которые корпорация Майкрософт хранит для пользователя. |

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлен сложный тип **onPremisesExtensionAttributes** для объекта [user](/graph/api/resources/user?view=graph-rest-beta). Он содержит локальные атрибуты расширения AD 1–15. |
| Дополнение        | Бета-версия        | Добавлен сложный тип **privacyProfile** для объекта [organization](/graph/api/resources/organization?view=graph-rest-beta). |
| Дополнение        | 1.0        | Добавлена поддержка [восстановления и окончательного удаления пользователей и групп](/graph/api/resources/directory?view=graph-rest-1.0). |

### <a name="identity-and-access--terms-of-use"></a>Удостоверение и доступ | Условия использования

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены ресурсы [agreement](/graph/api/resources/agreement?view=graph-rest-beta) и [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Для ресурса [agreement](/graph/api/resources/agreement?view=graph-rest-beta) добавлены API [создания](/graph/api/greement-post-agreements?view=graph-rest-beta), [перечисления](/graph/api/agreement-list?view=graph-rest-beta), [получения](/graph/api/agreement-get?view=graph-rest-beta), [обновления](/graph/api/agreement-update?view=graph-rest-beta) и [удаления](/graph/api/agreement-delete?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Для ресурса [user](/graph/api/resources/user?view=graph-rest-beta) добавлены отношения [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta). |

### <a name="reports"></a>Отчеты

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Дополнение|бета|Добавлено свойство **siteId** для объекта [sharePointSiteUsageDetail](/graph/api/resources/sharepointsiteusagedetail?view=graph-rest-beta).|

### <a name="workbooks-and-charts-excel"></a>Книги и диаграммы (Excel)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Изменение|1.0|Добавлено свойство **legacyId** для объекта [Excel Table](/graph/api/resources/table?view=graph-rest-1.0). Оно будет содержать числовой идентификатор (строковый тип данных), который будет оставаться постоянным для определенной таблицы Excel. Это свойство входит в состав дополнительных метаданных, если приложение использует устаревший идентификатор из старых клиентских приложений Excel. Примечание. Свойства `id` и `legacyId` должны интерпретироваться как непрозрачные строковые значения и не должны преобразовываться в другой тип в приложении. |


## <a name="february-2018"></a>Февраль 2018 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета|Добавлены новые объекты:<br/>[androidForWorkImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[androidImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[iosImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-iosimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10importedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10KioskConfiguration](/graph/api/resources/intune-deviceconfig-windows10kioskconfiguration?view=graph-rest-beta)<br/>[windowsPhone81ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлены новые сложные типы:<br/>[importedWindowsAutopilotDeviceIdentityState](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate?view=graph-rest-beta)<br/>|
|Дополнение|Бета|Добавлена функция [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
|Дополнение|Бета|Добавлена функция [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
|Дополнение|Бета|Добавлена функция [managedDeviceEnrollmentFailureTrends](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuretrends?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
|Дополнение|Бета|Добавлена функция [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
|Дополнение|Бета|Добавлена функция [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) для ресурса [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
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

### <a name="reports"></a>Отчеты
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | Бета-версия    | Добавлено свойство **activatedOnSharedComputer** для объекта [userActivationCounts](/graph/api/resources/useractivationcounts?view=graph-rest-beta).|
| Дополнение    | Бета-версия    | Добавлено свойство **sharedComputerActivation** для объекта [office365ActivationsUserCounts](/graph/api/resources/office365activationsusercounts?view=graph-rest-beta).|

### <a name="tasks-and-plans-planner"></a>Задачи и планы (Планировщик)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|бета|Добавлены новые сложные типы:<br/>[plannerPlanContext](/graph/api/resources/plannerplancontext?view=graph-rest-beta);<br/>[plannerPlanContextDetails](/graph/api/resources/plannerplancontextdetails?view=graph-rest-beta);<br/>[plannerPlanContextCollection](/graph/api/resources/plannerplancontextcollection?view=graph-rest-beta);<br/>[plannerPlanContextDetailsCollection](/graph/api/resources/plannerplancontextdetailscollection?view=graph-rest-beta);<br/>[plannerFavoritePlanReference](/graph/api/resources/plannerfavoriteplanreference?view=graph-rest-beta);<br/>[plannerRecentPlanReference](/graph/api/resources/plannerrecentplanreference?view=graph-rest-beta);<br/>[plannerFavoritePlanReferenceCollection](/graph/api/resources/plannerfavoriteplanreferencecollection?view=graph-rest-beta);<br/>[plannerRecentPlanReferenceCollection](/graph/api/resources/plannerrecentplanreferencecollection?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены свойства `favoritePlanReferences` и `recentPlanReferences` для объекта [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлены свойства навигации `favoritePlans` и `recentPlans` для объекта [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено свойство `contexts` для объекта [plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено свойство `contextDetails` для объекта [plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta). |
|Дополнение|Бета|Добавлен [разностный запрос](/graph/api/planneruser-list-delta?view=graph-rest-beta) планировщика. |


## <a name="january-2018"></a>Январь 2018 г.

### <a name="batch-requests"></a>Пакетные запросы

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлена поддержка [пакетной обработки JSON](json-batching.md). Установлено ограничение в 20 внутренних запросов.|
|Изменение|Бета-версия|Максимальное количество внутренних запросов при [пакетной обработке JSON](json-batching.md) увеличено с 5 до 20.|

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|1.0|Добавлены новые объекты:<br/>[androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-1.0);<br/>[androidCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidcustomconfiguration?view=graph-rest-1.0);<br/>[androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-1.0);<br/>[androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-1.0);<br/>[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-1.0);<br/>[androidManagedAppRegistration](/graph/api/resources/intune-mam-androidmanagedappregistration?view=graph-rest-1.0);<br/>[androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-1.0);<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-1.0);<br/>[applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0);<br/>[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-1.0);<br/>[detectedApp](/graph/api/resources/intune-devices-detectedapp?view=graph-rest-1.0);<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-1.0);<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-1.0);<br/>[deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0);<br/>[deviceCategory](/graph/api/resources/intune-shared-devicecategory?view=graph-rest-1.0);<br/>[deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0);<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-1.0);<br/>[deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-1.0);<br/>[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0);<br/>[deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-1.0);<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-1.0);<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-1.0);<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-1.0);<br/>[deviceComplianceScheduledActionForRule](/graph/api/resources/intune-deviceconfig-devicecompliancescheduledactionforrule?view=graph-rest-1.0);<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-1.0);<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-1.0);<br/>[deviceComplianceUserStatus](/graph/api/resources/intune-deviceconfig-devicecomplianceuserstatus?view=graph-rest-1.0);<br/>[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0);<br/>[deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-1.0);<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-1.0);<br/>[deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-1.0);<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-1.0);<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-1.0);<br/>[deviceConfigurationUserStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatus?view=graph-rest-1.0);<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-1.0)<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-1.0);<br/>[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0);<br/>[deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0);<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-1.0);<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-1.0);<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0);<br/>[editionUpgradeConfiguration](/graph/api/resources/intune-deviceconfig-editionupgradeconfiguration?view=graph-rest-1.0);<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-1.0);<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-1.0);<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-1.0);<br/>[iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-1.0);<br/>[iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-1.0);<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-1.0);<br/>[iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-1.0);<br/>[iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-1.0);<br/>[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-1.0);<br/>[iosManagedAppRegistration](/graph/api/resources/intune-mam-iosmanagedappregistration?view=graph-rest-1.0);<br/>[iosStoreApp](/graph/api/resources/intune-apps-iosstoreapp?view=graph-rest-1.0);<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-1.0);<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-1.0);<br/>[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-1.0);<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-1.0);<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-1.0)<br/>[localizedNotificationMessage](/graph/api/resources/intune-notification-localizednotificationmessage?view=graph-rest-1.0);<br/>[macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0);<br/>[macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-1.0);<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-1.0);<br/>[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-1.0);<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-1.0);<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-1.0);<br/>[managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-1.0);<br/>[managedApp](/graph/api/resources/intune-apps-managedapp?view=graph-rest-1.0);<br/>[managedAppConfiguration](/graph/api/resources/intune-mam-managedappconfiguration?view=graph-rest-1.0);<br/>[managedAppOperation](/graph/api/resources/intune-mam-managedappoperation?view=graph-rest-1.0);<br/>[managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-1.0);<br/>[managedAppPolicyDeploymentSummary](/graph/api/resources/intune-mam-managedapppolicydeploymentsummary?view=graph-rest-1.0);<br/>[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0);<br/>[managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0);<br/>[managedAppStatus](/graph/api/resources/intune-mam-managedappstatus?view=graph-rest-1.0);<br/>[managedAppStatusRaw](/graph/api/resources/intune-mam-managedappstatusraw?view=graph-rest-1.0);<br/>[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0);<br/>[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0);<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-1.0);<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-1.0);<br/>[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-1.0);<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-1.0);<br/>[managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-1.0);<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-1.0);<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-1.0);<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-1.0);<br/>[managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-1.0);<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-1.0);<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-1.0);<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-1.0mwindowsinformationprotectionpolicy);<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-1.0);<br/>[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0);<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-1.0);<br/>[mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-1.0);<br/>[mobileAppContent](/graph/api/resources/intune-apps-mobileappcontent?view=graph-rest-1.0);<br/>[mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0);<br/>[mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-1.0);<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-1.0);<br/>[notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-1.0);<br/>[onPremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0);<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0);<br/>[resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-1.0);<br/>[roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-1.0);<br/>[roleDefinition](/graph/api/resources/intune-rbac-roledefinition?view=graph-rest-1.0);<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-1.0);<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-1.0);<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-1.0);<br/>[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0);<br/>targetedManagedAppPolicyAssignment;<br/>[targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-1.0);<br/>[telecomExpenseManagementPartner](/graph/api/resources/intune-tem-telecomexpensemanagementpartner?view=graph-rest-1.0);<br/>[termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-1.0);<br/>[termsAndConditionsAcceptanceStatus](/graph/api/resources/intune-companyterms-termsandconditionsacceptancestatus?view=graph-rest-1.0);<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-1.0);<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-1.0);<br/>[webApp](/graph/api/resources/intune-apps-webapp?view=graph-rest-1.0);<br/>[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-1.0);<br/>[windows10CustomConfiguration](/graph/api/resources/intune-deviceconfig-windows10customconfiguration?view=graph-rest-1.0);<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-1.0)<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-1.0);<br/>[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0);<br/>[windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-1.0)<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-1.0)<br/>[windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-1.0);<br/>[windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-1.0);<br/>[windows81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows81generalconfiguration?view=graph-rest-1.0);<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-1.0);<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-1.0);<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-1.0);<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-1.0);<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-1.0);<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0);<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-1.0);<br/>[windowsPhone81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windowsphone81compliancepolicy?view=graph-rest-1.0);<br/>[windowsPhone81CustomConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81customconfiguration?view=graph-rest-1.0)<br/>[windowsPhone81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81generalconfiguration?view=graph-rest-1.0);<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-1.0);<br/>[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-1.0).<br/>|
|Дополнение|1.0|Добавлены новые сложные типы:<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-1.0);<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-1.0);<br/>[androidMinimumOperatingSystem](/graph/api/resources/intune-apps-androidminimumoperatingsystem?view=graph-rest-1.0);<br/>[androidMobileAppIdentifier](/graph/api/resources/intune-mam-androidmobileappidentifier?view=graph-rest-1.0);<br/>[appListItem](/graph/api/resources/intune-deviceconfig-applistitem?view=graph-rest-1.0);<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-1.0);<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-1.0);<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-1.0);<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devices-deleteuserfromsharedappledeviceactionresult?view=graph-rest-1.0);<br/>[deviceActionResult](/graph/api/resources/intune-devices-deviceactionresult?view=graph-rest-1.0);<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-1.0);<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-1.0);<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-1.0);<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-1.0)<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-devices-deviceexchangeaccessstatesummary?view=graph-rest-1.0);<br/>[deviceGeoLocation](/graph/api/resources/intune-devices-devicegeolocation?view=graph-rest-1.0);<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-1.0);<br/>[deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-1.0);<br/>[deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-1.0);<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-1.0);<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-1.0);<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-1.0);<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-1.0);<br/>[fileEncryptionInfo](/graph/api/resources/intune-apps-fileencryptioninfo?view=graph-rest-1.0);<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-1.0);<br/>[intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-1.0);<br/>[iosDeviceType](/graph/api/resources/intune-apps-iosdevicetype?view=graph-rest-1.0);<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-1.0);<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-1.0)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-1.0)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-1.0)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-1.0);<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-1.0)<br/>[iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0);<br/>[iosMobileAppIdentifier](/graph/api/resources/intune-mam-iosmobileappidentifier?view=graph-rest-1.0);<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-1.0).<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-1.0);<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-1.0);<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-1.0)<br/>[ipRange](/graph/api/resources/intune-mam-iprange?view=graph-rest-1.0);<br/>[iPv4Range](/graph/api/resources/intune-mam-ipv4range?view=graph-rest-1.0);<br/>[iPv6Range](/graph/api/resources/intune-mam-ipv6range?view=graph-rest-1.0);<br/>[keyValuePair](/graph/api/resources/intune-androidforwork-keyvaluepair?view=graph-rest-1.0);<br/>[locateDeviceActionResult](/graph/api/resources/intune-devices-locatedeviceactionresult?view=graph-rest-1.0);<br/>[managedAppDiagnosticStatus](/graph/api/resources/intune-mam-managedappdiagnosticstatus?view=graph-rest-1.0);<br/>[managedAppPolicyDeploymentSummaryPerApp](/graph/api/resources/intune-mam-managedapppolicydeploymentsummaryperapp?view=graph-rest-1.0);<br/>[mediaContentRatingAustralia](/graph/api/resources/intune-deviceconfig-mediacontentratingaustralia?view=graph-rest-1.0);<br/>[mediaContentRatingCanada](/graph/api/resources/intune-deviceconfig-mediacontentratingcanada?view=graph-rest-1.0);<br/>[mediaContentRatingFrance](/graph/api/resources/intune-deviceconfig-mediacontentratingfrance?view=graph-rest-1.0);<br/>[mediaContentRatingGermany](/graph/api/resources/intune-deviceconfig-mediacontentratinggermany?view=graph-rest-1.0);<br/>[mediaContentRatingIreland](/graph/api/resources/intune-deviceconfig-mediacontentratingireland?view=graph-rest-1.0);<br/>[mediaContentRatingJapan](/graph/api/resources/intune-deviceconfig-mediacontentratingjapan?view=graph-rest-1.0);<br/>[mediaContentRatingNewZealand](/graph/api/resources/intune-deviceconfig-mediacontentratingnewzealand?view=graph-rest-1.0);<br/>[mediaContentRatingUnitedKingdom](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedkingdom?view=graph-rest-1.0);<br/>[mediaContentRatingUnitedStates](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedstates?view=graph-rest-1.0);<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-1.0);<br/>[mimeContent](/graph/api/resources/intune-shared-mimecontent?view=graph-rest-1.0);<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-1.0)<br/>[mobileAppIdentifier](/graph/api/resources/intune-mam-mobileappidentifier?view=graph-rest-1.0);<br/>[omaSetting](/graph/api/resources/intune-deviceconfig-omasetting?view=graph-rest-1.0);<br/>[omaSettingBase64](/graph/api/resources/intune-deviceconfig-omasettingbase64?view=graph-rest-1.0);<br/>[omaSettingBoolean](/graph/api/resources/intune-deviceconfig-omasettingboolean?view=graph-rest-1.0);<br/>[omaSettingDateTime](/graph/api/resources/intune-deviceconfig-omasettingdatetime?view=graph-rest-1.0);<br/>[omaSettingFloatingPoint](/graph/api/resources/intune-deviceconfig-omasettingfloatingpoint?view=graph-rest-1.0);<br/>[omaSettingInteger](/graph/api/resources/intune-deviceconfig-omasettinginteger?view=graph-rest-1.0);<br/>[omaSettingString](/graph/api/resources/intune-deviceconfig-omasettingstring?view=graph-rest-1.0);<br/>[omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-1.0);<br/>[proxiedDomain](/graph/api/resources/intune-mam-proxieddomain?view=graph-rest-1.0);<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-1.0);<br/>[resetPasscodeActionResult](/graph/api/resources/intune-devices-resetpasscodeactionresult?view=graph-rest-1.0);<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-1.0);<br/>[rgbColor](/graph/api/resources/intune-onboarding-rgbcolor?view=graph-rest-1.0);<br/>[rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-1.0);<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-1.0);<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-1.0);<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-1.0);<br/>[vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-1.0);<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-1.0);<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-1.0);<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-1.0);<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-1.0);<br/>[windowsDeviceAzureADAccount](/graph/api/resources/intune-devices-windowsdeviceazureadaccount?view=graph-rest-1.0);<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-1.0);<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-1.0);<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-1.0);<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-1.0);<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-1.0);<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-1.0);<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-1.0);<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-1.0);<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-1.0);<br/>[windowsUpdateActiveHoursInstall](/graph/api/resources/intune-deviceconfig-windowsupdateactivehoursinstall?view=graph-rest-1.0);<br/>[windowsUpdateInstallScheduleType](/graph/api/resources/intune-deviceconfig-windowsupdateinstallscheduletype?view=graph-rest-1.0);<br/>[windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-1.0).<br/>|
|Дополнение|1.0|Добавлено действие [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-1.0) для объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлено действие [commit](/graph/api/intune-apps-mobileappcontentfile-commit?view=graph-rest-1.0) для объекта [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0). |
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
|Дополнение|1.0|Добавлено действие [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [updateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-1.0) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [removeAllDevicesFromManagement](/graph/api/intune-devices-user-removealldevicesfrommanagement?view=graph-rest-1.0) для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-1.0) для объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-1.0) для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [scheduleActionsForRules](/graph/api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules?view=graph-rest-1.0) для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [setMobileDeviceManagementAuthority](/graph/api/intune-onboarding-organization-setmobiledevicemanagementauthority?view=graph-rest-1.0) для объекта [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлено действие [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-1.0) для объекта [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [sync](/graph/api/intune-onboarding-devicemanagementexchangeconnector-sync?view=graph-rest-1.0) для объекта [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлено действие [setPriority](/graph/api/intune-onboarding-deviceenrollmentconfiguration-setpriority?view=graph-rest-1.0) для объекта [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0). |
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
|Дополнение|1.0|Добавлено действие [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-1.0) для объекта [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлено действие [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-1.0) для объекта [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0). |
|Дополнение|1.0|Добавлена функция [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-1.0) для объекта [applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-1.0) для объекта [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-1.0) для объекта [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-onboarding-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-1.0) к объекту [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция **getUserIdsWithFlaggedAppRegistration** в коллекции [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [getManagedAppDiagnosticStatuses](/graph/api/intune-mam-user-getmanagedappdiagnosticstatuses?view=graph-rest-1.0) для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [getManagedAppPolicies](/graph/api/intune-mam-user-getmanagedapppolicies?view=graph-rest-1.0) для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0). |
|Дополнение|Версия 1.0|Добавлена функция [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-1.0) для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0). |
|Изменение|Версия 1.0|Добавлено свойство **mobileDeviceManagementAuthority** для объекта [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0).|
|Изменение|Версия 1.0|Добавлено свойство **deviceEnrollmentLimit** для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0).|
|Изменение|Версия 1.0|Добавлены свойства навигации **managedDevices**, **managedAppRegistrations** и **deviceManagementTroubleshootingEvents** для объекта [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0).|
|||
|Дополнение|бета|Добавлены новые объекты:<br/>[deviceManagementScriptAssignment](/graph/api/resources/intune-devices-devicemanagementscriptassignment?view=graph-rest-beta);<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-beta);<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-beta).<br/>|
|Дополнение|бета|Добавлены новые сложные типы:<br/>[revokeAppleVppLicensesActionResult](/graph/api/resources/intune-devices-revokeapplevpplicensesactionresult?view=graph-rest-beta);<br/>[vppTokenRevokeLicensesActionResult](/graph/api/resources/intune-onboarding-vpptokenrevokelicensesactionresult?view=graph-rest-beta).<br/>|
|Дополнение|Бета-версия|Добавлено действие [revokeToken](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketoken?view=graph-rest-beta) для объекта [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-beta) для объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [assign](/graph/api/intune-devices-devicemanagementscript-assign?view=graph-rest-beta) к объекту [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [revokeAppleVppLicenses](/graph/api/intune-devices-manageddevice-revokeapplevpplicenses?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-beta) для объекта [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [revokeLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta) для объекта [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [wipeManagedAppRegistrationsByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationsbydevicetag?view=graph-rest-beta) для объекта [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta). |
|Дополнение|Бета|Добавлено действие [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) для объекта [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлена функция [getEffectiveDeviceEnrollmentConfigurations](/graph/api/intune-onboarding-user-geteffectivedeviceenrollmentconfigurations?view=graph-rest-beta) для объекта [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**appReportingOverviewStatus**<br/>**complianceSettingStateSummary**;<br/>**deviceConfigurationUserStateSummary**;<br/>**eBookGroupAssignment**;<br/>**eBookVppGroupAssignment**;<br/>**mobileAppGroupAssignment**;<br/>**mobileAppVppGroupAssignment**.<br/>|
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
|Изменение|бета|Добавлено свойство **packageId** для объекта [androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **faceIdBlocked** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **members** для объекта [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **macOSRestriction** для объекта [deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **whenPartnerDevicesWillBeRemovedDateTime** и **whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime** для объекта [deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta).|
|Изменение|Бета-версия|Изменен тип следующих свойств объекта [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta):<br/>**scriptContent** со String на Binary.<br/>|
|Изменение|бета|Добавлено свойство **smimeEnablePerMessageSwitch** для объекта [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **identityVersion** для объекта [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **faceIdBlocked** для объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **packageId** и **identityVersion** для объекта [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **azureADDeviceId** и **remoteAssistanceSessionErrorDetails** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **legacyAppConfiguration** для объекта [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **identityVersion** для объекта [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **identityVersion** для объекта [managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta).|
|Изменение|бета|Добавлено свойство **publishingState** для объекта [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **installState** для объекта [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство **identityVersion** для объекта [mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-beta).|
|Изменение|бета|Добавлено свойство **allowPartnerToCollectIOSApplicationMetadata** для объекта [mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta).|
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
|Изменение|бета|Добавлено свойство **showDisplayNameNextToLogo** для сложного типа [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **deviceUsageType** для сложного типа [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta).|
|Изменение|бета|Добавлены свойства **supportsUserLicensing** и **supportsDeviceLicensing** для сложного типа [vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-beta).|
|Изменение|бета|Удалено свойство **actionMessage** для сложного типа [vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta)|

### <a name="education"></a>Образование

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета-версия|Добавлены свойства навигации и улучшена поддержка фильтрации для [API списков](/graph/api/resources/education-overview?view=graph-rest-beta).|

### <a name="reports"></a>Отчеты
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | 1.0    | Добавлены следующие API:<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-1.0);<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-1.0);<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-1.0);<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-1.0);<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-1.0);<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-1.0). |

## <a name="december-2017"></a>Декабрь 2017 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|бета|Добавлены новые объекты:<br/>[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta);<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta);<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-beta);<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta).<br/>|
|Дополнение|бета|Добавлены новые сложные типы:<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-beta);<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-beta);<br/>[vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta);<br/>[windowsDeviceAADAccount](/graph/api/resources/intune-devices-windowsdeviceaadaccount?view=graph-rest-beta);<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-beta);<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-beta).<br/>|
|Дополнение|Бета-версия|Добавлено действие [revokeTokens](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketokens?view=graph-rest-beta) для объекта [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [createToken](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-createtoken?view=graph-rest-beta) для объекта [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [updateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [revokeLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta) для объекта [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлена функция [getDevicePasscode](/graph/api/intune-deviceconfig-devicecompliancepolicy-getdevicepasscode?view=graph-rest-beta) для коллекции [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлена функция [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-beta) для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta). |
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
|Изменение|бета|Добавлено свойство **minimumUpdateAutoInstallClassification** для объекта [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **defenderSecurityCenterDisableAppBrowserUI**, **defenderSecurityCenterDisableFamilyUI**, **defenderSecurityCenterDisableHealthUI**, **defenderSecurityCenterDisableNetworkUI**, **defenderSecurityCenterDisableVirusUI**, **defenderSecurityCenterOrganizationDisplayName**, **defenderSecurityCenterHelpEmail**, **defenderSecurityCenterHelpPhone**, **defenderSecurityCenterHelpURL**, **defenderSecurityCenterNotificationsFromApp**, **defenderSecurityCenterITContactDisplay** и **applicationGuardAllowVirtualGPU** для объекта [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **enableAutomaticRedeployment** и **authenticationAllowFIDODevice** для объекта [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **trustedNetworkDomains** для объекта [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **minimumUpdateAutoInstallClassification** для объекта [windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **androidForWorkEnrollmentProfiles** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **healthAttestationSupportedStatus** для сложного типа [deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **tpmSpecificationVersion**, **operatingSystemEdition**, **deviceFullQualifiedDomainName**, **deviceGuardVirtualizationBasedSecurityHardwareRequirementState**, **deviceGuardVirtualizationBasedSecurityState** и **deviceGuardLocalSystemAuthorityCredentialGuardState** для сложного типа [hardwareInformation](/graph/api/resources/intune-devices-hardwareinformation?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **vpnConfigurationId** для сложного типа [iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **resourceActions** для сложного типа [rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-beta).|

### <a name="reports"></a>Отчеты
| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Дополнение    | 1.0    | Добавлены следующие API:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-1.0);<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-1.0);<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-1.0);<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-1.0);<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-1.0);<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-1.0);<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-1.0);<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0);<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-1.0);<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-1.0);<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-1.0);<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0);<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-1.0);<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0);<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-1.0);<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-1.0);<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0);<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0);<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-1.0);<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-1.0);<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-1.0);<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-1.0);<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-1.0);<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-1.0);<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-1.0);<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0);<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-1.0);<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-1.0);<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-1.0);<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-1.0);<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-1.0);<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-1.0);<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-1.0);<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0);<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-1.0);<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-1.0);<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-1.0);<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-1.0);<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-1.0);<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-1.0);<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-1.0);<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-1.0);<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-1.0);<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-1.0);<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-1.0);<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-1.0);<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-1.0);<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-1.0);<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-1.0);<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-1.0);<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-1.0);<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-1.0);<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-1.0);<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-1.0)<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-1.0);<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-1.0);<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-1.0).|
| Дополнение    | Бета-версия    | Добавлены следующие API:<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-beta);<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-beta);<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-beta);<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-beta);<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-beta);<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-beta). |

### <a name="track-changes"></a>Отслеживание изменений

| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Изменение      | 1.0    | Добавлена возможность фильтрации разностных запросов [пользователей](/graph/api/user-delta?view=graph-rest-1.0) и [групп](/graph/api/group-delta?view=graph-rest-1.0). |


## <a name="november-2017"></a>Ноябрь 2017 г.

### <a name="change-notifications-webhooks"></a>Уведомления об изменениях (веб-перехватчики)

| Тип изменения | Версия | Описание                              |
|:------------|:--------|:-----------------------------------------|
| Критическое изменение | Бета-версия и версия 1.0 | Сокращен [максимальный период действия подписки](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type) с использованием [веб-перехватчиков](/graph/api/resources/webhooks?view=graph-rest-1.0) для элементов в корне диска. Новое значение — поддерживаемый максимальный срок действия для элементов в корне диска. |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|бета|Добавлены новые объекты:<br/>[auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta);<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-beta);<br/>[deviceSetupConfiguration](/graph/api/resources/intune-deviceconfig-devicesetupconfiguration?view=graph-rest-beta);<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-beta);<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-beta);<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta);<br/>[ndesConnector](/graph/api/resources/intune-deviceconfig-ndesconnector?view=graph-rest-beta).<br/>|
|Дополнение|бета|Добавлены новые сложные типы:<br/>[auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta);<br/>[auditProperty](/graph/api/resources/intune-auditing-auditproperty?view=graph-rest-beta);<br/>[auditResource](/graph/api/resources/intune-auditing-auditresource?view=graph-rest-beta);<br/>[bulkManagedDeviceActionResult](/graph/api/resources/intune-devices-bulkmanageddeviceactionresult?view=graph-rest-beta);<br/>[deviceProtectionOverview](/graph/api/resources/intune-devices-deviceprotectionoverview?view=graph-rest-beta);<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-beta);<br/>[operatingSystemVersionRange](/graph/api/resources/intune-deviceconfig-operatingsystemversionrange?view=graph-rest-beta);<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-beta).<br/>|
|Дополнение|Бета-версия|Добавлено действие executeAction для коллекции [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [shutDown](/graph/api/intune-devices-manageddevice-shutdown?view=graph-rest-beta) для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-beta) для объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-beta) для объекта [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие setDefaultProfile для объекта [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлено действие shareForSchoolDataSyncService для объекта [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
|Дополнение|бета|Добавлено действие unshareForSchoolDataSyncService для объекта [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлена функция getAuditCategories для коллекции [auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta). |
|Дополнение|Бета-версия|Добавлена функция getAuditActivityTypes для коллекции [auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta). |
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**mobileAppIdentifierDeployment**.<br/>|
|Удаление|Бета-версия|Удалены следующие сложные типы:<br/>**windowsInformationProtectionCloudResource**;<br/>**windowsInformationProtectionCloudResourceCollection**.<br/>|
|Изменение|Бета-версия|Изменены следующие свойства объекта [androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta):<br/>свойство **passcode** сделано необязательным.<br/>|
|Изменение|Бета-версия|Добавлены свойства **microsoftStoreForBusinessLastSuccessfulSyncDateTime**, **isEnabledForMicrosoftStoreForBusiness**, **microsoftStoreForBusinessLanguage** и **microsoftStoreForBusinessLastCompletedApplicationSyncTime** для объекта [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **target** для объекта [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **deviceProtectionOverview** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **exchangeAlias** и **exchangeOrganization** для объекта [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta).|
|Изменение|бета|Добавлены свойства **appStoreUrl** и **minimumSupportedOperatingSystem** для объекта [managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **remoteAssistanceSessionErrorString** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **appStoreUrl**, **applicableDeviceType** и **minimumSupportedOperatingSystem** для объекта [managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **notApplicableDeviceCount**, **pendingInstallDeviceCount**, **notApplicableUserCount** и **pendingInstallUserCount** для объекта [mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалены свойства **targetedSecurityGroupIds** и **targetedSecurityGroupsCount** объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалены свойства **targetedSecurityGroupsCount** и **targetedSecurityGroupIds** объекта [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **validOperatingSystemBuildRanges** для объекта [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства **activeFirewallRequired**, **uacRequired** и **validOperatingSystemBuildRanges** для объекта [ windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **enableExpeditedTelemetryReporting** для объекта [windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалены свойства **allowedApps**, **enterpriseCloudResources** и **targetedSecurityGroupIds** объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta).|
|Изменение|бета|Добавлено свойство **ignoreVersionDetection** для объекта [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **mobileAppIdentifierDeployments** объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **mobileAppIdentifierDeployments** объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **assignments** для объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **deviceConfiguration** объекта [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **deviceConfiguration** для объекта [deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлены свойства навигации **deviceSetupConfigurations**, **ndesConnectors**, **exchangeOnPremisesPolicies**, **conditionalAccessSettings**, **auditEvents** и **troubleshootingEvents** для объекта [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta).|
|Изменение|бета|Удалено свойство навигации **mobileAppIdentifierDeployments** объекта [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство навигации **windowsProtectionState** для объекта [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалены свойства навигации **mobileAppIdentifierDeployments** и **targetedSecurityGroups** объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **targetedSecurityGroups** объекта [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство навигации **deviceManagementTroubleshootingEvents** для объекта [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **allowedAppLockerFiles** объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta).|
|Изменение|Бета-версия|Удалено свойство навигации **windowsProtectionState** объекта [windowsManagedDevice](/graph/api/resources/intune-devices-windowsmanageddevice?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **v11_0** для сложного типа [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-beta).|
|Изменение|Бета-версия|Добавлено свойство **denied** для сложного типа [windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta).|

### <a name="education"></a>Образование

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета-версия|Добавлена поддержка сценариев для образования, в том числе следующих ресурсов:<br/>[учебные заведения](/graph/api/resources/educationschool?view=graph-rest-beta);<br/>[занятия](/graph/api/resources/educationclass?view=graph-rest-beta);<br/>[пользователи](/graph/api/resources/educationuser?view=graph-rest-beta);<br/>[назначения](/graph/api/resources/educationassignment?view=graph-rest-beta);<br/>[сданные работы](/graph/api/resources/educationsubmission?view=graph-rest-beta).<br/>Сведения о доступных методах см. в статьях об этих ресурсах.|

### <a name="identity-and-access--synchronization"></a>Удостоверение и доступ | Синхронизация

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета-версия    | Добавлена поддержка синхронизации удостоверений Azure AD, в том числе следующих ресурсов:<br/>[задание](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta);<br/>[схема](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta);<br/>[шаблон](/graph/api/resources/synchronization-synchronizationtemplate?view=graph-rest-beta).<br/>Сведения о доступных методах см. в статьях об этих ресурсах.|

### <a name="reports"></a>Отчеты
| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета-версия    | Добавлена поддержка JSON для следующих API:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta);<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta);<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta);<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta);<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta);<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta);<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta);<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta);<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta);<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta);<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta);<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta);<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta);<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta);<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta);<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta);<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta);<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta);<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta);<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta);<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta);<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta);<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta);<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta);<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta);<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta);<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta);<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta);<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta);<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta);<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta);<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta);<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta);<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta);<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta);<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta);<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta);<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta);<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta);<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-beta);<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-beta);<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-beta);<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-beta);<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-beta);<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-beta)<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-beta);<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-beta);<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-beta) |


## <a name="october-2017"></a>Октябрь 2017 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|бета|Добавлены новые объекты:<br/>[androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfigurationAssignment](/graph/api/resources/intune-apps-ioslobappprovisioningconfigurationassignment?view=graph-rest-beta)<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-beta)<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-beta)<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-beta)<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-beta)<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-beta)<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta)<br/>[windows10PFXImportCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pfximportcertificateprofile?view=graph-rest-beta)<br/>[windowsAssignedAccessProfile](/graph/api/resources/intune-deviceconfig-windowsassignedaccessprofile?view=graph-rest-beta)<br/>[windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta)<br/>|
|Дополнение|бета|Добавлены новые сложные типы:<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-beta)<br/>[iosSingleSignOnSettings](/graph/api/resources/intune-deviceconfig-iossinglesignonsettings?view=graph-rest-beta)<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-beta)<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta)<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-beta)<br/>[proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta)<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-beta)<br/>[windowsStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-windowsstoreforbusinessappassignmentsettings?view=graph-rest-beta)<br/>|
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
|Изменение|бета|Удалено свойство навигации **deviceCompliancePolicy** объекта [deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta).|
|Изменение|бета|Добавлено свойство навигации **deviceCompliancePolicy** для объекта [deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta).|
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
|Изменение|Бета-версия|Изменен тип следующих свойств сложного типа [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta):<br/>вместо Int32 для **errorCode** теперь используется Int64.<br/>|
|Изменение|Бета-версия|Изменен тип следующих свойств сложного типа [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta):<br/>вместо Int32 **errorCode** теперь используется Int64.<br/>|
|Изменение|Бета-версия|Изменен тип следующих свойств сложного типа [windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta):<br/>вместо **enterpriseCloudResources** [windowsNetworkIsolationCloudResourceCollection](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationcloudresourcecollection?view=graph-rest-beta) теперь используется коллекция [proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta);<br/>вместо **enterpriseInternalProxyServers** windowsNetworkIsolationResourceCollection теперь используется коллекция строк;<br/>**enterpriseIPRanges** windowsNetworkIsolationIPRangeCollection теперь используется коллекция [ipRange](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta);<br/>вместо **enterpriseNetworkDomainNames** windowsNetworkIsolationResourceCollection теперь используется коллекция строк;<br/>вместо **enterpriseProxyServers** windowsNetworkIsolationResourceCollection теперь используется коллекция строк;<br/>вместо **neutralDomainResources** windowsNetworkIsolationResourceCollection теперь используется коллекция строк.<br/>|

### <a name="identity-and-access-azure-ad"></a>Удостоверение и доступ (Azure AD)

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
|Дополнение|Бета-версия|Добавлены объект [identityProvider](/graph/api/resources/identityprovider?view=graph-rest-beta) и операции [create](/graph/api/identityprovider-post-identityproviders?view=graph-rest-beta), [list](/graph/api/identityprovider-list?view=graph-rest-beta), [get](/graph/api/identityprovider-get?view=graph-rest-beta), [update](/graph/api/identityprovider-update?view=graph-rest-beta) и [delete](/graph/api/identityprovider-delete?view=graph-rest-beta).|

### <a name="mail-outlook"></a>Почта (Outlook)

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Это улучшение поведения связано с получением общей почтовой папки или содержимого сообщений в ней, если кто-то предоставил вошедшему пользователю доступ к почтовой папке или делегировал ему почтовый ящик пользователя. В таких случаях приложение может указать ИД пользователя или имя участника-пользователя, чтобы [получить эту общую почтовую папку](/graph/api/mailfolder-get?view=graph-rest-1.0) или [получить сообщения из этого общего календаря](/graph/api/user-list-messages?view=graph-rest-1.0), при условии что вошедший пользователь предоставил приложению делегированные разрешения. |

### <a name="reports"></a>Отчеты
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

### <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

|Тип изменения|Версия|Описание|
|:---|:---|:---|
|Дополнение|Бета-версия|Добавлен новый объект [team](/graph/api/resources/team?view=graph-rest-beta).|
|Дополнение|Бета-версия|Добавлены операции [create](/graph/api/team-put-teams?view=graph-rest-beta), [get](/graph/api/team-get?view=graph-rest-beta) и [update](/graph/api/team-update?view=graph-rest-beta) для объекта [team](/graph/api/resources/team?view=graph-rest-beta).|

### <a name="users--outlook-settings"></a>Пользователи | Параметры Outlook

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
|Дополнение | Бета-версия | Добавлено новое свойство **workingHours** для объекта [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta). Сведения о поддерживаемых вариантах использования см. в описании [типа ресурса workingHours](/graph/api/resources/workinghours?view=graph-rest-beta).|
|Дополнение | Бета-версия | Добавлены следующие сложные типы: <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-beta) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-beta) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-beta) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-beta) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-beta)|


## <a name="september-2017"></a>Сентябрь 2017 г.

### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | Бета          | Добавлены функции [findRoomLists](/graph/api/user-findroomlists?view=graph-rest-beta) и [findRooms](/graph/api/user-findrooms?view=graph-rest-beta) для объекта [user](/graph/api/resources/user?view=graph-rest-beta). |
| Дополнение        | Бета          | Добавлено свойство **locations** для объекта [event](/graph/api/resources/event?view=graph-rest-beta), позволяющее организовать событие, в котором могут участвовать пользователи из нескольких расположений. |
| Дополнение        | Бета          | Добавлено свойство **locationType** для сложного типа [location](/graph/api/resources/location?view=graph-rest-beta). |
| Дополнение        | Бета          | Добавлены свойства **uniqueId** и **uniqueIdType** для сложного типа [location](/graph/api/resources/location?view=graph-rest-beta). В настоящее время эти свойства предназначены только для внутреннего использования. |
| Изменение          | 1.0 и бета-версия | Это улучшение поведения связано с получением общего календаря или содержимого событий в нем, если кто-то предоставил вошедшему пользователю доступ к календарю или делегировал ему почтовый ящик пользователя. В таких случаях приложение может указать ИД пользователя или имя участника-пользователя, чтобы [получить этот общий календарь](/graph/api/calendar-get?view=graph-rest-1.0) или [получить события из этого общего календаря](/graph/api/user-list-events?view=graph-rest-1.0), при условии что вошедший пользователь предоставил приложению делегированные разрешения. |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | бета    | Добавлены новые объекты:<br/>[activeDirectoryWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[azureADWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-beta)<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta)<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-beta)<br/>[windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta)<br/>[windows10NetworkBoundaryConfiguration](/graph/api/resources/intune-deviceconfig-windows10networkboundaryconfiguration?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta)<br/> |
| Дополнение    | бета    | Добавлены новые сложные типы:<br/>[adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta)<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-beta)<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-beta)<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-beta)<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta)<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-beta)<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-beta)<br/>[outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-beta)<br/>windowsNetworkIsolationCloudResource<br/>windowsNetworkIsolationCloudResourceCollection<br/>windowsNetworkIsolationIPRangeCollection<br/>[windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta)<br/>windowsNetworkIsolationResourceCollection<br/> |
| Дополнение    | Бета    | Добавлено действие [sync](/graph/api/intune-enrollment-windowsautopilotsettings-sync?view=graph-rest-beta) для объекта [windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta). |
| Дополнение    | бета    | Добавлено действие [assign](/graph/api/intune-enrollment-windowsautopilotdeploymentprofile-assign?view=graph-rest-beta) для объекта [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta). |
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
| Изменение      | бета    | Добавлено свойство **adminConsent** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
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
| Изменение      | бета    | Добавлены свойства навигации **windowsAutopilotSettings**, **windowsAutopilotDeviceIdentities**, **windowsAutopilotDeploymentProfiles**, **deviceEnrollmentConfigurations**, **deviceManagementPartners** и **depOnboardingSettings** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение      | Бета    | Удалено свойство навигации **cloudPkiSubscriptions** объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **assignments** для объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **assignments** для объекта [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство навигации **assignments** для объекта [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta). |

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

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

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство **internetMessageHeaders** для объекта [message](/graph/api/resources/message?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлен сложный тип [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлено свойство навигации **messageRules** для объекта [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta). **messageRules** — это набор экземпляров [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлены объект [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta) и сложные типы [messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-beta), [messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-beta) и [sizeRange](/graph/api/resources/sizerange?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлены следующие операции CRUD для правил обработки сообщений: [create](/graph/api/mailfolder-post-messagerules?view=graph-rest-beta), [list](/graph/api/mailfolder-list-messagerules?view=graph-rest-beta), [get](/graph/api/messagerule-get?view=graph-rest-beta), [update](/graph/api/messagerule-update?view=graph-rest-beta) и [delete](/graph/api/messagerule-delete?view=graph-rest-beta). |

### <a name="personal-contacts-outlook"></a>Личные контакты (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Это улучшение поведения связано с получением общей папки контактов или содержимого контактов в ней, если кто-то предоставил вошедшему пользователю доступ к папке контактов или делегировал ему почтовый ящик пользователя. В таких случаях приложение может указать ИД пользователя или имя участника-пользователя, чтобы [получить эту общую папку контактов](/graph/api/contactfolder-get?view=graph-rest-1.0) или [получить контакты из этой общей папки](/graph/api/user-list-contacts?view=graph-rest-1.0), при условии что вошедший пользователь предоставил приложению делегированные разрешения. |

### <a name="sites-and-lists-sharepoint"></a>Сайты и списки (SharePoint)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлены новые объекты: [ColumnDefinition][], [ColumnLink][], [ContentType][], [List][], [ListItem][]. |
| Дополнение        | 1.0        | Добавлены связи **columns**, **contentTypes**, **items** и **lists** для ресурса [Site][]. |
| Дополнение        | 1.0        | Добавлены новые сложные типы: [BooleanColumn][], [CalculatedColumn][], [ChoiceColumn][], [ContentTypeInfo][], [ContentTypeOrder][], [CurrencyColumn][], [DateTimeColumn][], [DefaultColumnValue][], [ListInfo][], [LookupColumn][], [NumberColumn][], [PersonOrGroupColumn][], [SystemFacet][], [TextColumn][]. |
| Дополнение        | Бета        | Добавлены новые объекты: [BaseItemVersion][BaseItemVersion-beta], [ColumnLink][ColumnLink-beta], [ContentType][ContentType-beta], [ListItemVersion][ListItemVersion-beta], |
| Дополнение        | Бета        | Добавлены свойства **columnGroup**, **currency**, **defaultValue** и **displayName** для объекта [ColumnDefinition][ColumnDefinition-beta]. |
| Дополнение        | Бета        | Добавлены свойства **displayName** и **system** для ресурса [List][List-beta]. |
| Дополнение        | Бета        | Добавлены связи **activities** и **contentTypes** для ресурса [List][List-beta]. |
| Дополнение        | Бета        | Добавлено свойство **contentType** для ресурса [ListItem][ListItem-beta]. |
| Дополнение        | Бета        | Добавлены связи **activities** и **versions** для ресурса [ListItem][ListItem-beta]. |
| Дополнение        | Бета        | Добавлена связь **contentTypes** для ресурса [Site][Site-beta]. |
| Дополнение        | Бета        | Добавлено свойство **outputType** для типа [BooleanColumn][BooleanColumn-beta]. |
| Дополнение        | Бета        | Добавлены новые сложные типы: [ContentTypeInfo][ContentTypeInfo-beta], [ContentTypeOrder][ContentTypeOrder-beta], [CurrencyColumn][CurrencyColumn-beta] и [SystemFacet][SystemFacet-beta]. |
| Дополнение        | Бета        | Добавлено свойство **contentTypesEnabled** для сложного типа [ListInfo][ListInfo-beta]. |
| Дополнение        | Бета        | Добавлено свойство **allowUnlimitedLength** для сложного типа [LookupColumn][LookupColumn-beta]. |
| Изменение          | Бета        | Имя свойства **allowMultipleValue** изменено на **allowMultipleValues** для сложного типа [LookupColumn][LookupColumn-beta]. |
| Изменение          | Бета        | Имя свойства **chooseFrom** изменено на **chooseFromType** для сложного типа [PersonOrGroupColumn][PersonOrGroupColumn-beta]. |
| Удаление        | Бета        | Удалено свойство **locale** сложного типа [NumberColumn][NumberColumn-beta]. |
| Удаление        | Бета        | Удалено свойство **enforceUniqueValues** сложного типа [PersonOrGroupColumn][PersonOrGroupColumn-beta]. |
| Дополнение        | Бета        | Добавлены свойства **dataLocationCode** и **root** для сложного типа [SiteCollection][SiteCollection-beta]. |

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
[SiteCollection-beta]: /graph/api/resources/sitecollection?view=graph-rest-beta
[SystemFacet-beta]: /graph/api/resources/systemfacet?view=graph-rest-beta
[SystemFacet]: /graph/api/resources/systemfacet?view=graph-rest-1.0
[TextColumn]: /graph/api/resources/textcolumn?view=graph-rest-1.0


### <a name="users--outlook-settings"></a>Пользователи | Параметры Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлено новое свойство навигации **masterCategories** для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta). **masterCategories** — это коллекция объектов [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлен объект [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлены следующие операции CRUD для объекта [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta): [создание](/graph/api/outlookuser-post-mastercategories?view=graph-rest-beta), [получение](/graph/api/outlookcategory-get?view=graph-rest-beta), [обновление](/graph/api/outlookcategory-update?view=graph-rest-beta) и [удаление](/graph/api/outlookcategory-delete?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлена новая функция [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-beta) для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлена новая функция [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-beta) для объекта [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta). |


## <a name="august-2017"></a>Август 2017 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | Бета-версия    | Добавлен новый объект:<br/>[windowsPrivacyDataAccessControlItem](/graph/api/resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem?view=graph-rest-beta)<br/> |
| Дополнение    | бета    | Добавлены новые сложные типы:<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-beta)<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-beta)<br/> |
| Дополнение    | Бета-версия    | Добавлено действие [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-beta) для [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Дополнение    | Бета-версия    | Добавлено действие [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-beta) для [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Дополнение    | Бета-версия    | Добавлено действие [windowsPrivacyAccessControls](/graph/api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols?view=graph-rest-beta) для [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлены свойства **automaticallyUpdateApps** и **countryOrRegion** для объекта [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta) |
| Изменение      | бета    | Добавлено свойство **enableAuthenticationViaCompanyPortal** для объекта [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) |
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
| Изменение      | бета    | Добавлено свойство **secureByDefault** для сложного типа [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Добавлено свойство **restartMode** для сложного типа [windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta) |

### <a name="groups"></a>Группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена сущность [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлены следующие API для политики жизненного цикла группы, а именно для: [создания](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-beta), [перечисления](/graph/api/grouplifecyclepolicy-list?view=graph-rest-beta), [получения](/graph/api/grouplifecyclepolicy-get?view=graph-rest-beta), [обновления](/graph/api/grouplifecyclepolicy-update?view=graph-rest-beta), [удаления](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-beta), [добавления группы](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-beta), [удаления группы](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-beta) и [возобновления группы](/graph/api/grouplifecyclepolicy-renewgroup?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлена функция [List groupLifecylePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-beta) для объекта [group](/graph/api/resources/group?view=graph-rest-beta). |

### <a name="notes-onenote"></a>Заметки (OneNote)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлено свойство навигации [onenote](/graph/api/resources/onenote?view=graph-rest-1.0) для **site**. |
| Дополнение        | Бета          | Добавлены целевые параметры *siteCollectionId* и *siteId* для операций копирования. Пример: [CopyNotebook](/graph/api/notebook-copynotebook?view=graph-rest-1.0). |

### <a name="social-and-workplace-intelligence--people"></a>Социальная и рабочая аналитика | Пользователи

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | В версию 1.0 добавлены интерфейсы [People API](/graph/api/resources/person?view=graph-rest-1.0). Подробные сведения об этих API см. в статье, посвященной [получению релевантной информации о людях](people-example.md). |
| Дополнение        | 1.0        | Добавлено разрешение People.Read.All. Дополнительные сведения см. в [справочнике по разрешениям](permissions-reference.md). |
| Дополнение        | 1.0        | Добавлен ресурс [personType](/graph/api/resources/persontype?view=graph-rest-1.0). |
| Изменение          | 1.0        | Ресурс [scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0) заменил ресурс **rankedEmailAddress**. |
| Изменение          | 1.0        | Ресурс [person](/graph/api/resources/person?view=graph-rest-1.0) был обновлен следующим образом:<ul><li>Свойство **scoredEmailAddresses** (коллекция типа [scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0)) заменило свойство **emailAddresses**.</li><li>Свойство **jobTitle** заменило свойство **title**.</li><li>Удалены свойства **sources** и **mailboxType**.</li><li>Свойство **personType** теперь имеет тип [personType](/graph/api/resources/persontype?view=graph-rest-1.0), а не строковый, и заменяет существовавшие ранее свойства **sources** и **mailboxType**.</li><li>Добавлено свойство **imAddress**.</li></ul> |
| Удаление        | 1.0        | Удален ресурс **personDataSource**. |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство **employeeId** для [user](/graph/api/resources/user?view=graph-rest-beta). |

## <a name="july-2017"></a>Июль 2017 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

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

### <a name="identity-and-access--group-setting"></a>Удостоверение и доступ | Параметры группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлена поддержка параметров группы.<br/>Новые типы ресурсов: [groupSetting](/graph/api/resources/groupsetting?view=graph-rest-1.0), [groupSettingTemplate](/graph/api/resources/groupsettingtemplate?view=graph-rest-1.0), [settingValue](/graph/api/resources/settingvalue?view=graph-rest-1.0) и [settingTemplateValue](/graph/api/resources/settingtemplatevalue?view=graph-rest-1.0). |
| Изменение          | 1.0        | Добавлено свойство **classification** и свойство навигации **settings** для [group](/graph/api/resources/group?view=graph-rest-1.0). |


## <a name="june-2017"></a>Июнь 2017 г.

### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Повышен уровень для следующих 4 свойств [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) до версии 1.0: **canEdit**, **canShare**, **canViewPrivateItems** и **owner**. |

### <a name="cross-device-experiences-project-rome"></a>Решения для нескольких устройств (Project Rome)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены следующие ресурсы и API:<br/>[Действие](/graph/api/resources/projectrome-activity?view=graph-rest-beta)<br/>[Создание или замена действия](/graph/api/projectrome-put-activity?view=graph-rest-beta)<br/>[Удаление действия](/graph/api/projectrome-delete-activity?view=graph-rest-beta)<br/>[Элемент журнала](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta)<br/>[Создание или замена элемента журнала](/graph/api/projectrome-put-historyitem?view=graph-rest-beta)<br/>[Удаление элемента журнала](/graph/api/projectrome-delete-historyitem?view=graph-rest-beta) |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | бета    | Добавлены новые объекты:<br/>[defaultDeviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-defaultdevicecompliancepolicy?view=graph-rest-beta);<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta);<br/>[deviceManagementScriptDeviceState](/graph/api/resources/intune-devicefe-devicemanagementscriptdevicestate?view=graph-rest-beta);<br/>[deviceManagementScriptRunSummary](/graph/api/resources/intune-devicefe-devicemanagementscriptrunsummary?view=graph-rest-beta);<br/>[deviceManagementScriptUserState](/graph/api/resources/intune-devicefe-devicemanagementscriptuserstate?view=graph-rest-beta);<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-beta);<br/>[windowsManagedDevice](/graph/api/resources/intune-devicefe-windowsmanageddevice?view=graph-rest-beta);<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-devicefe-windowsmanagementapphealthstate?view=graph-rest-beta)<br/>[windowsManagementAppHealthSummary](/graph/api/resources/intune-devicefe-windowsmanagementapphealthsummary?view=graph-rest-beta).<br/> |
| Дополнение    | бета    | Добавлены новые сложные типы:<br/>[bitLockerFixedDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerfixeddrivepolicy?view=graph-rest-beta);<br/>[bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta);<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-beta);<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devicefe-deleteuserfromsharedappledeviceactionresult?view=graph-rest-beta);<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-beta).<br/> |
| Удаление    | Бета-версия    | Удалены следующие объекты:<br/>**deviceManagementScriptState**<br/> |
| Удаление    | Бета-версия    | Удалено действие wipeByDeviceTag для [user](/graph/api/resources/intune-devicefe-user?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **innerAuthenticationProtocolForEapTtls**, **innerAuthenticationProtocolForPeap** и **outerIdentityPrivacyTemporaryValue** для объекта [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **nonEapAuthenticationMethodForEapTtls**, **nonEapAuthenticationMethodForPeap** и **enableOuterIdentityPrivacy** для объекта [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta). |
| Изменение      | бета    | Добавлено свойство **deployedAppCount** для объекта [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалены свойства **instanceDisplayName** и **settingPlatform** для объекта [complianceSettingStateSummary](/graph/api/resources/compliancesettingstatesummary?view=graph-rest-beta). |
| Изменение      | бета    | Добавлено свойство **deployedAppCount** для объекта [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **excludeGroup** для объекта [deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta) |
| Изменение      | Бета-версия    | Удалены свойства **instanceDisplayName** и **settingPlatform** для объекта [deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Удалено свойство **devicePlatform** для объекта [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлены свойства **assignmentStatus**, **assignmentProgress** и **assignmentErrorMessage** для объекта [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta). |
| Изменение      | бета    | Добавлено свойство **intuneBrand** для объекта [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
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

### <a name="identity-and-access--application"></a>Удостоверение и доступ | Приложение

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | Обновление API приложений. Это первый набор изменений, включающий изменение структуры и переименование свойств объекта [application](/graph/api/resources/application?view=graph-rest-beta).<br/>**Новые объекты:** [api](/graph/api/resources/api?view=graph-rest-beta]), [informationalUrl](/graph/api/resources/informationalurl?view=graph-rest-beta), [installedClient](/graph/api/resources/installedclient?view=graph-rest-beta), [permissionScope](/graph/api/resources/permissionscope?view=graph-rest-beta), [preauthorizedApplication](/graph/api/resources/preauthorizedapplication?view=graph-rest-beta), [web](/graph/api/resources/web?view=graph-rest-beta).<br/>**Удаленные свойства:** addIns, appRoles, availableToOtherOrganizations, knownClientApplications, oauth2AllowUrlPathMatching, recordConsentConditions.<br/>**Переименованные свойства:** с appId на id, с identifierUris на applicationAliases, с availableToOtherTenants на orgRestrictions, с mainLogo на logo, с oauth2Permissions на publishedPermissionsScopes, с publicClient на allowPublicClient, с replyUrls на redirectUrls.<br/>**Новые свойства:** tags. |

### <a name="tasks-and-plans-planner"></a>Задачи и планы (Планировщик)
| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Удаление        | Бета-версия        | Удалены следующие объекты:<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard** |

### <a name="cross-device-experiences-project-rome"></a>Решения для нескольких устройств (Project Rome)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавлена поддержка Project Rome, в том числе [получения списка устройств](/graph/api/user-list-devices?view=graph-rest-beta), [отправки команды устройству](/graph/api/send-device-command?view=graph-rest-beta) и [проверки состояния команды](/graph/api/get-device-command-status?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена поддержка ресурсов [activity](/graph/api/resources/projectrome-activity?view=graph-rest-beta) и [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta) для объектов user, включая [создание или замену activity](/graph/api/projectrome-put-activity?view=graph-rest-beta) и [создание или замену historyItem](/graph/api/projectrome-put-historyitem?view=graph-rest-beta). |

### <a name="identity-and-access--administrative-unit"></a>Удостоверение и доступ | Административная единица

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | Тип свойства roleMemberInfo объекта [scopedRoleMembership](/graph/api/resources/scopedrolemembership?view=graph-rest-beta) изменен на [identity](/graph/api/resources/identity?view=graph-rest-1.0). |
| Изменение          | Бета        | Свойство навигации scopedAdministratorOf объекта [user](/graph/api/resources/user?view=graph-rest-beta) заменено на scopedRoleMemberOf. |
| Изменение          | Бета        | Свойство навигации scopedAdministrators объекта [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) заменено на scopedRoleMembers. |
| Изменение          | Бета        | Свойство навигации scopedAdministrators объекта [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-beta) заменено на scopedMembers. |

### <a name="change-notifications-webhooks"></a>Уведомления об изменениях (веб-перехватчики)

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
| Изменение        | Бета       | Добавлена поддержка пользователей и групп в [веб-перехватчиках](/graph/api/resources/webhooks?view=graph-rest-beta).

### <a name="track-changes"></a>Отслеживание изменений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлена поддержка функции delta в версии 1.0. Она позволяет выполнять [разностный запрос](delta-query-overview.md) для следующих объектов:<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Примеры см. в следующих статьях:<br/>[Получение добавочных изменений для групп](delta-query-groups.md)<br/>[Получение добавочных изменений для сообщений в папке](delta-query-messages.md)<br/>[Получение добавочных изменений для пользователей](delta-query-users.md) |
| Изменение          | Бета        | Добавлена возможность дополнительной фильтрации запросов (по идентификатору) для [пользователей](/graph/api/user-delta?view=graph-rest-beta) и [групп](/graph/api/group-delta?view=graph-rest-beta). |

### <a name="added-user-resource-support-for-deleted-items"></a>Добавлена поддержка работы с удаленными элементами для ресурса user

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена поддержка [восстановления и окончательного удаления пользователей](/graph/api/resources/directory?view=graph-rest-beta). |

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
| Дополнение        | 1.0        | Добавлены операции с [domains](/graph/api/resources/domain?view=graph-rest-1.0).<br/>Новые объекты:</br>[domain](/graph/api/resources/domain?view=graph-rest-1.0);<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-1.0);<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-1.0);<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-1.0);<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-1.0);<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-1.0);<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-1.0).<br/>Новые действия:</br>[verify](/graph/api/domain-verify?view=graph-rest-1.0). |

### <a name="added-contracts-to-v10"></a>Добавлены контракты в версии 1.0

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Новый объект:</br>[contract](/graph/api/resources/contract?view=graph-rest-1.0) |

### <a name="added-licensedetails-to-v10"></a>Добавлен объект licenseDetails в версии 1.0

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Новый объект:</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-1.0) |
| Изменение          | 1.0        | Добавлено свойство навигации [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-1.0) для объекта [user](/graph/api/resources/user?view=graph-rest-1.0). |


### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Дополнение | 1.0 | Добавлен тип ресурса **baseItem**, состоящий из базовых свойств объекта **driveItem**.
| Дополнение | 1.0 и бета | В объект **thumbnail** добавлено свойство **sourceItemId**. <br/> В объект **sharepointIds** добавлено свойство **siteUrl**. <br/> В объект **shared** добавлены свойства **sharedBy** и **sharedDateTime**. <br/> В объект **remoteItem** добавлено свойство **shared**. <br/> В объекты**drive** и **itemReference** добавлено свойство **sharepointIds**. <br/> В объект **fileSystemInfo** добавлено свойство **lastAccessedDateTime**. <br/> В объект **sharedDriveItem** добавлены свойства навигации **driveItem** и **site**. <br/> В объект **baseItem** добавлено свойство **parentReference**.
| Изменение | 1.0 и бета | Объекты **driveItem** и **sharedDriveItem** теперь наследуются от объекта **baseItem**. <br/> Тип **identity** отмечен как открытый.
| Изменение | Бета | В объект **sharingLink** добавлены свойства **configuratorUrl** и **webHtml**. <br/> Добавлены тип ресурса **folderView** и свойство **view** для типа ресурса **folder**. <br/> В объект **driveItem** добавлено свойство навигации **listItem**. <br/> В объект **drive** добавлено свойство навигации **list**.


### <a name="add-custom-data-open-extensions"></a>Добавление пользовательских данных (открытые расширения)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Поддержка [openTypeExtension](/graph/api/resources/opentypeextension?view=graph-rest-1.0) в ресурсах [device](/graph/api/resources/device?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0), [organization](/graph/api/resources/organization?view=graph-rest-1.0) и [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Дополнение        | 1.0 и бета-версия | Если пользователь вошел с помощью личной учетной записи Майкрософт, открытые расширения поддерживаются в ресурсах event, post, group, message, contact и user. (При использовании рабочей или учебной учетной записи открытые расширения также поддерживаются в ресурсах device, group, organization и user.) |
| Дополнение        | 1.0 и бета-версия | Поддержка параметра `$expand` для [получения открытых расширений](/graph/api/opentypeextension-get?view=graph-rest-1.0) в ресурсах [device](/graph/api/resources/device?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0), [organization](/graph/api/resources/organization?view=graph-rest-1.0), [post](/graph/api/resources/post?view=graph-rest-1.0) и [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Дополнение        | Бета          | Поддержка параметра `$expand` для [получения открытых расширений](/graph/api/opentypeextension-get?view=graph-rest-1.0) в объекте [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta). |


### <a name="add-custom-data-schema-extensions"></a>Добавление пользовательских данных (расширения схемы)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0          | Новый ресурс [schemaExtension](/graph/api/resources/schemaextension?view=graph-rest-1.0) и методы CRUD для управления определениями расширений для следующих ресурсов: [contact](/graph/api/resources/contact?view=graph-rest-1.0), [device](/graph/api/resources/device?view=graph-rest-1.0), [event](/graph/api/resources/event?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0), [message](/graph/api/resources/message?view=graph-rest-1.0), [organization](/graph/api/resources/organization?view=graph-rest-1.0), [post](/graph/api/resources/post?view=graph-rest-1.0) и [user](/graph/api/resources/user?view=graph-rest-1.0). Обратите внимание, что объект [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) по-прежнему поддерживается только в бета-версии. |
| Дополнение        | 1.0          | Существующие методы POST, GET и PATCH ресурсов [contact](/graph/api/resources/contact?view=graph-rest-1.0), [device](/graph/api/resources/device?view=graph-rest-1.0), [event](/graph/api/resources/event?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0), [message](/graph/api/resources/message?view=graph-rest-1.0), [organization](/graph/api/resources/organization?view=graph-rest-1.0), [post](/graph/api/resources/post?view=graph-rest-1.0) и [user](/graph/api/resources/user?view=graph-rest-1.0) теперь поддерживают добавление, получение, обновление и удаление пользовательских данных, хранящихся в виде расширений схемы в соответствующих экземплярах ресурсов. |
| Дополнение        | 1.0 и бета-версия | Теперь вы можете использовать параметр `$filter` для поиска экземпляров ресурсов, свойства которых совпадают с определенным значениями свойств расширений, например имени. Эта возможность рассматривается подробнее в этом [примере](extensibility-schema-groups.md#5-get-a-group-and-its-extension-data). |
| Изменение          | 1.0 и бета | [Удаление определения расширения схемы](/graph/api/schemaextension-delete?view=graph-rest-1.0) больше не влияет на доступ к пользовательским данным, добавленным на основе этого определения. |
| Изменение          | 1.0 и бета | Теперь вы можете задать для сложного типа расширения схемы значение null, чтобы удалить расширение схемы из экземпляра ресурса. |


### <a name="groups"></a>Группы

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Дополнение | 1.0 и бета | Добавлены свойства навигации **drives** и **sites** для объекта **group**.

### <a name="social-and-workplace-intelligence--insights"></a>Социальная и рабочая аналитика | Аналитические сведения

|**Тип изменения**|**Версия**|**Описание**|
|:-------------|:-----------|:--------------|
|Дополнение|Бета|Добавлен [API Shared](/graph/api/resources/insights-shared?view=graph-rest-beta).<br />Новые ресурсы:<br />[sharingDetail](/graph/api/resources/insights-sharingdetail?view=graph-rest-beta) <br />[insightIdentity](/graph/api/resources/insights-insightidentity?view=graph-rest-beta) <br />
|Дополнение|Бета|Добавлен [API Used](/graph/api/resources/insights-used?view=graph-rest-beta).<br />Новые ресурсы:<br />[usageDetails](/graph/api/resources/insights-usagedetails?view=graph-rest-beta) <br />
|Изменение|Бета|Новое свойство **Type** в<br />ресурсе [resourceVisualization](/graph/api/resources/insights-resourcevisualization?view=graph-rest-beta). <br />
|Удаление|Бета-версия|Удалены следующие объекты:<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | бета    | Добавлены новые объекты:<br/>[androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta)<br/>[cartToClassAssociation](/graph/api/resources/intune-deviceconfig-carttoclassassociation?view=graph-rest-beta)<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta)<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-beta)<br/>[eBookVppGroupAssignment](/graph/api/resources/intune-books-ebookvppgroupassignment?view=graph-rest-beta)<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta)<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta)<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)<br/>[windowsDeviceMalwareState](/graph/api/resources/intune-endpointprotection-windowsdevicemalwarestate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-beta)<br/>[windowsMalwareInformation](/graph/api/resources/intune-endpointprotection-windowsmalwareinformation?view=graph-rest-beta)<br/>[windowsProtectionState](/graph/api/resources/intune-endpointprotection-windowsprotectionstate?view=graph-rest-beta)<br/> |
| Дополнение    | бета    | Добавлены новые сложные типы:<br/>[androidPermissionAction](/graph/api/resources/intune-apps-androidpermissionaction?view=graph-rest-beta)<br/>[bitLockerSystemDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockersyst?view=graph-rest-betarivepolicy)<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-beta)<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-beta)<br/> |
| Дополнение    | Бета    | Добавлено действие [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) для объекта [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-beta) для объекта [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta). |
| Дополнение    | Бета    | Добавлено действие [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-beta) для объекта [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta). |
| Удаление    | Бета-версия    | Удалены следующие объекты:<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/> |
| Удаление    | Бета-версия    | Удалены следующие сложные типы:<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/> |
| Изменение      | бета    | Добавлены свойства **workProfilePasswordBlockFingerprintUnlock**, **workProfilePasswordBlockTrustAgents**, **workProfilePasswordExpirationDays**, **workProfilePasswordMinimumLength**, **workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**, **workProfilePasswordPreviousPasswordBlockCount**, **workProfilePasswordSignInFailureCountBeforeFactoryReset**, **workProfilePasswordRequiredType** и **workProfileRequirePassword** для объекта [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta). |
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
| Изменение      | Бета    | Удалено свойство **creationOptions** из объекта [event](/graph/api/resources/event?view=graph-rest-beta) |
| Изменение      | Бета    | Удалено свойство **isDelegated** для объекта [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-beta). |
| Изменение      | Бета    | Удалены свойства **unseenConversationsCount** и **unseenMessagesCount** для объекта [group](/graph/api/resources/group?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлены свойства **settingXml** и **settings** для объекта [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta). |
| Изменение      | Бета    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [iosPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-iospkcscertificateprofile?view=graph-rest-beta). |
| Изменение      | Бета-версия    | Добавлено свойство **subjectAlternativeNameFormatString** для объекта [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta). |
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
| Изменение      | Бета-версия    | Добавлены свойства **subjectNameFormatString** и **subjectAlternativeNameFormatString** для объекта [windowsPhone81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81scepcertificateprofile?view=graph-rest-beta). |
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


### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Для метода **findMeetingTimes** добавлено значение перечисления **unrestricted**, указываемое в качестве свойства **activityDomain** в составе параметра **timeConstraint**. Это позволяет методу **findMeetingTimes** искать интервалы времени, соответствующие типу планируемого мероприятия. Дополнительные сведения см. в разделе [request body](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body). |
| Дополнение        | Бета-версия          | Содержание объекта **event** теперь можно получать в виде обычного текста, а не только в формате HTML. Дополнительные сведения см. в описаниях событий [get](/graph/api/event-get?view=graph-rest-beta) и [list](/graph/api/user-list-events?view=graph-rest-beta). |

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | Содержание объекта **message** теперь можно получать в виде обычного текста, а не только в формате HTML. Дополнительные сведения см. в описаниях событий [get](/graph/api/message-get?view=graph-rest-beta) и [list](/graph/api/user-list-messages?view=graph-rest-beta). |


### <a name="to-do-tasks-outlook"></a>Задачи из списка дел (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | В объект [user](/graph/api/resources/user?view=graph-rest-beta) добавлено новое свойство навигации **outlook** для доступа к задачам Outlook. |
| Дополнение        | Бета        | Новые объекты [outlookuser](/graph/api/resources/outlookuser?view=graph-rest-beta), [outlookTaskGroup](/graph/api/resources/outlooktaskgroup?view=graph-rest-beta), [outlookTaskFolder](/graph/api/resources/outlooktaskfolder?view=graph-rest-beta) и [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-beta), а также их методы поддерживают доступ к задачам Outlook. |
| Дополнение        | Бета        | Задачи Outlook поддерживают вложения (ресурсы [attachment](/graph/api/resources/attachment?view=graph-rest-beta), [fileAttachment](/graph/api/resources/fileattachment?view=graph-rest-beta), [itemAttachment](/graph/api/resources/itemattachment?view=graph-rest-beta) и [referenceAttachment](/graph/api/resources/referenceattachment?view=graph-rest-beta)). |
| Дополнение        | Бета        | Задачи Outlook поддерживают [расширенные свойства](/graph/api/resources/extended-properties-overview?view=graph-rest-beta) (ресурсы [singleValueLegacyExtendedProperty](/graph/api/resources/singlevaluelegacyextendedproperty?view=graph-rest-beta) и [multiValueLegacyExtendedProperty](/graph/api/resources/multivaluelegacyextendedproperty?view=graph-rest-beta)). |

### <a name="tasks-and-plans-planner"></a>Задачи и планы (Планировщик)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен [API Планировщика](/graph/api/resources/planner-overview?view=graph-rest-1.0).<br />Новые ресурсы:<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-1.0) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-1.0); <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-1.0); <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-1.0); <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-1.0); <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-1.0); <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-1.0); <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-1.0). |

### <a name="sites-and-lists-sharepoint"></a>Сайты и списки (SharePoint)

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Дополнение      | 1.0      | Теперь в конечной точке версии 1.0 доступен ресурс сайтов.<br/> Добавлены типы ресурсов **site** и **siteCollection**.
| Изменение        | Бета      | Изменился формат идентификатора ресурса **site**. Это критическое изменение в бета-версии API.
| Удаленные элементы       | Бета      | Объект **sharePoint** удален из бета-версии API. Эта функциональность теперь доступна из коллекции **sites**.

### <a name="sites-and-lists-sharepoint"></a>Сайты и списки (SharePoint)

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:----------|:--------------|
| Изменение | Бета | Удалены свойства навигации **sharepoint**. Теперь для доступа к сайтам используется свойство навигации **sites**. <br/> Удален ресурс **fieldDefinition**. Он заменен ресурсом **columnDefinition**. <br/> Удалены свойства **siteCollectionId** и **siteId** объекта **site**. Используйте вместо них свойство **sharepointIds**. <br/> Удалено свойство **listItemId** объекта **listItem**. Используйте вместо него свойство **sharepointIds**. <br/> Свойство **columnSet** объекта **listItem** переименовано на **fields**. <br/> Идентификаторы ресурсов **site** теперь включают имя узла SharePoint.
| Дополнение | Бета | Добавлены типы ресурсов **booleanColumn**, **calculatedColumn**, **choiceColumn**, **dateTimeColumn**, **lookupColumn**, **numberColumn**, **personOrGroupColumn** и **textColumn**. <br/> В объект **site** добавлено свойство **displayName**. <br/> В объект **site** добавлено свойство навигации **columns**. <br/> В объект **sharedDriveItem** добавлены свойства навигации **list** и **listItem**. <br/> В объекты **list**, **listItem** и **site** добавлено свойство **sharepointIds**. <br/> Добавлен тип ресурса **columnDefinition**.




## <a name="april-2017"></a>Апрель 2017 г.

### <a name="identity-and-access--administrative-unit"></a>Удостоверение и доступ | Административная единица

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | Обновления API административных единиц будут предоставлены в бета-версиях. Первый набор изменений будет применен 3 мая 2017 г. Изменения включают в себя следующие переименования:<br />сложный тип - **roleMemberInfo** для объекта scopedRoleMembership теперь зовется **identity**;<br />свойство навигации - **scopedAdministratorOf** для объекта user теперь зовется **scopedRoleMemberOf**;<br />свойство навигации - **scopedAdministrators** для объекта administrativeUnit теперь зовется **scopedRoleMembers**;<br />свойство навигации - **scopedAdministrators** для объекта directoryRole теперь зовется **scopedMembers**. |

### <a name="identity-and-access"></a>Удостоверение и доступ

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | API [application](/graph/api/resources/application?view=graph-rest-beta) и [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) будут обновлены в бета-версии. Первый набор изменений будет применен 15 мая 2017 г. Изменения включают переименование и реструктуризацию свойств. Некоторые свойства (например, appRoles и addIns) будут доступны только после применения изменений. Прежде чем выйдет версия 1.0 с изменениями, будут выпущены бета-версии. |

### <a name="cloud-solution-provider"></a>Cloud Solution Provider

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Приложения, разрешение на использование которых было заранее предоставлено согласно программе Cloud Solution Provider, теперь могут вызывать Microsoft Graph. Описание см. в новой [статье об авторизации](auth-cloudsolutionprovider.md). |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | К объекту [user](/graph/api/resources/user?view=graph-rest-beta) добавлены новые свойства для onPremises: onPremisesDomainName, OnPremisesSamAccountName и onPremisesUserPrincipalName. |

### <a name="groups"></a>Группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета-версия        | Добавлено значение **HiddenMembership** для свойства видимости объекта [Group](/graph/api/resources/group?view=graph-rest-beta). |

### <a name="tasks-and-plans-planner"></a>Задачи и планы (Планировщик)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлен новый [API Планировщика](/graph/api/resources/planner-overview?view=graph-rest-beta).<br />Новые ресурсы:<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-beta); <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta); <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-beta); <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-beta); <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-beta); <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-beta); <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-beta). |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)
| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлены новые объекты:<br/>[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta);<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta);<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-beta);<br/>[deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta)<br/>[deviceManagementScriptGroupAssignment](/graph/api/resources/intune-deviceconfig-devicemanagementscriptgroupassignment?view=graph-rest-beta)<br/>[deviceManagementScriptState](/graph/api/resources/intune-deviceconfig-devicemanagementscriptstate?view=graph-rest-beta)<br/>[eBookGroupAssignment](/graph/api/resources/intune-books-ebookgroupassignment?view=graph-rest-beta);<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-beta);<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta);<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-beta);<br/>[windowsManagementApp](/graph/api/resources/intune-deviceconfig-windowsmanagementapp?view=graph-rest-beta)<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-deviceconfig-windowsmanagementapphealthstate?view=graph-rest-beta)<br/> |
| Дополнение        | бета        | Добавлены новые сложные типы:<br/>[dailySchedule](/graph/api/resources/intune-deviceconfig-dailyschedule?view=graph-rest-beta)<br/>[hourlySchedule](/graph/api/resources/intune-deviceconfig-hourlyschedule?view=graph-rest-beta)<br/>[iosBookmark](/graph/api/resources/intune-deviceconfig-iosbookmark?view=graph-rest-beta);<br/>[iosWebContentFilterAutoFilter](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterautofilter?view=graph-rest-beta);<br/>[iosWebContentFilterBase](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterbase?view=graph-rest-beta);<br/>[iosWebContentFilterSpecificWebsitesAccess](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterspecificwebsitesaccess?view=graph-rest-beta);<br/>[runSchedule](/graph/api/resources/intune-deviceconfig-runschedule?view=graph-rest-beta)<br/>[sharedAppleDeviceUser](/graph/api/resources/intune-deviceconfig-sharedappledeviceuser?view=graph-rest-beta)<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-beta).<br/> |
| Дополнение        | Бета-версия        | Добавлено действие [requestRemoteAssistance](/graph/api/intune-devices-manageddevice-requestremoteassistance?view=graph-rest-beta) к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлено действие [cleanWindowsDevice](/graph/api/intune-devices-manageddevice-cleanwindowsdevice?view=graph-rest-beta) к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлено действие [logoutSharedAppleDeviceActiveUser](/graph/api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser?view=graph-rest-beta) к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлено действие [deleteUserFromSharedAppleDevice](/graph/api/intune-devices-manageddevice-deleteuserfromsharedappledevice?view=graph-rest-beta) к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлено действие [assign](/graph/api/intune-deviceconfig-devicemanagementscript-assign?view=graph-rest-beta) к объекту [deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta). |
| Дополнение        | Бета        | Добавлено действие [syncLicenses](/graph/api/intune-onboarding-applevolumepurchaseprogramtoken-synclicenses?view=graph-rest-beta) к объекту [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена функция **getTopMobileApps** для коллекции [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена функция [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-deviceconfig-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-beta) к объекту [applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена функция [getDeviceComplianceSettingStates](/graph/api/intune-deviceconfig-devicemanagement-getdevicecompliancesettingstates?view=graph-rest-beta) к объекту [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена функция [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-beta) к объекту [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлена функция [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-beta) к объекту [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta). |
| Удаление        | Бета-версия        | Удалены следующие сложные типы:<br/>**enterpriseCloudResource**;<br/>**windowsInformationProtectionAppRule**;<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**<br/>**windowsInformationProtectionAppRuleDesktopTemplate**<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**<br/>**windowsInformationProtectionAppRuleTemplate**<br/>**windowsInformationProtectionCorporateNetworkLocation**<br/>**windowsInformationProtectionProtectedLocation**<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**<br/>**windowsInformationProtectionProtectedLocationNeutralResources**<br/> |
| Изменение          | бета        | Добавлено свойство **deviceSharingAllowed** к объекту [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Удалено **deviceSharingBlocked** свойство из объекта [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **minimumRequiredSdkVersion** к объекту [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **windowsManagementAppEnabled** к объекту [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **notificationTemplateId** к объекту [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлено свойство **excludeGroup** к объекту [deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta) |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-beta):<br/>**payloadFileName** теперь можно не указывать.<br/> |
| Изменение          | Бета-версия        | Добавлено свойство **contentFilterSettings** к объекту [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta). |
| Изменение          | Бета        | Добавлены свойства **cellularBlockPersonalHotspot** и **passcodeBlockFingerprintModification** к объекту [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta). |
| Изменение          | Бета        | Добавлено свойство **minimumRequiredSdkVersion** к объекту [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Изменены следующие свойства объекта [macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-beta):<br/>**payloadFileName** теперь можно не указывать.<br/> |
| Изменение          | Бета-версия        | Добавлены свойства **disableAppPinIfDevicePinIsSet**, **minimumRequiredOsVersion**, **minimumWarningOsVersion**, **minimumRequiredAppVersion** и **minimumWarningAppVersion** к объекту [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta). |
| Изменение          | Бета-версия        | Добавлены свойства **remoteAssistanceSessionUrl**, **isEncrypted**, **model** и **manufacturer** к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
| Изменение          | Бета        | Изменены следующие свойства объекта [getMobileAppCount](/graph/api/intune-apps-mobileapp-getmobileappcount?view=graph-rest-beta):<br/>для **bindingParameter** вместо **mobileApp** теперь используется **коллекция** *mobileApp*;<br/>для свойства **status** вместо типа GUID теперь используется String.<br/> |
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
| Изменение          | бета        | Изменены следующие свойства сложного типа [omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-beta):<br/>**fileName** больше не обязательно указывать.<br/> |

## <a name="march-2017"></a>Март 2017 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | бета    | Добавлены новые объекты:<br/>[androidForWorkApp](/graph/api/resources/intune-apps-androidforworkapp?view=graph-rest-beta);<br/>[androidForWorkAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschema?view=graph-rest-beta);<br/>[androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta);<br/>[androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta);<br/>[applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta)<br/>[complianceSettingStateSummary](/graph/api/resources/intune-deviceconfig-compliancesettingstatesummary?view=graph-rest-beta);<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-beta);<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-beta);<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-beta);<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-beta);<br/>[enterpriseCodeSigningCertificate](/graph/api/resources/intune-apps-enterprisecodesigningcertificate?view=graph-rest-beta);<br/>[iosEduDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosedudeviceconfiguration?view=graph-rest-beta);<br/>[managedDeviceCertificateState](/graph/api/resources/intune-devices-manageddevicecertificatestate?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta);<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta);<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy);<br/>[mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta);<br/>[mobileAppProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-mobileappprovisioningconfiggroupassignment?view=graph-rest-beta);<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta);<br/>[officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta);<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-beta);<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-beta);<br/>[symantecCodeSigningCertificate](/graph/api/resources/intune-apps-symanteccodesigningcertificate?view=graph-rest-beta);<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta);<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta);<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-beta);<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta);<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta).<br/> |
| Дополнение    | бета    | Добавлены новые сложные типы:<br/>[androidForWorkAppConfigurationExample](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexample?view=graph-rest-beta);<br/>[androidForWorkAppConfigurationExampleJson](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexamplejson?view=graph-rest-beta);<br/>[androidForWorkAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschemaitem?view=graph-rest-beta);<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta);<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta);<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-deviceconfig-deviceexchangeaccessstatesummary?view=graph-rest-beta)<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-beta);<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-beta);<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-beta);<br/>[excludedApps](/graph/api/resources/intune-apps-excludedapps?view=graph-rest-beta);<br/>[iosEduCertificateSettings](/graph/api/resources/intune-deviceconfig-ioseducertificatesettings?view=graph-rest-beta);<br/>[ipRange](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta);<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta);<br/>[windowsInformationProtectionCloudResource](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresource?view=graph-rest-beta);<br/>[windowsInformationProtectionCloudResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresourcecollection?view=graph-rest-beta);<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-beta);<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-beta);<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-beta);<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-beta).<br/> |
| Дополнение    | Бета    | Добавлено действие [requestSignupUrl](/graph/api/intune-androidforwork-androidforworksettings-requestsignupurl?view=graph-rest-beta) к объекту [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta). |
| Дополнение    | бета    | Добавлено действие [completeSignup](/graph/api/intune-androidforwork-androidforworksettings-completesignup?view=graph-rest-beta) к объекту [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta). |
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
| Дополнение    | бета    | Добавлено действие [updateTargetedSecurityGroups](/graph/api/intune-mam-windowsinformationprotection-updatetargetedsecuritygroups?view=graph-rest-beta) к объекту [windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлено действие [updateTargetedSecurityGroups](/graph/api/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy-updatetargetedsecuritygroups) к объекту [mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy). |
| Дополнение    | Бета-версия    | Добавлено действие [wipeManagedAppRegistrationByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationbydevicetag?view=graph-rest-beta) к объекту [user](/graph/api/resources/intune-deviceconfig-user?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлена функция [getTopMobileApps](/graph/api/intune-apps-mobileapp-gettopmobileapps?view=graph-rest-beta) к объекту [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta). |
| Дополнение    | Бета-версия    | Добавлена функция [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-corpenrollment-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-beta) к объекту [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta). |
| Удаление    | Бета-версия    | Удалены следующие объекты:<br/>**appProvisioningConfigGroupAssignment**;<br/>**defaultManagedAppConfiguration**;<br/>**enterpriseCertificate**;<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**;<br/>**symantecCertificate**;<br/>**windows10WindowsInformationProtectionConfiguration**.<br/> |
| Удаление    | Бета-версия    | Удалены следующие сложные типы:<br/>**mobileAppInstallSummary**;<br/>**windowsArchitecture**;<br/>**windowsDeviceType**.<br/> |
| Изменение      | Бета    | Добавлено свойство **webBrowserBlockPopups** к объекту [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta). |
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
| Изменение      | Бета    | Добавлено свойство навигации **managedDeviceCertificateStates** к объекту [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta). |
| Изменение      | бета    | Добавлены свойства навигации **deviceConfigurationStates** и **deviceCompliancePolicyStates** к объекту [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta). |
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

### <a name="identity-and-access"></a>Удостоверение и доступ

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Новый ресурс:</br>[contract](/graph/api/resources/contract?view=graph-rest-beta). |
| Дополнение        | Бета-версия        | Добавлены функции к объектам [domains](/graph/api/resources/domain?view=graph-rest-beta).<br/>Новые объекты:</br>[domain](/graph/api/resources/domain?view=graph-rest-beta);<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-beta);<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-beta);<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-beta);<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-beta);<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-beta);<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-beta).<br/>Новые действия:</br>[forceDelete](/graph/api/domain-forcedelete?view=graph-rest-beta);</br>[verify](/graph/api/domain-verify?view=graph-rest-beta). |

### <a name="add-custom-data-schema-extensions"></a>Добавление пользовательских данных (расширения схемы)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Добавление данных приложения в Microsoft Graph с помощью [расширений схемы](extensibility-overview.md#schema-extensions)  поддерживается для следующих ресурсов:<br/>administrative unit;<br/>calendar event;<br/>device;<br/>group;<br/>message;<br/>organization;<br/>personal contact;<br/>post;<br/>user<br/>Пример приведен в следующей статье:<br/>[Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](extensibility-schema-groups.md). |
| Дополнение        | бета        | Предоставлен альтернативный способ создания определения расширения схемы без подтвержденного личного домена .com. Подробности см. в разделе [Расширения схемы](extensibility-overview.md#schema-extensions). |

### <a name="add-custom-data-open-extensions"></a>Добавление пользовательских данных (открытые расширения)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Вместо термина "расширения данных Office 365" теперь используется "открытые расширения". |
| Дополнение        | Бета-версия          | Добавлены ресурсы, которые поддерживают [открытые расширения](extensibility-overview.md#open-extensions): <br/>administrative unit;<br/>device;<br/>group<br/>organization;<br/>user<br/>Пример приведен в следующей статье:<br/>[Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](extensibility-open-users.md). |

### <a name="identity-and-access-directory-apis"></a>Удостоверение и доступ (API каталогов)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена поддержка [восстановления и окончательного удаления групп](/graph/api/resources/directory?view=graph-rest-beta).<br/>Новый объект: каталог со свойством навигации deleteditems. |
| Дополнение        | Бета        | Новый объект:</br>[Конечная точка](/graph/api/resources/endpoint?view=graph-rest-beta) |
| Изменение          | Бета        | Новое свойство навигации [endpoints](/graph/api/group-list-endpoints?view=graph-rest-beta) для ресурса [group](/graph/api/resources/group?view=graph-rest-beta) |
| Дополнение        | Бета        | Новый объект:</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-beta) |
| Изменение          | бета        | Добавлено свойство навигации [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-beta) для объекта [user](/graph/api/resources/user?view=graph-rest-beta). |
| Дополнение        | Бета        | Новый объект:</br>[contract](/graph/api/resources/contract?view=graph-rest-beta). |

### <a name="reports"></a>Отчеты

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Представлена предварительная версия нового API для функций создания отчетов в Office 365. С его помощью можно получать отчеты об использовании служб Office 365 сотрудниками компании. Например, вы можете определить, кто использует службу по максимуму, а кому вообще не нужна лицензия Office 365. Дополнительные сведения см. в статье о ресурсе [report](/graph/api/resources/report?view=graph-rest-beta). |


## <a name="february-2017"></a>Февраль 2017 г.

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

| Тип изменения | Версия | Описание                              |
| :---------- | :------ | :--------------------------------------- |
| Дополнение    | бета    | Добавлены новые объекты:<br/>[androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta)<br/>[androidForWorkEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkeasemailprofilebase?view=graph-rest-beta)<br/>[androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidForWorkGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgmaileasconfiguration?view=graph-rest-beta)<br/>[androidForWorkNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworknineworkeasconfiguration?view=graph-rest-beta)<br/>[androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta)<br/>[androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta)<br/>[androidForWorkTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidforworktrustedrootcertificate?view=graph-rest-beta)<br/>[androidForWorkWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkwificonfiguration?view=graph-rest-beta)<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-beta)<br/>[appProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-appprovisioningconfiggroupassignment?view=graph-rest-beta)<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta)<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta)<br/>[enterpriseCertificate](/graph/api/resources/intune-apps-enterprisecertificate?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappprovisioningconfigurationdevicestatus?view=graph-rest-beta)<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta)<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta)<br/>[symantecCertificate](/graph/api/resources/intune-apps-symanteccertificate?view=graph-rest-beta)<br/>[windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta)<br/>[windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta)<br/>[windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta)<br/>[windowsPhone81AppXBundle](/graph/api/resources/intune-apps-windowsphone81appxbundle?view=graph-rest-beta)<br/>[windowsPhoneXAP](/graph/api/resources/intune-apps-windowsphonexap?view=graph-rest-beta)<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta)<br/> |
| Дополнение    | бета    | Добавлены новые сложные типы:<br/>[airPrintDestination](/graph/api/resources/intune-deviceconfig-airprintdestination?view=graph-rest-beta)<br/>[windowsArchitecture](/graph/api/resources/intune-apps-windowsarchitecture?view=graph-rest-beta)<br/>[windowsDeviceType](/graph/api/resources/intune-apps-windowsdevicetype?view=graph-rest-beta)<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta)<br/>[windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta)<br/> |
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
| Изменение      | бета    | Удалено свойство **numberOfTargetedSecurityGroups** из объекта [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta). |
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

### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Новое действие [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) для ресурса [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Дополнение        | 1.0        | Новый сложный тип [attendeeBase](/graph/api/resources/attendeebase?view=graph-rest-1.0), который состоит из свойства типа участников. |
| Дополнение        | 1.0        | Новые сложные типы:<br/>[attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-1.0)<br/>[locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-1.0) <br/>[locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-1.0)<br/>[meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-1.0)<br/>[meetingTimeSuggestionsResult](/graph/api/resources/meetingtimesuggestionsresult?view=graph-rest-1.0)<br/>[timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-1.0)<br/>[timeSlot](/graph/api/resources/timeslot?view=graph-rest-1.0) |
| Изменение          | 1.0        | Сложный тип [attendee](/graph/api/resources/attendee?view=graph-rest-1.0) теперь является производным от attendeeBase, который, в свою очередь, является производным от [recipient](/graph/api/resources/recipient?view=graph-rest-1.0). Он состоит из тех же свойств **status**, **type** и **emailAddress**, что и раньше, а также унаследованных свойств. |
| Дополнение        | Бета        | В ресурс [calendar](/graph/api/resources/calendar?view=graph-rest-beta) добавлено свойство hexColor. |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлены новые объекты: <br/>[appReportingOverviewStatus](/graph/api/resources/intune-apps-appreportingoverviewstatus?view=graph-rest-beta)<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta)<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta)<br/>[deviceManagementExchangeOnpremisesPolicy](/graph/api/resources/intune-onboarding-devicemanagementexchangeonpremisespolicy?view=graph-rest-beta)<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)<br/>[onpremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-beta)<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta)<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-beta)<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)<br/>[windows10WindowsInformationProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10windowsinformationprotectionconfiguration?view=graph-rest-beta) |
|Дополнение|бета|Добавлены новые сложные типы: <br/> [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta)<br/>[enterpriseCloudResource](/graph/api/resources/intune-deviceconfig-enterprisecloudresource?view=graph-rest-beta)<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-beta)<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-beta)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-beta)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-beta)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-beta)<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta)<br/>[iPv6Range](/graph/api/resources/intune-deviceconfig-ipv6range?view=graph-rest-beta)<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRule](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprule?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruleapplockerpolicyfiletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruledesktoptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprulestoreapptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionCorporateNetworkLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectioncorporatenetworklocation?view=graph-rest-beta)<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocation?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisecloudresources?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv4ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv6ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationneutralresources?view=graph-rest-beta)
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
|Изменение|бета|Добавлена коллекция [notificationMessageTemplates](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta) к одиночному объекту [deviceManagement](/graph/api/resources/intune-deviceconfig-devicemanagement?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **isDefault**, **lastModifiedDateTime**, **locale**, **messageTemplate** и **subject** к объекту [localizedNotificationMessage](/graph/api/resources/intune-deviceconfig-localizednotificationmessage?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **azureActiveDirectoryDeviceId**, **deviceCategory**, **deviceRegistrationState** и **managementAgent** к объекту [managedDevice](/graph/api/resources/intune-onboarding-manageddevice?view=graph-rest-beta).|
|Изменение|Бета|Добавлено свойство **lastModifiedDateTime** к объекту [mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **brandingOptions**, **defaultLocale**, **displayName**, **fromEmailAddress**, **lastModifiedDateTime**, **localizedNotificationMessages** к объекту [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta).|
|Изменение|Бета|Добавлены свойства **appsAllowTrustedAppsSideloading**, **appsBlockWindowsStoreOriginatedApps**, **developerUnlockSetting**, **edgeBlockAccessToAboutFlags**, **edgeBlockDeveloperTools**, **edgeBlockExtensions**, **edgeBlockInPrivateBrowsing**, **edgeFirstRunUrl**, **edgeHomepageUrls**, **gameDvrBlocked**, **settingsBlockAddProvisioningPackage**, **settingsBlockChangeLanguage**, **settingsBlockChangePowerSleep**, **settingsBlockChangeRegion**, **settingsBlockChangeSystemTime**, **settingsBlockEditDeviceName**, **settingsBlockRemoveProvisioningPackage**, **sharedUserAppDataAllowed**, **smartScreenBlockPromptOverride**, **smartScreenBlockPromptOverrideForFiles**, **storageRestrictAppDataToSystemVolume**, **storageRestrictAppInstallToSystemVolume**, **webRtcBlockLocalhostIpAddress**, **windowsStoreBlockAutoUpdate** и **windowsStoreEnablePrivateStoreOnly** к объекту [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|

## <a name="december-2016"></a>Декабрь 2016 г.

### <a name="track-changes"></a>Отслеживание изменений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | В следующие объекты добавлена новая функция delta для выполнения [запроса на получение различий](delta-query-overview.md):<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Примеры см. в следующих статьях:<br/>[Получение добавочных изменений групп (предварительная версия)](delta-query-groups.md)<br/>[Получение добавочных изменений сообщений в папке (предварительная версия)](delta-query-messages.md)<br/>[Получение добавочных изменений пользователей (предварительная версия)](delta-query-users.md) |

### <a name="workbooks-and-charts-excel"></a>Книги и диаграммы (Excel)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлены ресурс workbookPivotTable, действия refresh и refreshAll в сводных таблицах, ресурс workbookRangeView, действие visibleView в отфильтрованном диапазоне для возврата workbookRangeView пользователю, коллекция строк get и ресурс range из visibleView, функции columnsAfter, columnsBefore, resizedRange, rowsAbove и rowsBelow из ресурса range и новые свойства таблицы. |

### <a name="devices-and-apps-microsoft-intune"></a>Устройства и приложения (Microsoft Intune)

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

### <a name="identity-and-access--invitation-manager"></a>Удостоверение и доступ | Диспетчер приглашений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство invitedUserType к типу объекта приглашений, определяющее тип приглашаемого пользователя (**Guest** или **Member**). |
| Удаление        | Бета        | Мы удалим свойство invitedToGroups для типа объекта invitation 11 ноября 2016 г. Это значит, что вы больше не сможете добавить приглашаемого пользователя в группу с помощью этого API. Это можно будет сделать с помощью [API добавления членов](/graph/api/group-post-members?view=graph-rest-1.0). |

## <a name="september-2016"></a>Сентябрь 2016 г.

### <a name="identity-and-access--application"></a>Удостоверение и доступ | Приложение

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Теперь API Azure AD Application Proxy доступны в конечной точке Microsoft Graph бета-версии. Эти API позволяют безопасно публиковать локальные приложения для пользователей, находящихся за пределами корпоративной сети, используя Azure AD в качестве общей системы управления доступом. Опубликованные API позволяют создавать приложения, которые могут получать и обновлять различные аспекты прокси приложения, например параметры _connectors_, _connectorGroups_ и _onPremisesPublishing_ приложения. |

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена коллекция _shared_, благодаря которой можно получать доступ к общим элементам driveItem с помощью идентификатора shareId или URL-адреса для совместного доступа. |
| Дополнение        | Бета-версия        | Добавлена функция _search_ к объекту drive, которая позволяет искать элементы не только в корневой папке диска. |


### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлена поддержка элемента _createUploadSession_, который позволяет отправлять файлы размером более 4 МБ в OneDrive, OneDrive для бизнеса и библиотеки документов SharePoint. |
| Дополнение        | Бета-версия        | Добавлено свойство _sharepointIds_, которое возвращает традиционные идентификаторы API SharePoint для элементов driveItem, хранящихся в SharePoint. |
| Дополнение        | Бета-версия        | Добавлены дополнительные свойства для _remoteItem_. |
| Дополнение        | Бета        | Добавлено значение _quickXorHash_ для файлов в OneDrive для бизнеса. |
| Дополнение        | Бета-версия        | Добавлена область для объекта _createSharingLink_, которая позволяет создавать ссылки для совместного доступа в компании или анонимного совместного доступа. |

### <a name="calendar-groups-mail-personal-contacts"></a>Календарь, группы, почта, личные контакты

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

### <a name="hybrid-deployment"></a>Гибридное развертывание

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Приложения могут использовать API Почты, Календаря и Контактов Outlook версии 1.0 для доступа к локальным почтовым ящикам в гибридном развертывании Exchange 2016 с накопительным пакетом обновления 3 (CU3). Дополнительные сведения о поддержке REST API см. в разделах, посвященных соответствующему [гибридному развертыванию](hybrid-rest-support.md). **Примечание.** Если вы используете эти наборы API версии 1.0, то теперь ваши приложения (включая рабочие) будут работать с локальными почтовыми ящиками, которые соответствуют требованиям для гибридных развертываний. Доступна только предварительная версия этой возможности. |

### <a name="identity-and-access--identity-protection"></a>Удостоверение и доступ | Защита удостоверений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | В рамках изменения схемы, при котором тип двух свойств расположений будет заменен новым сложным типом в конечной точке identityRiskEvents, в конечной точке identityRiskEvents изменены или добавлены следующие свойства:</br>**location** теперь относится не к Edm.String, а к signInLocation ComplexType;<br/>**previousLocation** теперь относится не к Edm.String, а к signInLocation ComplexType;<br/>**signInLocation** — новый элемент ComplexType, содержащий свойства city, state, countryOrRegion и geoCoordinates;<br/>**geoCoordinates** — новый элемент ComplexType, содержащий свойства latitude и longitude. |

### <a name="identity-and-access--invitation-manager"></a>Удостоверение и доступ | Диспетчер приглашений

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Теперь API диспетчера приглашений доступны в конечной точке Microsoft Graph бета-версии. С помощью API диспетчера приглашений вы можете создать приглашение для добавления внешнего пользователя в организацию. Кроме того, при приглашении пользователя вы можете добавить его в группу Office 365. Дополнительные сведения см. в статье [о диспетчере приглашений](/graph/api/resources/invitation?view=graph-rest-beta). |

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен метод **CreateUploadSession** для **driveItem**, который позволяет отправлять большие файлы и возобновлять отправку. |
| Дополнение        | 1.0        | Добавлены свойства для отслеживания идентификаторов SharePoint в элементах из SharePoint (**sharepointIds**) и свойство для идентификации корневых папок (**root**). |
| Дополнение        | 1.0        | Добавлена корневая коллекция **Shares**, которую можно использовать с идентификаторами shareId или ссылками для совместного доступа к общим элементам в OneDrive и SharePoint. Возвращает новый тип — sharedDriveItem. |
| Дополнение        | 1.0        | Добавлен метод **Invite** для driveItem, который позволяет добавлять разрешения для элементов. |
| Дополнение        | 1.0        | Добавлен метод **Search** для drive, который позволяет искать элементы на диске, а также общие элементы. |
| Дополнение        | 1.0        | Добавлено свойство **processingMetadata** для свойства quickXorHash сложного типа hashes. |
| Дополнение        | 1.0        | Добавлено свойство **quickXorHash** к сложному типу hashes. |

### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлено свойство **onlineMeetingUrl** к ресурсу [event](/graph/api/resources/event?view=graph-rest-1.0). |
| Дополнение        | Бета-версия        | Добавлено действие [forward](/graph/api/event-forward?view=graph-rest-beta) к ресурсу event. |
| Дополнение        | Бета-версия        | К ресурсу [calendar](/graph/api/resources/calendar?view=graph-rest-beta) добавлены свойства, c помощью которых можно предоставлять общий доступ к календарю: **canEdit**, **canShare**, **canViewPrivateItems**, **isShared**, **isShareWithMe** и **owner**. |

### <a name="change-notifications-webhooks"></a>Уведомления об изменениях (веб-перехватчики)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | В веб-перехватчики добавлены корневые элементы Drive в качестве ресурса, доступного для подписки. |

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлена возможность создавать, отображать, получать и удалять один или несколько экземпляров объекта [mention](/graph/api/resources/mention?view=graph-rest-beta) в сообщении. С помощью объектов mention можно привлечь внимание других пользователей в сообщении. |
| Дополнение        | Бета-версия        | Добавлена поддержка действия [getMailTips](/graph/api/user-getmailtips?view=graph-rest-beta) для получения подсказок для определенных получателей. Добавлены следующие ресурсы: [automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-beta), [mailTips](/graph/api/resources/mailtips?view=graph-rest-beta), [mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-beta). |

### <a name="query-parameters"></a>Параметры запроса

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | С 26 сентября 2016 г. поддерживаются параметры запроса без префиксов $. Префикс $ в параметрах запроса не является обязательным. Дополнительные сведения см. в записи блога [Поддержка параметров запросов без префиксов $ в Microsoft Graph](https://dev.office.com/queryparametersinMicrosoftGraph). |

### <a name="sites-and-lists-sharepoint"></a>Сайты и списки (SharePoint)

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

### <a name="users--outlook-settings"></a>Пользователи | Параметры Outlook

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен сложный тип [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0), который включает свойства **automaticRepliesSetting**, **timeZone** и **language**. |
| Дополнение        | 1.0        | Добавлено свойство **mailboxSettings** к ресурсу [user](/graph/api/resources/user?view=graph-rest-1.0). |


## <a name="august-2016"></a>Август 2016 г.

### <a name="personal-contacts-outlook"></a>Личные контакты (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | В рамках изменения схемы, при котором удаляются несколько свойств и добавляются соответствующие коллекции в конечную точку contacts, в эту конечную точку добавлены следующие свойства: _Websites Collection(ComplexType: Website)_,_Phones Collection (ComplexType: Phone)_, _PostalAddress Collection(ComplexType: PhysicalAddress)_. Дополнительные сведения см. в записи блога [Предстоящие изменения API Контактов и Людей](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/). |
| Удаление        | Бета        | В рамках изменения схемы, при котором удаляются несколько свойств и добавляются соответствующие коллекции в конечную точку contacts, из этой конечной точки удалены следующие свойства: _BusinessHomePage_,_HomePhones_, _MobilePhone1_, _BusinessPhones_, _HomeAddress_, _BusinessAddress_, _OtherAddress_. Дополнительные сведения см. в записи блога [Предстоящие изменения API Контактов и Людей](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/). |

### <a name="workbooks-and-charts-excel"></a>Книги и диаграммы (Excel)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | REST API Excel стал общедоступным в Microsoft Graph. Теперь вы можете обеспечить глубокую и сложную интеграцию с книгами Excel в Office 365. Дополнительные сведения см. в записи блога [Настройка использования REST API для Excel в приложениях с помощью Microsoft Graph](https://developer.microsoft.com/office/blogs/power-your-apps-with-the-new-excel-rest-api/). |

### <a name="social-and-workplace-intelligence--people"></a>Социальная и рабочая аналитика | Пользователи

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Изменение          | Бета        | Свойство _WebSite_ переименовано на _Websites_. Дополнительные сведения см. в записи [Предстоящие изменения API Контактов и Людей](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/). |

### <a name="identity-and-access--privileged-identity-management"></a>Удостоверение и доступ | Управление привилегированными пользователями (PIM)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Теперь REST API управления привилегированными пользователями доступны в конечной точке Microsoft Graph (бета-версия). [Управление привилегированными пользователями](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) обеспечивает активацию "точно в срок" для привилегированных ролей в организации Azure AD, например ролей глобального администратора, администратора выставления счетов и т. д. C помощью опубликованных API разработчики могут создавать приложения, которые получают и обновляют привилегированные роли и активируют роли для пользователей. Дополнительные сведения см. в статьях [Microsoft Graph: доступна бета-версия API для Azure AD Privileged Identity Management](https://developer.microsoft.com/office/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta/) и [Azure AD Privileged Identity Management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta). |

## <a name="july-2016"></a>Июль 2016 г.

### <a name="identity-and-access--administrative-unit"></a>Удостоверение и доступ | Административная единица

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Представлен новый API Administrative Units (предварительная версия). Административные единицы позволяют организациям делить Azure Active Directory на подразделения и делегировать административные обязанности этим подразделениям. Подразделения могут представлять регионы, отделы, места возникновения затрат и т. д. Теперь ими можно управлять с помощью API Microsoft Graph. |

## <a name="june-2016"></a>Июнь 2016 г.

### <a name="identity-and-access--identity-protection"></a>Удостоверение и доступ | Защита удостоверений

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Дополнение|Бета|Представлен новый API IdentityRiskEvents (предварительная версия). Этот API работает в сочетании с защитой идентификации Azure Active Directory. Его можно использовать для запрашивания событий рисков, созданных функцией защиты идентификации. Дополнительные сведения см. в статье [Знакомство с предварительной версией нового API в Microsoft Graph: IdentityRiskEvents](https://developer.microsoft.com/office/blogs/identityriskevents-api-preview/).

### <a name="change-notifications-webhooks"></a>Уведомления об изменениях (веб-перехватчики)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Области, предназначенные только для приложений, теперь поддерживаются для подписок _mail_ и _contacts_. |

## <a name="may-2016"></a>Май 2016 г.

### <a name="calendar-outlook"></a>Календарь (Outlook)

|**Тип изменения**|**Версия**|**Описание**|
|:--------------|:-----------|:--------------|
|Существенные изменения|Бета|Изменения в API findMeetingTimes. Дополнительные сведения см. в записи блога [Обновление API findMeetingTimes в Microsoft Graph](https://dev.office.com/microsoft-graph-findmeetingtimes-api-update). Это изменение вступило в силу 19 мая 2016 г.

### <a name="personal-contact-outlook"></a>Личный контакт (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен абстрактный тип _extensions_ для поддержки открытого типа openTypeExtension в OData версии 4. |

### <a name="identity-and-access--directory-setting"></a>Удостоверение и доступ | Параметры каталога

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Существенные изменения | Бета        | Свойство _settingTemplateId_ теперь называется _templateId_. Это изменение вступило в силу 19 мая 2016 г. |

### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен абстрактный тип _extensions_ для объекта **event** с целью поддержки открытого типа openTypeExtension в OData версии 4. |
| Дополнение        | 1.0        | Добавлены типы _inferenceClassification_ и _extensions_ к объекту **eventMessage**. |
| Дополнение        | бета        | Добавлено свойство _responseRequested_ к объекту **eventMessageRequest**. |

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлены типы _inferenceClassification_ и _extensions_ к объекту **message**. |

### <a name="personal-contacts-outlook"></a>Личные контакты (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлено свойство _wellknownname_ для объекта **contactFolder**. |

### <a name="groups"></a>Группы

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | Добавлен абстрактный тип _extensions_ для объекта **post** с целью поддержки открытого типа openTypeExtension в OData версии 4. |

### <a name="users"></a>Пользователи

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
| Дополнение        | 1.0          | Добавлена поддержка сегмента приведения в пути expand. Например: "https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event" |
| Дополнение        | Бета          | Добавлена поддержка запроса PATCH для структурных свойств. Например: "PATCH /me/mailboxSettings" |
| Дополнение        | Бета          | Теперь Azure Active Directory используется в качестве резервного ресурса для запросов /beta/users/id/photo, когда приложению Outlook не удается обслужить запрос (например, когда у пользователя нет лицензии на почтовый ящик или у клиента нет подписки на Exchange Online). ПРИМЕЧАНИЕ. Этот резервный ресурс доступен и для запросов GET, и для запросов PATCH. |
| Дополнение        | бета          | Добавлена поддержка сегмента приведения в пути expand. Например: "https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event" |

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Исправление             | 1.0        | Устранена неисправность, из-за которой при выполнении запросов createLink в OneDrive возникала ошибка 500: "Неподдерживаемый тип свойства расширения". |

## <a name="march-2016"></a>Март 2016 г.

### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_. |
| Дополнение        | Бета-версия        | Добавлено свойство _suggestionHint_ к _meetingTimeCandidate_. |
| Дополнение        | Бета-версия        | Добавлено свойство _locationUri_ к _location_. |
| Дополнение        | Бета-версия        | Добавлены свойства _type_ и _postOfficeBox_ к _physicalAddress_. |
| Изменение          | Бета-версия        | У метода _findMeetingTimes_ появился новый параметр _ReturnSuggestionHints_. |
| Изменение          | Бета-версия        | Метод _findMeetingTimes_ теперь возвращает коллекцию объектов _meetingTimeCandidate_. |

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлена функция _recent_ для вывода списка элементов, которые недавно использовал пользователь, вошедший в систему. Этот список включает элементы, находящиеся на диске пользователя, а также элементы на других дисках, к которым у пользователя есть доступ. Пример: GET /me/drive/recent. |
| Дополнение        | 1.0 и бета-версия | Добавлена функция _sharedWithMe_ для вывода списка элементов, доступ к которым предоставлен текущему пользователю. Пример: GET /me/drive/sharedWithMe. |

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлен тип _remoteItem_, который позволяет предоставить ссылку на элемент на другом диске. |
| Дополнение        | 1.0 и бета-версия | Добавлен тип _sharingInvitation_, который позволяет предоставить сведения о приглашении к совместному использованию, связанном с этим разрешением. |
| Дополнение        | 1.0 и бета-версия | Добавлена функция _delta_, чтобы отслеживать изменения элементов на диске. Пример: GET /me/drive/items/{item-id}/delta |
| Дополнение        | 1.0 и бета-версия | Добавлен метод _copy_, который создает копию _driveItem_ (в том числе всех дочерних элементов) в новом родительском элементе или с новым именем. Пример: POST /me/drive/items/{item-id}/copy |
| Дополнение        | 1.0 и бета-версия | Атрибуты экземпляра _conflictBehavior_ теперь можно применять к _driveItem_. |
|Дополнение|Бета|Добавлена функция _invite_, которая позволяет отправить приглашение к совместному использованию для существующего элемента. Приглашение к совместному использованию создает уникальную ссылку для совместного доступа и отправляет ее получателю приглашения. Пример: POST /drive/items/{item-id}/invite

### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | бета        | Добавлены новое свойство _onlineMeetingUrl_ и новый метод _cancel_ к объекту **event**. |
| Дополнение        | бета        | Добавлены свойства _startDateTime_, _endDateTime_, _location_, _type_, _recurrence_, _isOutOfDate_, _conversationIndex_, _unsubscribe_, _unsubscribeData_, _unsubscribeEnabled_ и _flag_ к объекту **eventmessage**. |
| Дополнение        | бета        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_ к объекту **eventMessage**. |
| Дополнение        | бета        | Добавлен новый метод _unsubscribe_ к объекту **eventMessage**.|

### <a name="workbooks-and-charts-excel"></a>Книги и диаграммы (Excel)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Мы добавляем новые REST API Excel, которые позволяют считывать и изменять данные в рабочей книге Excel. Теперь вы можете создавать интеллектуальные приложения, с помощью которых пользователи смогут эффективно анализировать содержимое, хранящееся в рабочих книгах Excel. Используйте аналитические функции Excel, создавайте таблицы и визуально привлекательные диаграммы в своем приложении. Дополнительные сведения см. в статье [Работа с Excel в Microsoft Graph](/graph/api/resources/excel?view=graph-rest-beta). |

### <a name="general"></a>Общие

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета | Улучшено сообщение об ошибке при сопоставлении псевдонима клиента и отклоненных токенов JWT (AAD). |
| Дополнение        | 1.0 и бета | Сведения о расположении конечной точки службы авторизации теперь возвращаются в заголовке _www-authenticate_ при получении запроса с пустым токеном носителя. |
| Дополнение        | 1.0 и бета-версия | Исправлена возможность фильтрации по свойству id объекта. Пример: GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>Ранее в запросах POST требовалось добавлять microsoft.graph перед именем функции или действия. Например: POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups.<br/>Теперь не требуется указывать префикс (хотя его по-прежнему можно указывать). Таким образом, указанный ниже запрос также будет работать. POST https://graph.microsoft.com/v1.0/me/getMemberGroups |
| Изменение          | Бета          | Удалены имена свойств подписок.  |
| Дополнение        | бета          | Мы добавили возможность находить (с помощью _directorySettingTemplates_) и переопределять поведение по умолчанию (путем создания _setting_ на основе шаблона) для объектов и связанных с ними функций. Изначально для управления поведением групп Office использовался только этот шаблон. |

### <a name="mail-outlook"></a>Почта (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены свойства _wellKnownName_ и _userConfigurations_ к объекту **mailFolder**. |
| Дополнение        | бета        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_ к объекту **mailFolder**. |
| Дополнение        | 1.0          | Добавлено свойство _mobilePhone_ для объекта **message**.            |
| Дополнение        | 1.0 и бета-версия | Добавлено свойство _internetMessageId_ для объекта **message**. Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). |
| Изменение          | Бета-версия          | Свойство _mobilePhone1_ теперь называется _mobilePhone_ в объекте **message**. |
| Изменение          | Бета-версия          | У методов _createReply_ и _createReplyAll_ объекта **message** появились новый параметры — _message_ и _comment_. |
| Изменение          | бета          | У метода _createForward_ объекта **message** появились новые параметры _Message_, _ToRecipients_ и _comment_. |
| Изменение          | Бета-версия          | У методов _reply_, _replyAll_ и _forward_ объекта **message** появился новый параметр — _Message_. |

### <a name="permission"></a>Разрешение

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Добавлено свойство _sharingInvitation_ для предоставления сведений о приглашении к совместному использованию, связанном с этим разрешением. |

### <a name="social-and-workplace-intelligence--people"></a>Социальная и рабочая аналитика | Пользователи

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлены новые свойства: _birthday_, _personNotes_, _isFavorite_, _phones_, _permission_, _postalAddresses_, _websites_, _yomiCompany_, _department_, _profession_, _mailboxType_ и _personType_. |
| Дополнение        | Бета-версия        | Добавлены новые типы перечислений: _physicalAddressType_, _webSite_, _phone_ и _webSiteType_. |

### <a name="calendar-group-mail-to-do-tasks"></a>Календарь, группа, почта, задачи To-Do

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | К объекту **referenceAttachment** добавлены новые свойства: _sourceUrl_, _providerType_, _thumbnailUrl_, _previewUrl_, _permission_ и _isFolder_. (Справочные сведеления о вложениях поддерживаются в **event**, **message**, **outlookTask** или **post**.)  |
| Дополнение        | Бета-версия        | Добавлены свойства _singleValueExtendedProperties_ и _multiValueExtendedProperties_ к объекту **referenceAttachment**. |
| Дополнение        | Бета-версия        | Добавлены новые типы перечислений — _referenceAttachmentProvider_ и _referenceAttachmentPermission_. |

### <a name="change-notifications-webhooks"></a>Уведомления об изменениях (веб-перехватчики)

| **Тип изменения** | **Конечная точка** | **Описание**                          |
| :-------------- | :----------- | :--------------------------------------- |
| Дополнение        | 1.0         | Веб-перехватчики теперь доступны для ресурса _/Subscriptions_ в конечной точке версии 1.0. Создавайте, просматривайте, продлевайте и удаляйте подписки на уведомления о данных из чатов в Outlook и группах Office 365. |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | Добавлено свойство _mailboxSettings_ и соответствующие типы. |

## <a name="february-2016"></a>Февраль 2016 г.

### <a name="files-onedrive-for-business"></a>Файлы (OneDrive для бизнеса)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Дополнение        | 1.0 и бета-версия | Новое свойство _remoteItem_ для driveItem для учетных записей Майкрософт. |

### <a name="general"></a>Общие

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Конструкция-_/me/drive_ теперь работает как для учетных записей Майкрософт, так и для рабочих и учебных учетных записей. |
| Изменение          | 1.0 и бета-версия | Запросы Drive для учетных записей, хранилища OneDrive которых подготовлены по запросу, работают более надежно и в большем количестве сценариев, где для используемых по умолчанию сайтов SharePoint клиента применяются нестандартные имена. |
| Удаление        | Бета          | Из бета-версии схемы удалены различные нереализованные типы для более точного соответствия схеме версии 1.0. |

### <a name="change-notifications-webhooks"></a>Уведомления об изменениях (веб-перехватчики)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета        | Проверка notificationUrl на создание подписок. Дополнительные сведения см. в статье [Обновление веб-перехватчиков Microsoft Graph — январь 2016 г.](https://developer.microsoft.com/office/blogs/Microsoft-Graph-WebHooks-Update-January-2016/) |
| Дополнение        | Бета-версия        | Теперь можно удалять объекты подписки. Соответствующий запрос: DELETE https://graph.microsoft.com/beta/subscriptions/. |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Изменение          | 1.0 и бета-версия | Теперь для учетных записей Майкрософт возвращается _displayName_. |

## <a name="january-2016"></a>Январь 2016 г.

### <a name="personal-contacts-outlook"></a>Личные контакты (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | 1.0        | В набор объектов личных контактов добавлено свойство mobilePhone. |

### <a name="identity-and-access-directory"></a>Удостоверение и доступ (каталог)

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Исправление             | 1.0 и бета-версия | Исправлены действия вызовов, привязанные к directoryObjects, при которых возникали сбои со следующим сообщением об ошибке:  Тип значения, возвращаемого в результате операции, невозможен для заданного набора объектов. Это относится к следующим действиям: _microsoft.graph.checkMemberObjects_, _microsoft.graph.getMemberObjects_, _microsoft.graph.checkMemberGroups_, _microsoft.graph.assignLicense_, _microsoft.graph.changePassword_. |

## <a name="december-2015"></a>Декабрь 2015 г.

### <a name="personal-contacts-outlook"></a>Личные контакты (Outlook)

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

### <a name="calendar-outlook"></a>Календарь (Outlook)

| **Тип изменения** | **Версия** | **Описание**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Дополнение        | Бета-версия        | К типу eventMessage добавлен подтип для свойств eventMessageRequest eventMessage, startDateTime, endDateTime, location, type, recurrence и isOutOfDate. |

### <a name="users"></a>Пользователи

| **Тип изменения** | **Версия**   | **Описание**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Исправление             | 1.0 и бета-версия | Устранена возможность выбирать определенные свойства других пользователей, когда на них ссылаются по их основному имени участника-пользователя. Например: https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe |
| Исправление             | 1.0 и бета-версия | Исправлен вызов функции _microsoft.graph.reminderView_, привязанной к пользователю, при котором возникал сбой и отображалось следующее сообщение об ошибке: "Не удалось найти свойство с именем businessPhones в типе Microsoft.OutlookServices.Reminder". |
| Исправление             | 1.0 и бета-версия | Устранена проблема, из-за которой при создании и обновлении пользователей (POST/PATCH /v1.0/users) возникала ошибка 400. |
