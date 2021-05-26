---
title: Тип ресурса deviceManagement
description: 'Ресурс deviceManagement представляет контейнер, содержимое которого зависит от рабочего процесса, в том числе:  '
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1423a165bb66e89dbb67b40aa97c2d1dddb395b7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665569"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс deviceManagement представляет контейнер, содержимое которого зависит от рабочего процесса, в том числе:  

- Параметры Android for Work
- События аудита
- Корпоративные условия 
- Профили корпоративных регистраций
- Параметры конфигурации устройства
- Параметры намерения устройства
- Управление устройствами
- Электронная SIM-карта (ESIM)
- Фехтования
- Аналитика групповой политики
- Уведомления
- Политики, параметры и подробные сведения
- Набор политик
- Политика доступа к ресурсам
- Удаленный доступ
- Партнеры удаленной помощи
- Политики управления доступом на основе ролей (RBAC)
- Отчётность
- Партнеры по управлению телекоммуникационными ресурсами
- События устранения неполадок
- Windows Сводки по защите информации

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
|[функция getRoleScopeTagsByIds](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|[Коллекция roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Пока не задокументировано.|
|[функция getRoleScopeTagsByResource](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|[Коллекция roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Н/Д|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор, связанный с устройством.|
|**Конфигурация устройств**|
|intuneAccountId|Guid|ID учетной записи Intune для данного клиента|
|legacyPcManangementEnabled|Логический|Свойство, чтобы включить для этой учетной записи управление устаревшим КОМПЬЮТЕРом без MDM. Это свойство доступно только для чтения.|
|maximumDepTokens|Int32|Максимальное количество маркеров DEP, разрешенных для каждого клиента.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Параметры уровня учетной записи.|
|**Управление устройствами**|
|accountMoveCompletionDateTime|DateTimeOffset|Дата &, когда данные клиента перемещаются между scaleunits.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Сведения о согласии администратора.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);|Обзор защиты устройств.|
|managedDeviceCleanupSettings;|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);|Правило очистки устройств|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Состояние подписки на управление мобильными устройствами для клиента. Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|subscriptions|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Подписка клиента. Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Обзор вредоносных программ для устройств Windows.|
|**Аналитика групповой политики**|
|groupPolicyObjectFiles|[коллекция groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Список загруженных файлов объектов групповой политики.|
|**Адаптация**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.|
|**Odj**|
|domainJoinConnectors|[коллекция deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Список объектов соединитений.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android для работы**|
|androidDeviceOwnerEnrollmentProfiles|[коллекция androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Сущностями профилей владельцев android-устройств.|
|androidForWorkAppConfigurationSchemas|Коллекция [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Сущности схемы конфигурации в приложении Android for Work.|
|androidForWorkEnrollmentProfiles|Коллекция [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Сущности профиля регистрации Android for Work.|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Одноэлементная сущность параметров Android for Work.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Объект корпоративных параметров учетной записи единой учетной записи Android с управляемым управлением.|
|AndroidManagedStoreAppConfigurationSchemas|[коллекция androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Android Enterprise сущностями конфигурации приложений.|
|**Аудит**|
|auditEvents|Коллекция [auditEvent](../resources/intune-auditing-auditevent.md)|События аудита|
|**Условия компании**|
|termsAndConditions|Коллекция [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Условия, связанные с управлением устройствами в компании.|
|**Корпоративная регистрация**|
|enrollmentProfiles|[коллекция enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Профили регистрации.|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity collection](../resources/intune-enrollment-importedappledeviceidentity.md)|Импортируемые удостоверения устройств Apple.|
|importedDeviceIdentities|[importedDeviceIdentity collection](../resources/intune-enrollment-importeddeviceidentity.md)|Идентификаторы импортируемых устройств.|
|**Конфигурация устройств**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Сводное состояние состояния onboarding ATP для этой учетной записи.|
|cartToClassAssociations|[коллекция cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Ассоциации корзины к классу.|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|Политики соответствия устройств требованиям.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Общие сведения о состоянии соответствия устройств требованиям для этой учетной записи.|
|deviceCompliancePolicySettingStateSummaries|Коллекция [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Общие сведения о состоянии параметров политики соответствия требованиям для этой учетной записи.|
|deviceConfigurationConflictSummary|[коллекция deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Сводка политик в состоянии конфликта для этой учетной записи.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Общие сведения о состоянии конфигурации устройства для этой учетной записи.|
|deviceConfigurationRestrictedAppsViolations|[коллекция restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Ограничение нарушений приложений для этой учетной записи.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|Конфигурации устройств.|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md);|Сводка состояния состояния конфигурации устройства для этой учетной записи.|
|iosUpdateStatuses|Коллекция [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Состояния установки обновления программного обеспечения IOS для этой учетной записи.|
|ndesConnectors|[Коллекция ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Коллекция соединители Ndes для этой учетной записи.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Общие сведения о состоянии обновления программного обеспечения.|
|**Намерение устройства**|
|намерения|[коллекция deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Намерения управления устройствами|
|settingDefinitions|[коллекция deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Определения параметров настройки умысла управления устройствами|
|шаблоны|[коллекция deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Доступные шаблоны|
|categories|[коллекция deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Доступные категории|
|**Управление устройствами**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Сертификат push-уведомлений Apple|
|dataSharingConsents|[коллекция dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Согласие на общий доступ к данным.|
|detectedApps|Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)|Список обнаруженных приложений, связанных с устройством.|
|deviceManagementScripts|[коллекция deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Список сценариев управления устройствами, связанных с клиентом.|
|deviceShellScripts|[коллекция deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Список сценариев оболочки устройств, связанных с клиентом.|
|deviceHealthScripts|[коллекция deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Список скриптов для здоровья устройств, связанных с клиентом.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Обзор устройств|
|managedDevices|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Список управляемых устройств.|
|remoteActionAudits|[коллекция remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Список аудитов удаленного действия устройства с клиентом.|
|windowsMalwareInformation|[коллекция windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md)|Список затронутых вредоносных программ в клиенте.|
|mobileAppTroubleshootingEvents|[коллекция mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Свойство коллекции MobileAppTroubleshootingEvent.|
|userExperienceAnalyticsOverview|[userExperienceAnalyticsOverview](../resources/intune-devices-userExperienceAnalyticsOverview.md)|Обзор аналитики пользовательских интерфейсов|
|userExperienceAnalyticsBaselines|[коллекция userExperienceAnalyticsBaseline](../resources/intune-devices-userExperienceAnalyticsBaseline.md)|Базовые показатели аналитики пользовательских интерфейсов|
|UserExperienceAnalyticsCategories|[коллекция userExperienceAnalyticsCategory](../resources/intune-devices-userExperienceAnalyticsCategory.md)|Категории аналитики пользовательских интерфейсов|
|userExperienceAnalyticsDevicePerformance|[коллекция userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userExperienceAnalyticsDevicePerformance.md)|Производительность устройства аналитики пользовательских интерфейсов|
|userExperienceAnalyticsRegressionSummary|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userExperienceAnalyticsRegressionSummary.md)|Сводка регрессии аналитики пользовательских интерфейсов|
|userExperienceAnalyticsDeviceStartupHistory|[коллекция userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userExperienceAnalyticsDeviceStartupHistory.md)|История запуска устройства для аналитики пользовательских интерфейсов|
|userExperienceAnalyticsDeviceStartupProcesses|[коллекция userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userExperienceAnalyticsDeviceStartupProcess.md)|Процессы запуска устройства для аналитики пользовательских интерфейсов|
|userExperienceAnalyticsDeviceStartupProcessPerformance|[коллекция userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userExperienceAnalyticsDeviceStartupProcessPerformance.md)|Производительность процесса запуска устройства для аналитики пользовательских интерфейсов|
|depOnboardingSettings|[коллекция depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Это коллекция нескольких маркеров DEP для каждого клиента.|
|importedDeviceIdentities|[importedDeviceIdentity collection](../resources/intune-enrollment-importeddeviceidentity.md)|Идентификаторы импортируемых устройств.|
|importedWindowsAutopilotDeviceIdentities|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Коллекция импортированных устройств Windows AutoPilot.|
|windowsAutopilotDeploymentProfiles|[коллекция windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Windows автопилот развертывания|
|windowsAutopilotDeviceIdentities|[коллекция windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Идентификаторы Windows автопилота содержали коллекцию.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Параметры Windows автопилота.|
|**Встроенная SIM-карта**|
|embeddedSIMActivationCodePools|[коллекция embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Встроенные пулы кодов активации SIM-карт, созданные этой учетной записью.|
|**Фехтования**|
|managementConditions|[коллекция managementCondition](../resources/intune-fencing-managementcondition.md)|Условия управления, связанные с управлением устройствами компании.|
|managementConditionStatements|[коллекция managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Отчеты об условиях управления, связанные с управлением устройствами компании.|
|**Аналитика групповой политики**|
|groupPolicyMigrationReports|[коллекция groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Список отчетов о миграции групповой политики.|
|**Уведомления**|
|notificationMessageTemplates|Коллекция [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Шаблоны сообщений уведомления.|
|**Адаптация**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Параметры локального условного доступа в Exchange. Для локального условного доступа устройства должны быть зарегистрированы для доступа к почте и поддерживать его.|
|Объекты deviceCategory|Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)|Список категорий устройств в клиенте.|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Список настроек регистрации устройств.|
|Объекты deviceManagementPartner|Коллекция объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Список партнеров по управлению устройствами, настроенных с помощью клиента.|
|Объекты exchangeConnector|Коллекция объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Список соединителей Exchange, настроенных с помощью клиента.|
|exchangeOnPremisesPolicies|[коллекция deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Список политик Exchange Premisis, настроенных клиентом.|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Политика, контролируемая доступом мобильных устройств к Exchange On Premises|
|Объекты mobileThreatDefenseConnector|Коллекция объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Список соединителей Mobile Threat Defense, настроенных с помощью клиента.|
|**Набор политик**|
|deviceManagementScripts|[коллекция deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Список сценариев управления устройствами, связанных с клиентом.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|Список конфигураций устройств, связанных с клиентом.|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|Список политик соответствия требованиям устройств, связанных с клиентом.|
|windowsAutopilotDeploymentProfiles|[коллекция windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Windows автопилот развертывания|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Список настроек регистрации устройств.|
|**Политика доступа к ресурсам**|
|derivedCredentials|[коллекция deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Коллекция параметров производных учетных данных, связанных с учетной записью.|
|**Удаленный доступ**|
|userPfxCertificates|[коллекция userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Коллекция сертификатов PFX, связанных с пользователем.|
|**Удаленная помощь**|
|remoteAssistancePartners|Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Партнеры по удаленной помощи.|
|**Управление доступом на основе ролей (RBAC)**|
|resourceOperations|Коллекция [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Операции с ресурсами.|
|roleAssignments|Коллекция [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Назначения ролей.|
|roleDefinitions|Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)|Определения ролей.|
|roleScopeTags|[Коллекция roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Теги области ролей.|
|**Создание отчетов**|
|отчеты|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Отчеты singleton|
|**Обновление программного обеспечения**|
|windowsFeatureUpdateProfiles|[коллекция windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Коллекция профилей обновления функций Windows|
|**Управление расходами на телеком (TEM)**|
|telecomExpenseManagementPartners|Коллекция [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Партнеры по управлению затратами на телекоммуникации.|
|**Устранение неполадок**|
|troubleshootingEvents|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Список событий устранения неполадок для клиента.|
|**Windows Information Protection**|
|intuneBrandingProfiles|[коллекция intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Профили брендинга Intune, нацеленные на группы AAD|
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




