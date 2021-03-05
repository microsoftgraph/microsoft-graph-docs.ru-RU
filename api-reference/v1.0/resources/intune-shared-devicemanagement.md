---
title: Тип ресурса deviceManagement
description: 'Ресурс deviceManagement представляет контейнер, содержимое которого зависит от рабочего процесса, в том числе:  '
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 83d3f3cda24c5961a34cb5c38de3ee43d6f5fe44
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475774"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс deviceManagement представляет контейнер, содержимое которого зависит от рабочего процесса, в том числе:  

- События аудита  
- Корпоративные условия   
- Параметры конфигурации устройства  
- Управление устройствами  
- Endpoint Protection  
- Профили регистрации  
- Уведомления  
- Политики, параметры и подробные сведения  
- Политики управления доступом на основе ролей (RBAC)  
- Партнеры удаленной помощи  
- Партнеры по управлению телекоммуникационными ресурсами  
- События устранения неполадок  
- Сводки по защите информации Windows  

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune-shared-devicemanagement-get.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune-shared-devicemanagement-update.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md)|Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).|
|**Адаптация**|
|[Функция verifyWindowsEnrollmentAutoDiscovery](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Boolean|Н/Д|
|**RBAC**|
|[Функция getEffectivePermissions](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|[коллекция rolePermission](../resources/intune-rbac-rolepermission.md) или коллекция строк|Получает действующие разрешения пользователя, прошедшего проверку подлинности|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства.|
|**Конфигурация устройств**|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Параметры уровня учетной записи.|
|**Управление устройствами**|
|subscriptionState|String|Состояние подписки на управление мобильными устройствами для клиента. Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|**Адаптация**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Корпоративные условия**|
|termsAndConditions|Коллекция [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Условия, связанные с управлением устройствами в компании.|
|**Конфигурация устройств**|
|intuneAccountId|Guid|ID учетной записи Intune для данного клиента.|
|deviceCompliancePolicies|Коллекция [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|Политики соответствия устройств требованиям.|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Общие сведения о состоянии соответствия устройств требованиям для этой учетной записи.|
|deviceCompliancePolicySettingStateSummaries|Коллекция [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Общие сведения о состоянии параметров политики соответствия требованиям для этой учетной записи.|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|Общие сведения о состоянии конфигурации устройства для этой учетной записи.|
|deviceConfigurations|Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|Конфигурации устройств.|
|iosUpdateStatuses|Коллекция [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Состояния установки обновления программного обеспечения IOS для этой учетной записи.|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Общие сведения о состоянии обновления программного обеспечения.|
|**Управление устройствами**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Сертификат push-уведомлений Apple|
|detectedApps|Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)|Список обнаруженных приложений, связанных с устройством.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Обзор устройств|
|managedDevices|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Список управляемых устройств.|
|**Уведомления**|
|notificationMessageTemplates|Коллекция [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Шаблоны сообщений уведомления.|
|**Адаптация**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Параметры локального условного доступа в Exchange. Для локального условного доступа устройства должны быть зарегистрированы для доступа к почте и поддерживать его.|
|Объекты deviceCategory|Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)|Список категорий устройств в клиенте.|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Список настроек регистрации устройств.|
|Объекты deviceManagementPartner|Коллекция объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Список партнеров по управлению устройствами, настроенных с помощью клиента.|
|complianceManagementPartners|[коллекция complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Список партнеров по управлению соответствием требованиям, настроенный клиентом.|
|Объекты exchangeConnector|Коллекция объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Список соединителей Exchange, настроенных с помощью клиента.|
|Объекты mobileThreatDefenseConnector|Коллекция объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Список соединителей Mobile Threat Defense, настроенных с помощью клиента.|
|**RBAC**|
|resourceOperations|Коллекция [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Операции с ресурсами.|
|roleAssignments|Коллекция [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Назначения ролей.|
|roleDefinitions|Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)|Определения ролей.|
|**Удаленная помощь**|
|remoteAssistancePartners|Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Партнеры по удаленной помощи.|
|**Управление расходами телекома**|
|telecomExpenseManagementPartners|Коллекция [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Партнеры по управлению затратами на телекоммуникации.|
|**Устранение неполадок**|
|troubleshootingEvents|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Список событий устранения неполадок для клиента.|
|**Windows Information Protection**|
|windowsInformationProtectionAppLearningSummaries|Коллекция [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Сводки по обучению Windows Information Protection для приложений.|
|windowsInformationProtectionNetworkLearningSummaries|Коллекция [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Сводки по обучению Windows Information Protection для сетей.|


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









