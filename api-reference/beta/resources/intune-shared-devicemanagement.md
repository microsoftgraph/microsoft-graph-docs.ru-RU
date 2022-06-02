---
title: Тип ресурса deviceManagement
description: 'Ресурс deviceManagement представляет контейнер, содержимое которого зависит от рабочего процесса, включая:  '
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f07febfdaee04e2baf57f5403cfc07e2de13af10
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858312"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс deviceManagement представляет контейнер, содержимое которого зависит от рабочего процесса, включая:  

- Параметры Android for Work
- События аудита
- Корпоративные условия 
- Профили корпоративной регистрации
- Параметры конфигурации устройства
- Параметры намерения устройства
- Управление устройствами
- Электронная SIM-карта (ESIM)
- Ограждения
- групповая политика Analytics
- Уведомления
- Политики подключения, параметры и сведения
- Набор политик
- Политика доступа к ресурсам
- Удаленный доступ
- Партнеры по удаленной помощи
- Политики управления доступом на основе ролей (RBAC)
- Создание отчетов
- Партнеры по управлению телекоммуникационными ресурсами
- События устранения неполадок
- Windows Information Protection сводки

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
|id|Строка|Уникальный идентификатор, связанный с устройством.|
|**Конфигурация устройств**|
|intuneAccountId|Guid|Intune учетной записи для данного клиента|
|legacyPcManangementEnabled|Boolean|Свойство, которое позволяет включить для этой учетной записи устаревшее управление КОМПЬЮТЕРами, не управляемым MDM. Это свойство доступно только для чтения.|
|maximumDepTokens|Int32|Максимальное число токенов DEP, разрешенных для каждого клиента.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Параметры уровня учетной записи.|
|**Управление устройствами**|
|accountMoveCompletionDateTime|DateTimeOffset|Дата &, когда данные клиента перемещаются между единицами масштабирования.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Администратор согласия.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);|Обзор защиты устройств.|
|managedDeviceCleanupSettings;|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);|Правило очистки устройства|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Состояние подписки на управление мобильными устройствами для клиента. Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|subscriptions|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Подписка клиента. Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Обзор вредоносных программ для устройств Windows.|
|**групповая политика Analytics**|
|groupPolicyObjectFiles|[Коллекция groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Список отправленных групповая политика объектов.|
|**Адаптация**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.|
|**Odj**|
|domainJoinConnectors|[Коллекция deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Список объектов соединителя.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android для работы**|
|androidDeviceOwnerEnrollmentProfiles|[Коллекция androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Android сущностями профиля регистрации владельца устройства.|
|androidForWorkAppConfigurationSchemas|Коллекция [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Сущности схемы конфигурации в приложении Android for Work.|
|androidForWorkEnrollmentProfiles|Коллекция [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Сущности профиля регистрации Android for Work.|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Одноэлементная сущность параметров Android for Work.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Одноэлементная Android сущностей корпоративных параметров управляемой учетной записи хранения.|
|androidManagedStoreAppConfigurationSchemas|[Коллекция androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Android Enterprise сущностями схемы конфигурации приложения.|
|**Аудит**|
|auditEvents|Коллекция [auditEvent](../resources/intune-auditing-auditevent.md)|События аудита|
|**Условия компании**|
|termsAndConditions|Коллекция [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Условия, связанные с управлением устройствами в компании.|
|**Политики конфигурации**|
|configurationPolicies|[Коллекция deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-deviceManagementConfigurationPolicy.md)|Список всех политик конфигурации|
|configurationSettings|[Коллекция deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-deviceManagementConfigurationSettingDefinition.md)|Список всех configurationSettings|
|configurationCategories|[Коллекция deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-deviceManagementConfigurationCategory.md)|Список всех категорий конфигурации|
|**Корпоративная регистрация**|
|enrollmentProfiles|[Коллекция enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Профили регистрации.|
|importedAppleDeviceIdentities|[Коллекция importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Импортированные удостоверения устройств Apple.|
|importedDeviceIdentities|[Коллекция importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Импортированные удостоверения устройств.|
|**Конфигурация устройств**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Сводное состояние состояния подключения ATP для этой учетной записи.|
|CartToClassAssociations|[Коллекция cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Сопоставления корзины и класса.|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|Политики соответствия устройств требованиям.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Общие сведения о состоянии соответствия устройств требованиям для этой учетной записи.|
|deviceCompliancePolicySettingStateSummaries|Коллекция [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Общие сведения о состоянии параметров политики соответствия требованиям для этой учетной записи.|
|deviceConfigurationConflictSummary|[Коллекция deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Сводка политик в состоянии конфликта для этой учетной записи.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Общие сведения о состоянии конфигурации устройства для этой учетной записи.|
|DeviceConfigurationRestrictedAppsViolations|[Коллекция restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Нарушения ограниченного использования приложений для этой учетной записи.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|Конфигурации устройств.|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md);|Сводка состояния пользователя конфигурации устройства для этой учетной записи.|
|iosUpdateStatuses|Коллекция [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Состояния установки обновления программного обеспечения IOS для этой учетной записи.|
|ndesConnectors|[Коллекция ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Коллекция соединителей Ndes для этой учетной записи.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Общие сведения о состоянии обновления программного обеспечения.|
|**Намерение устройства**|
|Намерений|[Коллекция deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Намерения управления устройствами|
|settingDefinitions|[Коллекция deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Определения параметров намерения управления устройствами|
|Шаблоны|[Коллекция deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Доступные шаблоны|
|categories|[Коллекция deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Доступные категории|
|**Управление устройствами**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Сертификат push-уведомлений Apple|
|dataSharingConsents|[Коллекция dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Согласие на общий доступ к данным.|
|detectedApps|Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)|Список обнаруженных приложений, связанных с устройством.|
|DeviceManagementScripts|[Коллекция deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Список сценариев управления устройствами, связанных с клиентом.|
|DeviceShellScripts|[Коллекция deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Список скриптов оболочки устройства, связанных с клиентом.|
|deviceHealthScripts|[Коллекция deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Список скриптов работоспособности устройств, связанных с клиентом.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Обзор устройств|
|managedDevices|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Список управляемых устройств.|
|remoteActionAudits|[Коллекция remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Список аудитов удаленных действий устройства с клиентом.|
|windowsMalwareInformation|[Коллекция windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md)|Список затронутых вредоносных программ в клиенте.|
|mobileAppTroubleshootingEvents|[Коллекция mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Свойство коллекции MobileAppTroubleshootingEvent.|
|userExperienceAnalyticsOverview|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Общие сведения об аналитике пользовательского интерфейса|
|userExperienceAnalyticsBaselines|[Коллекция userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Базовые показатели аналитики пользовательского интерфейса|
|UserExperienceAnalyticsCategories|[Коллекция userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Категории аналитики пользовательского интерфейса|
|userExperienceAnalyticsDevicePerformance|[Коллекция userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Производительность устройства аналитики пользовательского интерфейса|
|userExperienceAnalyticsRegressionSummary|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)|Сводка по регрессии аналитики пользовательского интерфейса|
|userExperienceAnalyticsDeviceStartupHistory|[Коллекция userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Журнал запуска устройства аналитики пользовательского интерфейса|
|userExperienceAnalyticsDeviceStartupProcesses|[Коллекция userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Процессы запуска устройства аналитики пользовательского интерфейса|
|userExperienceAnalyticsDeviceStartupProcessPerformance|[Коллекция userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)|Производительность процесса запуска устройства аналитики пользовательского интерфейса|
|userExperienceAnalyticsScoreHistory|[Коллекция userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Журнал оценки устройства аналитики пользовательского интерфейса|
|**Регистрация**|
|depOnboardingSettings|[Коллекция depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Это коллекции из нескольких токенов DEP для каждого клиента.|
|importedDeviceIdentities|[Коллекция importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Импортированные удостоверения устройств.|
|importedWindowsAutopilotDeviceIdentities|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Коллекция импортированных устройств Windows AutoPilot.|
|windowsAutopilotDeploymentProfiles|[Коллекция windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Windows профилей автоматического пилотного развертывания|
|windowsAutopilotDeviceIdentities|[Коллекция windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|В Windows содержится коллекция удостоверений устройств Autopilot.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Параметры Windows autopilot.|
|**Внедренная SIM-карта**|
|embeddedSIMActivationCodePools|[Коллекция embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Встроенные пулы кода активации SIM-карты, созданные этой учетной записью.|
|**Ограждения**|
|managementConditions|[Коллекция managementCondition](../resources/intune-fencing-managementcondition.md)|Условия управления, связанные с управлением устройствами компании.|
|managementConditionStatements|[Коллекция managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Операторы условий управления, связанные с управлением устройствами компании.|
|**групповая политика Analytics**|
|groupPolicyMigrationReports|[Коллекция groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Список отчетов групповая политика миграции.|
|**MicrosoftTunnel**|
|microsoftTunnelConfigurations|[Коллекция microsoftTunnelConfiguration](../resources/intune-mstunnel-microsoftTunnelConfiguration.md)|Коллекция параметров MicrosoftTunnelConfiguration, связанных с учетной записью.|
|microsoftTunnelSites|[Коллекция microsoftTunnelSite](../resources/intune-mstunnel-microsoftTunnelSite.md)|Коллекция параметров MicrosoftTunnelSite, связанных с учетной записью.|
|**Уведомления**|
|notificationMessageTemplates|Коллекция [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Шаблоны сообщений уведомления.|
|**Адаптация**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Параметры локального условного доступа в Exchange. Для локального условного доступа устройства должны быть зарегистрированы для доступа к почте и поддерживать его.|
|Объекты deviceCategory|Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)|Список категорий устройств в клиенте.|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Список настроек регистрации устройств.|
|Объекты deviceManagementPartner|Коллекция объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Список партнеров по управлению устройствами, настроенных с помощью клиента.|
|Объекты exchangeConnector|Коллекция объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Список соединителей Exchange, настроенных с помощью клиента.|
|exchangeOnPremisesPolicies|[Коллекция deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Список политик Exchange on Premisis, настроенных клиентом.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnpremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Политика, которая управляет доступом мобильных устройств к Exchange локально|
|Объекты mobileThreatDefenseConnector|Коллекция объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Список соединителей Mobile Threat Defense, настроенных с помощью клиента.|
|**Набор политик**|
|DeviceManagementScripts|[Коллекция deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Список сценариев управления устройствами, связанных с клиентом.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|Список конфигураций устройств, связанных с клиентом.|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|Список политик соответствия устройств, связанных с клиентом.|
|windowsAutopilotDeploymentProfiles|[Коллекция windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Windows профилей автоматического пилотного развертывания|
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
|Отчеты|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Одноэлементные отчеты|
|**Обновление программного обеспечения**|
|windowsFeatureUpdateProfiles|[Коллекция windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Коллекция профилей обновления компонентов Windows|
|**Управление затратами на телекоммуникации (TEM)**|
|telecomExpenseManagementPartners|Коллекция [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Партнеры по управлению затратами на телекоммуникации.|
|**Устранение неполадок**|
|troubleshootingEvents|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Список событий устранения неполадок для клиента.|
|**Windows Information Protection**|
|intuneBrandingProfiles|[Коллекция intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Intune фирменной символики, предназначенные для групп AAD|
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



