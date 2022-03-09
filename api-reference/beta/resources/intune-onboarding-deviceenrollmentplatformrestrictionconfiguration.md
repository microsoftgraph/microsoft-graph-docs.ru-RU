---
title: тип ресурса deviceEnrollmentPlatformRestrictionConfiguration
description: Конфигурация регистрации устройств, ограничивающая типы устройств, которые пользователь может зарегистрировать для одной платформы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 50388e5e9c265f2e257d8eef1498ecaf8855e799
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63368030"
---
# <a name="deviceenrollmentplatformrestrictionconfiguration-resource-type"></a>тип ресурса deviceEnrollmentPlatformRestrictionConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация регистрации устройств, ограничивающая типы устройств, которые пользователь может зарегистрировать для одной платформы


Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список устройствEnrollmentPlatformRestrictionConfigurations](../api/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration-list.md)|[коллекция deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)|Список свойств и связей [объектов deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) .|
|[Get deviceEnrollmentPlatformRestrictionConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration-get.md)|[deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)|Чтение свойств и связей [объекта deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) .|
|[Создание deviceEnrollmentPlatformRestrictionConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration-create.md)|[deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)|Создание нового [объекта deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) .|
|[Удаление deviceEnrollmentPlatformRestrictionConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration-delete.md)|Нет|Удаляет [устройствоEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md).|
|[Обновление устройстваEnrollmentPlatformRestrictionConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration-update.md)|[deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)|Обновление свойств объекта [deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|String|Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|Строка|Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации. Пользователи подчиняются только конфигурации с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|Коллекция String|Необязательные теги области ролей для ограничений регистрации. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|deviceEnrollmentConfigurationType|[deviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|Поддержка типа конфигурации регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md). Возможные значения: `unknown`, `limit`, `platformRestrictions`, `windowsHelloForBusiness`, `defaultLimit`, `defaultPlatformRestrictions`, `defaultWindowsHelloForBusiness`, `defaultWindows10EnrollmentCompletionPageConfiguration`, `windows10EnrollmentCompletionPageConfiguration`, `deviceComanagementAuthorityConfiguration`, `singlePlatformRestriction`, `unknownFutureValue`.|
|platformRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Ограничения на основе платформы, версии операционной системы платформы и владения устройствами|
|platformType|[enrollmentRestrictionPlatformType](../resources/intune-onboarding-enrollmentrestrictionplatformtype.md)|Тип платформы, для которой применяется это ограничение. Возможные значения: `allPlatforms`, `ios`, `windows`, `windowsPhone`, `android`, `androidForWork`, `mac`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Список групповых назначений для профиля конфигурации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestrictionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionConfiguration",
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
  "platformRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "blockedManufacturers": [
      "String"
    ],
    "blockedSkus": [
      "String"
    ]
  },
  "platformType": "String"
}
```




