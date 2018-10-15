# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс deviceManagement представляет контейнер, содержимое которого различается в зависимости от рабочего процесса, включая следующие элементы:  

- События аудита
- Корпоративные сроки и условия 
- Корпоративные профили регистрации
- Параметры конфигурации устройства
- Управление устройствами
- Защита конечной точки
- Профили регистрации
- Уведомления
- Вводные политики, параметры и сведения
- Политики управления доступа на основе роли
- Удаленные вспомогательные партнеры
- Партнеры управления расширением телекоммуникаций
- События, связанные с устранением неполадок
- Сводки по Windows Information Protection

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune_shared_devicemanagement_get.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune_shared_devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune_shared_devicemanagement_update.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md)|Обновление свойств объекта [deviceManagement](../resources/intune_shared_devicemanagement.md).|
|**On-boarding**|
|[Функция verifyWindowsEnrollmentAutoDiscovery](../api/intune_shared_devicemanagement_verifywindowsenrollmentautodiscovery.md)|Boolean|Н/Д|
|**RBAC**|
|[Функция getEffectivePermissions](../api/intune_shared_devicemanagement_geteffectivepermissions.md)|Коллекция [rolePermission](../resources/intune_rbac_rolepermission.md) или коллекция строк|Получает действующие разрешения пользователя, прошедшего проверку подлинности|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства.|
|**Конфигурация устройства**|
|settings|[deviceManagementSettings](../resources/intune_deviceconfig_devicemanagementsettings.md)|Параметры уровня учетной записи.|
|**Управление устройствами**|
|subscriptionState|String|Состояние подписки на управление мобильными устройствами для клиента. Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|**On-boarding**|
|intuneBrand|[intuneBrand](../resources/intune_onboarding_intunebrand.md)|Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Аудит**|
|auditEvents|Коллекция [auditEvent](../resources/intune_auditing_auditevent.md)|События аудита|
|**Корпоративные сроки и условия**|
|termsAndConditions|Коллекция [termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Условия, связанные с управлением устройствами в компании.|
|**Конфигурация устройства**|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|Политики соответствия устройств требованиям.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|Общие сведения о состоянии соответствия устройств требованиям для этой учетной записи.|
|deviceCompliancePolicySettingStateSummaries|Коллекция [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md)|Общие сведения о состоянии параметров политики соответствия требованиям для этой учетной записи.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|Общие сведения о состоянии конфигурации устройства для этой учетной записи.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|Конфигурации устройств.|
|iosUpdateStatuses|Коллекция [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)|Состояния установки обновления программного обеспечения IOS для этой учетной записи.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|Общие сведения о состоянии обновления программного обеспечения.|
|**Управление устройствами**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Сертификат push-уведомлений Apple|
|detectedApps|Коллекция [detectedApp](../resources/intune_devices_detectedapp.md)|Список обнаруженных приложений, связанных с устройством.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)|Обзор устройств|
|managedDevices|Коллекция [managedDevice](../resources/intune_devices_manageddevice.md)|Список управляемых устройств.|
|**Регистрация**|
|importedWindowsAutopilotDeviceIdentities|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Коллекция импортированных устройств Windows AutoPilot.|
|importedWindowsAutopilotDeviceIdentityUploads|Коллекция [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|Коллекция импортированных устройств Windows AutoPilot.|
|**Уведомления**|
|notificationMessageTemplates|Коллекция [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Шаблоны сообщений уведомления.|
|**On-boarding**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|Параметры локального условного доступа в Exchange. Для локального условного доступа устройства должны быть зарегистрированы для доступа к почте и поддерживать его.|
|deviceCategories|Коллекция объектов [deviceCategory](../resources/intune_shared_devicecategory.md)|Список категорий устройств в клиенте.|
|deviceEnrollmentConfigurations|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|Список настроек регистрации устройств.|
|deviceManagementPartners|Коллекция объектов [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|Список партнеров по управлению устройствами, настроенных с помощью клиента.|
|exchangeConnectors|Коллекция объектов [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|Список соединителей Exchange, настроенных с помощью клиента.|
|mobileThreatDefenseConnectors|Коллекция объектов [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Список соединителей Mobile Threat Defense, настроенных с помощью клиента.|
|**RBAC**|
|resourceOperations|Коллекция [resourceOperation](../resources/intune_rbac_resourceoperation.md)|Операции с ресурсами.|
|roleAssignments|Коллекция [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|Назначения ролей.|
|roleDefinitions|Коллекция [roleDefinition](../resources/intune_rbac_roledefinition.md)|Определения ролей.|
|**Удаленная помощь**|
|remoteAssistancePartners|Коллекция [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Партнеры по удаленной помощи.|
|**Управление расходами на телекоммуникации**|
|telecomExpenseManagementPartners|Коллекция [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|Партнеры по управлению затратами на телекоммуникации.|
|**Устранение неполадок**|
|troubleshootingEvents|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|Список событий, связанных с устранением неполадок для клиента.|
|**Windows Information Protection**|
|windowsInformationProtectionAppLearningSummaries|Коллекция [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)|Сводки по обучению Windows Information Protection для приложений.|
|windowsInformationProtectionNetworkLearningSummaries|Коллекция [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|Сводки по обучению Windows Information Protection для сетей.|


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "intuneBrand": {"@odata.type": "microsoft.graph.intuneBrand"},
  "subscriptionState": "String",
  "settings": {"@odata.type": "microsoft.graph.deviceManagementSettings"}
}
```



