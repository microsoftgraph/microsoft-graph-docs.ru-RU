---
title: Тип ресурса deviceManagement
description: 'Ресурс deviceManagement представляет контейнер, содержимое которого зависит от рабочего процесса, в том числе:  '
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af2682655d3f5b76e7b99af7ceced20059deb8ff
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154805"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс deviceManagement представляет контейнер, содержимое которого зависит от рабочего процесса, в том числе:  

- Параметры Android for Work
- События аудита
- Корпоративные условия 
- Профили корпоративной регистрации
- Параметры конфигурации устройства
- Параметры намерения устройства
- Управление устройствами
- Электронная SIM-карта (ESIM)
- Скайсинг
- Аналитика групповой политики
- Уведомления
- Политики, параметры и сведения для входящего параметров
- Набор политик
- Политика доступа к ресурсам
- Удаленный доступ
- Партнеры удаленной помощи
- Политики управления доступом на основе ролей (RBAC)
- Отчётность
- Партнеры по управлению телекоммуникационными ресурсами
- Устранение неполадок событий
- Сводки windows Information Protection

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune-shared-devicemanagement-get.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune-shared-devicemanagement-update.md)|Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|**Конфигурация устройств**|
|[Действие enableLegacyPcManagement](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|Нет|Н/Д|
|**Управление устройствами**|
|[Действие sendCustomNotificationToCompanyPortal](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|Нет|Н/Д|
|**Адаптация**|
|[Функция verifyWindowsEnrollmentAutoDiscovery](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolean|Н/Д|
|**Управление доступом на основе ролей (RBAC)**|
|[Функция getEffectivePermissions](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)|Получает действующие разрешения пользователя, прошедшего проверку подлинности|
|[Функция getRoleScopeTagsByIds](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|[Коллекция roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Пока не задокументировано.|
|[Функция getRoleScopeTagsByResource](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|[Коллекция roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Н/Д|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор, связанный с устройством.|
|**Конфигурация устройств**|
|intuneAccountId|Guid|ИД учетной записи Intune для данного клиента|
|legacyPcManangementEnabled|Boolean|Свойство, которое позволяет управлять устаревшими компьютерами, не управляемыми MDM, для этой учетной записи. Это свойство доступно только для чтения.|
|maximumDepTokens|Int32|Максимальное количество маркеров DEP, разрешенных для каждого клиента.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Параметры уровня учетной записи.|
|**Управление устройствами**|
|accountMoveCompletionDateTime|DateTimeOffset|Дата &, когда данные клиента перемещаются между scaleunits.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Сведения о согласии администратора.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);|Обзор защиты устройств.|
|managedDeviceCleanupSettings;|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);|Правило очистки устройства|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Состояние подписки на управление мобильными устройствами для клиента. Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|subscriptions|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Подписка клиента. Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Обзор вредоносных программ для устройств с Windows.|
|**Аналитика групповой политики**|
|groupPolicyObjectFiles|[Коллекция groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Список загруженных файлов объектов групповой политики.|
|**Адаптация**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.|
|**Odj**|
|domainJoinConnectors|[Коллекция deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Список объектов соединитений.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android for Work**|
|androidDeviceOwnerEnrollmentProfiles|[Коллекция androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Объекты профиля регистрации владельца устройства Android.|
|androidForWorkAppConfigurationSchemas|Коллекция [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Сущности схемы конфигурации в приложении Android for Work.|
|androidForWorkEnrollmentProfiles|Коллекция [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Сущности профиля регистрации Android for Work.|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Одноэлементная сущность параметров Android for Work.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Однотонная сущность корпоративных параметров учетной записи управляемого магазина Android.|
|androidManagedStoreAppConfigurationSchemas|[Коллекция androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Объекты схемы конфигурации корпоративных приложений Android.|
|**Аудит**|
|auditEvents|Коллекция [auditEvent](../resources/intune-auditing-auditevent.md)|События аудита|
|**Условия компании**|
|termsAndConditions|Коллекция [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Условия, связанные с управлением устройствами в компании.|
|**Корпоративная регистрация**|
|enrollmentProfiles|[Коллекция enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Профили регистрации.|
|importedAppleDeviceIdentities|[Коллекция importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Импортируемые удостоверения устройств Apple.|
|importedDeviceIdentities|[Коллекция importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Импортируемые удостоверения устройств.|
|**Конфигурация устройств**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Сводное состояние состояния подбора ATP для этой учетной записи.|
|cartToClassAssociations|[Коллекция cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Связи корзины с классом.|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|Политики соответствия устройств требованиям.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Общие сведения о состоянии соответствия устройств требованиям для этой учетной записи.|
|deviceCompliancePolicySettingStateSummaries|Коллекция [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Общие сведения о состоянии параметров политики соответствия требованиям для этой учетной записи.|
|deviceConfigurationConflictSummary|[Коллекция deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Сводка политик в состоянии конфликта для этой учетной записи.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Общие сведения о состоянии конфигурации устройства для этой учетной записи.|
|deviceConfigurationRestrictedAppsViolations|[Коллекция restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Ограничения на использование приложений для этой учетной записи.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|Конфигурации устройств.|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md);|Сводка о состоянии пользователя конфигурации устройства для этой учетной записи.|
|iosUpdateStatuses|Коллекция [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Состояния установки обновления программного обеспечения IOS для этой учетной записи.|
|ndesConnectors|[Коллекция ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Коллекция соединители Ndes для этой учетной записи.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Общие сведения о состоянии обновления программного обеспечения.|
|**Намерение устройства**|
|intents|[Коллекция deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Намерения управления устройствами|
|settingDefinitions|[Коллекция deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Определения параметров намерения управления устройствами|
|templates|[Коллекция deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Доступные шаблоны|
|categories|[Коллекция deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Доступные категории|
|**Управление устройствами**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Сертификат push-уведомлений Apple|
|dataSharingConsents|[Коллекция dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Согласие на общий доступ к данным.|
|detectedApps|Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)|Список обнаруженных приложений, связанных с устройством.|
|deviceManagementScripts|[Коллекция deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Список сценариев управления устройствами, связанных с клиентом.|
|deviceShellScripts|[Коллекция deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Список сценариев оболочки устройства, связанных с клиентом.|
|deviceHealthScripts|[Коллекция deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Список сценариев состояния устройства, связанных с клиентом.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Обзор устройств|
|managedDevices|Коллекция [managedDevice](../resources/intune-shared-manageddevice.md)|Список управляемых устройств.|
|remoteActionAudits|[Коллекция remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Список аудитов удаленных действий устройства с клиентом.|
|windowsMalwareInformation|[Коллекция windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md)|Список затронутых вредоносных программ в клиенте.|
|mobileAppTroubleshootingEvents|[Коллекция mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Свойство коллекции MobileAppTroubleshootingEvent.|
|userExperienceAnalyticsOverview|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Обзор аналитики пользовательского интерфейса|
|userExperienceAnalyticsBaselines|[Коллекция userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Базовые параметры аналитики пользовательского интерфейса|
|userExperienceAnalyticsCategories|[Коллекция userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Категории аналитики пользовательского интерфейса|
|userExperienceAnalyticsDevicePerformance|[Коллекция userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Производительность устройства аналитики пользовательского интерфейса|
|userExperienceAnalyticsRegressionSummary|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Сводка по регрессии аналитики пользовательского интерфейса|
|userExperienceAnalyticsDeviceStartupHistory|[Коллекция userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|История запуска устройства аналитики пользовательского интерфейса|
|userExperienceAnalyticsDeviceStartupProcesses|[Коллекция userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Процессы запуска устройства аналитики пользовательского интерфейса|
|userExperienceAnalyticsDeviceStartupProcessPerformance|[Коллекция userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Производительность процесса запуска устройства аналитики пользовательского интерфейса|
|**Регистрация**|
|depOnboardingSettings|[Коллекция depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Это наборы нескольких маркеров DEP для каждого клиента.|
|importedDeviceIdentities|[Коллекция importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Импортируемые удостоверения устройств.|
|importedWindowsAutopilotDeviceIdentities|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Коллекция импортированных устройств Windows AutoPilot.|
|windowsAutopilotDeploymentProfiles|[Коллекция windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Профили автоматического пилотного развертывания Windows|
|windowsAutopilotDeviceIdentities|[Коллекция windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Идентификаторы устройств Windows Autopilot, содержащие коллекцию.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Параметры учетной записи Windows Autopilot.|
|**Внедренная SIM-карта**|
|embeddedSIMActivationCodePools|[Коллекция embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Пулы кода активации внедренной SIM-карты, созданные этой учетной записью.|
|**Скайсинг**|
|managementConditions|[коллекция managementCondition](../resources/intune-fencing-managementcondition.md)|Условия управления, связанные с управлением устройствами компании.|
|managementConditionStatements|[коллекция managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Условия управления, связанные с управлением устройствами компании.|
|**Аналитика групповой политики**|
|groupPolicyMigrationReports|[Коллекция groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Список отчетов о миграции групповой политики.|
|**Уведомления**|
|notificationMessageTemplates|Коллекция [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Шаблоны сообщений уведомления.|
|**Адаптация**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Параметры локального условного доступа в Exchange. Для локального условного доступа устройства должны быть зарегистрированы для доступа к почте и поддерживать его.|
|Объекты deviceCategory|Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)|Список категорий устройств в клиенте.|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Список настроек регистрации устройств.|
|Объекты deviceManagementPartner|Коллекция объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Список партнеров по управлению устройствами, настроенных с помощью клиента.|
|Объекты exchangeConnector|Коллекция объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Список соединителей Exchange, настроенных с помощью клиента.|
|exchangeOnPremisesPolicies|[Коллекция deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Список политик предварительной настройки Exchange, настроенных клиентом.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Политика, которая контролирует доступ с мобильных устройств к локальной сети Exchange|
|Объекты mobileThreatDefenseConnector|Коллекция объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Список соединителей Mobile Threat Defense, настроенных с помощью клиента.|
|**Набор политик**|
|deviceManagementScripts|[Коллекция deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Список сценариев управления устройствами, связанных с клиентом.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|Список конфигураций устройств, связанных с клиентом.|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|Список политик соответствия устройств требованиям, связанных с клиентом.|
|windowsAutopilotDeploymentProfiles|[Коллекция windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Профили автоматического пилотного развертывания Windows|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Список настроек регистрации устройств.|
|**Политика доступа к ресурсам**|
|derivedCredentials|[Коллекция deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Коллекция параметров производных учетных данных, связанных с учетной записью.|
|**Удаленный доступ**|
|userPfxCertificates|[Коллекция userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Коллекция сертификатов PFX, связанных с пользователем.|
|**Удаленная помощь**|
|remoteAssistancePartners|Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Партнеры по удаленной помощи.|
|**Управление доступом на основе ролей (RBAC)**|
|resourceOperations|Коллекция [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Операции с ресурсами.|
|roleAssignments|Коллекция [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Назначения ролей.|
|roleDefinitions|Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)|Определения ролей.|
|roleScopeTags|[Коллекция roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Теги области роли.|
|**Создание отчетов**|
|reports|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Singleton reports|
|**Обновление программного обеспечения**|
|windowsFeatureUpdateProfiles|[Коллекция windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Коллекция профилей обновления функций Windows|
|**Управление затратами на телекоммуникации (TEM)**|
|telecomExpenseManagementPartners|Коллекция [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Партнеры по управлению затратами на телекоммуникации.|
|**Устранение неполадок**|
|troubleshootingEvents|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Список событий устранения неполадок для клиента.|
|**Windows Information Protection**|
|intuneBrandingProfiles|[Коллекция intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Профили фирменой марки Intune, нацеленные на группы AAD|
|windowsInformationProtectionAppLearningSummaries|Коллекция [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Сводки по обучению Windows Information Protection для приложений.|
|windowsInformationProtectionNetworkLearningSummaries|Коллекция [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Сводки по обучению Windows Information Protection для сетей.|


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```




