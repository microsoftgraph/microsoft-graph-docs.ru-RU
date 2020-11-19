---
title: Тип ресурса deviceManagement
description: 'Ресурс deviceManagement представляет контейнер, содержимое которого зависит от рабочего процесса, в том числе:  '
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 95a958bef0550047b7e08cf372cd05b8e9112bca
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300824"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс deviceManagement представляет контейнер, содержимое которого зависит от рабочего процесса, в том числе:  

- Параметры Android for Work
- События аудита
- Корпоративные положения и условия 
- Профили корпоративной регистрации
- Параметры конфигурации устройств
- Параметры намерения устройства
- Управление устройствами
- Электронная SIM-карта (ESIM)
- Ограждение
- Аналитика групповой политики
- Уведомления
- Политики, параметры и сведения о входящей миграции
- Набор политик
- Политика доступа к ресурсам
- Удаленный доступ
- Партнеры удаленного помощника
- Политики управления доступом на основе ролей (RBAC)
- Reporting
- Партнеры по управлению телекоммуникационной експансе
- События устранения неполадок
- Сводки Windows Information Protection

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
|[Функция Жетролескопетагсбидс](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|Коллекция [ролескопетаг](../resources/intune-rbac-rolescopetag.md)|Пока не задокументировано.|
|[Функция Жетролескопетагсбиресаурце](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|Коллекция [ролескопетаг](../resources/intune-rbac-rolescopetag.md)|Н/Д|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор, связанный с устройством.|
|**Конфигурация устройств**|
|интунеаккаунтид|Guid|Идентификатор учетной записи Intune для данного клиента|
|легаципкмананжементенаблед|Boolean|Свойство, позволяющее управлять устаревшим управлением устаревших ПК для этой учетной записи. Это свойство доступно только для чтения.|
|максимумдептокенс|Int32|Максимальное число маркеров DEP, разрешенных для каждого клиента.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Параметры уровня учетной записи.|
|**Управление устройствами**|
|аккаунтмовекомплетиондатетиме|DateTimeOffset|Дата & время, когда данные клиента перемещаются между скалеунитс.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Сведения о согласия администратора.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);|Общие сведения о защите устройств.|
|managedDeviceCleanupSettings;|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);|Правило очистки устройств|
|subscriptionState|[девицеманажементсубскриптионстате](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Состояние подписки на управление мобильными устройствами для клиента. Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|subscriptions|[девицеманажементсубскриптионс](../resources/intune-devices-devicemanagementsubscriptions.md)|Подписка клиента. Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Обзор вредоносных программ для устройств с Windows.|
|**Аналитика групповой политики**|
|граупполициобжектфилес|Коллекция [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Список загруженных файлов объектов групповой политики.|
|**Адаптация**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.|
|**одж**|
|домаинжоинконнекторс|Коллекция [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Список объектов Connector.|

## <a name="relationships"></a>Связи
|Связь|Тип|Обзор&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android для работы**|
|андроиддевицеовнеренроллментпрофилес|Коллекция [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Объекты профилей регистрации владельца устройств Android.|
|androidForWorkAppConfigurationSchemas|Коллекция [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Сущности схемы конфигурации в приложении Android for Work.|
|androidForWorkEnrollmentProfiles|Коллекция [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Сущности профиля регистрации Android for Work.|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Одноэлементная сущность параметров Android for Work.|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Одноэлементная сущность учетной записи для учетной записи управляемого хранилища Android.|
|андроидманажедстореаппконфигуратионсчемас|Коллекция [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|Сущности схемы конфигурации корпоративных приложений Android.|
|**Аудит**|
|auditEvents|Коллекция [auditEvent](../resources/intune-auditing-auditevent.md)|События аудита|
|**Условия компании**|
|termsAndConditions|Коллекция [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Условия, связанные с управлением устройствами в компании.|
|**Политики конфигурации**|
|конфигуратионполиЦиес|Коллекция [девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-deviceManagementConfigurationPolicy.md)|Список всех политик конфигурации|
|конфигуратионсеттингс|Коллекция [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-deviceManagementConfigurationSettingDefinition.md)|Список всех Конфигуратионсеттингс|
|конфигуратионкатегориес|Коллекция [девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-deviceManagementConfigurationCategory.md)|Список всех категорий конфигурации|
|**Корпоративная регистрация**|
|enrollmentProfiles|Коллекция [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|Профили регистрации.|
|importedAppleDeviceIdentities|Коллекция [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|Импортированные удостоверения устройств Apple.|
|импортеддевицеидентитиес|Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Импортированные удостоверения устройств.|
|**Конфигурация устройств**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Сводное состояние состояния входящей миграции ATP для этой учетной записи.|
|Свойства carttoclassassociations|Коллекция [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md)|Корзина для сопоставления классов.|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|Политики соответствия устройств требованиям.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Общие сведения о состоянии соответствия устройств требованиям для этой учетной записи.|
|deviceCompliancePolicySettingStateSummaries|Коллекция [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Общие сведения о состоянии параметров политики соответствия требованиям для этой учетной записи.|
|deviceConfigurationConflictSummary|Коллекция [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Сводка политик в состоянии конфликтов для этой учетной записи.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Общие сведения о состоянии конфигурации устройства для этой учетной записи.|
|девицеконфигуратионрестриктедаппсвиолатионс|Коллекция [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md)|Нарушения ограниченного доступа к приложениям для этой учетной записи.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|Конфигурации устройств.|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md);|Сводка по состоянию пользователей конфигурации устройств для этой учетной записи.|
|iosUpdateStatuses|Коллекция [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Состояния установки обновления программного обеспечения IOS для этой учетной записи.|
|ндесконнекторс|Коллекция [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md)|Коллекция соединителей NDES для этой учетной записи.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Общие сведения о состоянии обновления программного обеспечения.|
|**Цель устройства**|
|целей|Коллекция [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md)|Целей управления устройствами|
|сеттингдефинитионс|Коллекция [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Определения параметров намерения управления устройствами|
|шаблонов|Коллекция [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|Доступные шаблоны|
|categories|Коллекция [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Доступные категории|
|**Управление устройствами**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Сертификат push-уведомлений Apple|
|даташарингконсентс|Коллекция [даташарингконсент](../resources/intune-devices-datasharingconsent.md)|Совместное использование данных.|
|detectedApps|Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)|Список обнаруженных приложений, связанных с устройством.|
|deviceManagementScripts|Коллекция [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Список сценариев управления устройствами, связанных с клиентом.|
|девицешеллскриптс|Коллекция [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md)|Список сценариев оболочки устройств, связанных с клиентом.|
|девицехеалсскриптс|Коллекция [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md)|Список сценариев работоспособности устройств, связанных с клиентом.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Обзор устройств|
|managedDevices|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Список управляемых устройств.|
|ремотеактионаудитс|Коллекция [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Список аудитов удаленных действий устройств с клиентом.|
|windowsMalwareInformation|Коллекция [windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md)|Список уязвимых вредоносных программ в клиенте.|
|мобилеапптраублешутинжевентс|Коллекция [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md)|Свойство Collection объекта Мобилеапптраублешутинжевент.|
|userExperienceAnalyticsOverview|[userExperienceAnalyticsOverview](../resources/intune-devices-userExperienceAnalyticsOverview.md)|Обзор анализа пользовательского интерфейса|
|усерекспериенцеаналитиксбаселинес|Коллекция [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userExperienceAnalyticsBaseline.md)|Шаблоны аналитики взаимодействия с пользователем|
|усерекспериенцеаналитикскатегориес|Коллекция [усерекспериенцеаналитикскатегори](../resources/intune-devices-userExperienceAnalyticsCategory.md)|Категории аналитики взаимодействия с пользователем|
|userExperienceAnalyticsDevicePerformance|Коллекция [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userExperienceAnalyticsDevicePerformance.md)|Производительность устройства аналитики взаимодействия с пользователем|
|userExperienceAnalyticsRegressionSummary|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userExperienceAnalyticsRegressionSummary.md)|Сводка по регрессии аналитики взаимодействия с пользователем|
|userExperienceAnalyticsDeviceStartupHistory|Коллекция [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userExperienceAnalyticsDeviceStartupHistory.md)|Журнал запуска устройства Analytics User Experience|
|усерекспериенцеаналитиксдевицестартуппроцессес|Коллекция [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userExperienceAnalyticsDeviceStartupProcess.md)|Процессы запуска устройства Analytics User Experience|
|userExperienceAnalyticsDeviceStartupProcessPerformance|Коллекция [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userExperienceAnalyticsDeviceStartupProcessPerformance.md)|Производительность процесса запуска устройства Analytics User Experience|
|**Регистрации**|
|depOnboardingSettings|Коллекция [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Эти коллекции нескольких маркеров DEP для каждого клиента.|
|импортеддевицеидентитиес|Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Импортированные удостоверения устройств.|
|importedWindowsAutopilotDeviceIdentities|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Коллекция импортированных устройств Windows AutoPilot.|
|виндовсаутопилотдеплойментпрофилес|Коллекция [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Профили развертывания автоматического пилотного развертывания Windows|
|виндовсаутопилотдевицеидентитиес|Коллекция [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Коллекция удостоверений устройств с автопилотом Windows содержит коллекцию.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Параметры учетной записи автопилота Windows.|
|**Встроенная SIM-карта**|
|ембеддедсимактиватионкодепулс|Коллекция [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md)|Встроенные пулы кода активации SIM-карты, созданные этой учетной записью.|
|**Ограждение**|
|манажементкондитионс|Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)|Условия управления, связанные с управлением устройствами компании.|
|манажементкондитионстатементс|Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)|Операторы условия управления, связанные с управлением устройствами компании.|
|**Аналитика групповой политики**|
|граупполицимигратионрепортс|Коллекция [граупполицимигратионрепорт](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Список отчетов о миграции групповой политики.|
|**микрософттуннел**|
|микрософттуннелконфигуратионс|Коллекция [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsoftTunnelConfiguration.md)|Коллекция параметров Микрософттуннелконфигуратион, связанных с учетной записью.|
|микрософттуннелситес|Коллекция [микрософттуннелсите](../resources/intune-mstunnel-microsoftTunnelSite.md)|Коллекция параметров Микрософттуннелсите, связанных с учетной записью.|
|**Уведомления**|
|notificationMessageTemplates|Коллекция [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Шаблоны сообщений уведомления.|
|**Адаптация**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Параметры локального условного доступа в Exchange. Для локального условного доступа устройства должны быть зарегистрированы для доступа к почте и поддерживать его.|
|Объекты deviceCategory|Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)|Список категорий устройств в клиенте.|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Список настроек регистрации устройств.|
|Объекты deviceManagementPartner|Коллекция объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Список партнеров по управлению устройствами, настроенных с помощью клиента.|
|Объекты exchangeConnector|Коллекция объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Список соединителей Exchange, настроенных с помощью клиента.|
|ексчанжеонпремисесполиЦиес|Коллекция [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Список политик Exchange для Премисис, настроенных клиентом.|
|ексчанжеонпремисесполици|[девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Политика, которая управляет доступом мобильных устройств к локальной среде Exchange|
|Объекты mobileThreatDefenseConnector|Коллекция объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Список соединителей Mobile Threat Defense, настроенных с помощью клиента.|
|**Набор политик**|
|deviceManagementScripts|Коллекция [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Список сценариев управления устройствами, связанных с клиентом.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|Список конфигураций устройств, связанных с клиентом.|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|Список политик соответствия требованиям к устройствам, связанных с клиентом.|
|виндовсаутопилотдеплойментпрофилес|Коллекция [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Профили развертывания автоматического пилотного развертывания Windows|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Список настроек регистрации устройств.|
|**Полци доступа к ресурсам**|
|дериведкредентиалс|Коллекция [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Коллекция параметров производных учетных данных, связанных с учетной записью.|
|**Удаленный доступ**|
|усерпфксцертификатес|Коллекция [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md)|Коллекция сертификатов PFX, связанных с пользователем.|
|**Удаленная помощь**|
|remoteAssistancePartners|Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Партнеры по удаленной помощи.|
|**Управление доступом на основе ролей (RBAC)**|
|resourceOperations|Коллекция [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Операции с ресурсами.|
|roleAssignments|Коллекция [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Назначения ролей.|
|roleDefinitions|Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)|Определения ролей.|
|roleScopeTags|Коллекция [ролескопетаг](../resources/intune-rbac-rolescopetag.md)|Теги области применения роли.|
|**Создание отчетов**|
|определяется|[deviceManagementReports](../resources/intune-shared-devicemanagementreports.md)|Одноэлементные отчеты|
|**Обновление программного обеспечения**|
|виндовсфеатуреупдатепрофилес|Коллекция [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|Коллекция профилей обновления компонентов Windows|
|**Управление расходами по телекоммуникационной связи (TEM)**|
|telecomExpenseManagementPartners|Коллекция [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Партнеры по управлению затратами на телекоммуникации.|
|**Устранение неполадок**|
|troubleshootingEvents|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Список событий устранения неполадок для клиента.|
|**Windows Information Protection**|
|интунебрандингпрофилес|Коллекция [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md)|Профили фирменной символики Intune, предназначенные для групп AAD|
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




