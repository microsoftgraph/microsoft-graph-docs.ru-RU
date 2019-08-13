---
title: Тип ресурса deviceManagement
description: 'Ресурс deviceManagement представляет контейнер, содержимое которого зависит от рабочего процесса, в том числе:  '
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: be12232d387309992b0e967580dfc8d593c53056
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36376061"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
- Уведомления
- Политики, параметры и сведения о входящей миграции
- Удаленный доступ
- Партнеры удаленного помощника
- Политики управления доступом на основе ролей (RBAC)
- Партнеры по управлению телекоммуникационной експансе
- События устранения неполадок
- Сводки Windows Information Protection

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune-shared-devicemanagement-get.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune-shared-devicemanagement-update.md)|Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|**Настройка устройства**|
|[Действие enableLegacyPcManagement](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|Нет|Пока не задокументировано.|
|**Управление устройствами**|
|[Действие sendCustomNotificationToCompanyPortal](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|Нет|Пока не задокументировано.|
|**Входящая миграция**|
|[Функция verifyWindowsEnrollmentAutoDiscovery](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolean|Н/Д|
|**Управление доступом на основе ролей (RBAC)**|
|[Функция getEffectivePermissions](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)|Получает действующие разрешения пользователя, прошедшего проверку подлинности|
|[Функция Жетролескопетагсбидс](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|Коллекция [ролескопетаг](../resources/intune-rbac-rolescopetag.md)|Пока не задокументировано.|
|[Функция Жетролескопетагсбиресаурце](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|Коллекция [ролескопетаг](../resources/intune-rbac-rolescopetag.md)|Н/Д|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор, связанный с устройством.|
|**Настройка устройства**|
|интунеаккаунтид|GUID|Идентификатор учетной записи Intune для данного клиента|
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
|**Входящая миграция**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.|
|**одж**|
|домаинжоинконнекторс|Коллекция [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Список объектов Connector.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Обзор&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
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
|**Корпоративная регистрация**|
|enrollmentProfiles|Коллекция [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|Профили регистрации.|
|importedAppleDeviceIdentities|Коллекция [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|Импортированные удостоверения устройств Apple.|
|импортеддевицеидентитиес|Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Импортированные удостоверения устройств.|
|**Настройка устройства**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Сводное состояние состояния входящей миграции ATP для этой учетной записи.|
|Свойства carttoclassassociations|Коллекция [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md)|Корзина для сопоставления классов.|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|Политики соответствия устройств требованиям.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Общие сведения о состоянии соответствия устройств требованиям для этой учетной записи.|
|deviceCompliancePolicySettingStateSummaries|Коллекция [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Общие сведения о состоянии параметров политики соответствия требованиям для этой учетной записи.|
|deviceConfigurationConflictSummary|Коллекция [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Сводка политик в состоянии конфликтов для этой учетной записи.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Общие сведения о состоянии конфигурации устройства для этой учетной записи.|
|девицеконфигуратионрестриктедаппсвиолатионс|Коллекция [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md)|Нарушения ограниченного доступа к приложениям для этой учетной записи.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|Конфигурации устройств.|
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
|deviceManagementScripts|Коллекция [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Список сценариев управления устройствами, связанных с клиентом.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Обзор устройств|
|managedDevices|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Список управляемых устройств.|
|ремотеактионаудитс|Коллекция [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Список аудитов удаленных действий устройств с клиентом.|
|windowsMalwareInformation|Коллекция [windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md)|Список уязвимых вредоносных программ в клиенте.|
|**Регистрации**|
|depOnboardingSettings|Коллекция [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Эти коллекции нескольких маркеров DEP для каждого клиента.|
|импортеддевицеидентитиес|Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)|Импортированные удостоверения устройств.|
|importedWindowsAutopilotDeviceIdentities|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Коллекция импортированных устройств Windows AutoPilot.|
|виндовсаутопилотдеплойментпрофилес|Коллекция [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Профили развертывания автоматического пилотного развертывания Windows|
|виндовсаутопилотдевицеидентитиес|Коллекция [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Коллекция удостоверений устройств с автопилотом Windows содержит коллекцию.|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Параметры учетной записи автопилота Windows.|
|**Встроенная SIM-карта**|
|ембеддедсимактиватионкодепулс|Коллекция [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md)|Встроенные пулы кода активации SIM-карты, созданные этой учетной записью.|
|**Ограждение**|
|манажементкондитионс|Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)|Условия управления, связанные с управлением устройствами компании.|
|манажементкондитионстатементс|Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)|Операторы условия управления, связанные с управлением устройствами компании.|
|**Уведомления**|
|notificationMessageTemplates|Коллекция [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Шаблоны сообщений уведомления.|
|**Входящая миграция**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Параметры локального условного доступа в Exchange. Для локального условного доступа устройства должны быть зарегистрированы для доступа к почте и поддерживать его.|
|Объекты deviceCategory|Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)|Список категорий устройств в клиенте.|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Список настроек регистрации устройств.|
|Объекты deviceManagementPartner|Коллекция объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Список партнеров по управлению устройствами, настроенных с помощью клиента.|
|Объекты exchangeConnector|Коллекция объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Список соединителей Exchange, настроенных с помощью клиента.|
|ексчанжеонпремисесполиЦиес|Коллекция [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Список политик Exchange для Премисис, настроенных клиентом.|
|ексчанжеонпремисесполици|[девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Политика, которая управляет доступом мобильных устройств к локальной среде Exchange|
|Объекты mobileThreatDefenseConnector|Коллекция объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Список соединителей Mobile Threat Defense, настроенных с помощью клиента.|
|**Удаленный доступ**|
|усерпфксцертификатес|Коллекция [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md)|Коллекция сертификатов PFX, связанных с пользователем.|
|**Удаленная помощь**|
|remoteAssistancePartners|Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Партнеры по удаленной помощи.|
|**Управление доступом на основе ролей (RBAC)**|
|resourceOperations|Коллекция [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Операции с ресурсами.|
|roleAssignments|Коллекция [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Назначения ролей.|
|roleDefinitions|Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)|Определения ролей.|
|roleScopeTags|Коллекция [ролескопетаг](../resources/intune-rbac-rolescopetag.md)|Теги области применения роли.|
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



