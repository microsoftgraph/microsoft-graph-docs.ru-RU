---
title: Тип ресурса deviceEnrollmentNotificationConfiguration
description: Конфигурация уведомления о регистрации, используемая для отправки уведомления
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 370fd69ef878051dca2a62ef98b84f93de806ed3
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213311"
---
# <a name="deviceenrollmentnotificationconfiguration-resource-type"></a>Тип ресурса deviceEnrollmentNotificationConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация уведомления о регистрации, используемая для отправки уведомления


Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceEnrollmentNotificationConfiguration](../api/intune-onboarding-deviceenrollmentnotificationconfiguration-list.md)|[Коллекция deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md)|Список свойств и связей объектов [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) .|
|[Получение объекта deviceEnrollmentNotificationConfiguration](../api/intune-onboarding-deviceenrollmentnotificationconfiguration-get.md)|[deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md)|Чтение свойств и связей объекта [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) .|
|[Создание объекта deviceEnrollmentNotificationConfiguration](../api/intune-onboarding-deviceenrollmentnotificationconfiguration-create.md)|[deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md)|Создайте объект [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) .|
|[Удаление объекта deviceEnrollmentNotificationConfiguration](../api/intune-onboarding-deviceenrollmentnotificationconfiguration-delete.md)|Нет|Удаляет [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md).|
|[Обновление объекта deviceEnrollmentNotificationConfiguration](../api/intune-onboarding-deviceenrollmentnotificationconfiguration-update.md)|[deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md)|Обновление свойств объекта [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор учетной записи, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|Строка|Отображаемое имя конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|Строка|Описание конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|Приоритет используется, когда пользователь существует в нескольких группах, для которых назначена конфигурация регистрации. На пользователей распространяется только конфигурация с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Дата создания в формате UTC конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения в формате UTC конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|Идентификаторы roleScopeTagId|Коллекция объектов string|Необязательные теги области роли для ограничений регистрации. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|DeviceEnrollmentConfigurationType|[DeviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|Поддержка типа конфигурации регистрации, унаследованного [от deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md). Возможные значения: `unknown`, `limit`, `platformRestrictions`, `windowsHelloForBusiness`, `defaultLimit`, `defaultPlatformRestrictions`, `defaultWindowsHelloForBusiness`, `defaultWindows10EnrollmentCompletionPageConfiguration`, `windows10EnrollmentCompletionPageConfiguration`, `deviceComanagementAuthorityConfiguration`, `singlePlatformRestriction`, `unknownFutureValue`, `enrollmentNotificationsConfiguration`.|
|platformType|[enrollmentRestrictionPlatformType](../resources/intune-onboarding-enrollmentrestrictionplatformtype.md)|Тип платформы уведомления о регистрации. Возможные значения: `allPlatforms`, `ios`, `windows`, `windowsPhone`, `android`, `androidForWork`, `mac`.|
|templateType|[enrollmentNotificationTemplateType](../resources/intune-onboarding-enrollmentnotificationtemplatetype.md)|Тип шаблона уведомления о регистрации. Возможные значения: `email`, `push`, `unknownFutureValue`.|
|NotificationMessageTemplateId|Guid|Идентификатор шаблона сообщения уведомления|
|brandingOptions|[enrollmentNotificationBrandingOptions](../resources/intune-onboarding-enrollmentnotificationbrandingoptions.md)|Параметры фирменной символики для уведомления о регистрации. Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`, `includeDeviceDetails`.|
|defaultLocale|String|DefaultLocale для уведомления о регистрации|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Список назначений групп для профиля конфигурации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentNotificationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentNotificationConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ],
  "deviceEnrollmentConfigurationType": "String",
  "platformType": "String",
  "templateType": "String",
  "notificationMessageTemplateId": "Guid",
  "brandingOptions": "String",
  "defaultLocale": "String"
}
```




