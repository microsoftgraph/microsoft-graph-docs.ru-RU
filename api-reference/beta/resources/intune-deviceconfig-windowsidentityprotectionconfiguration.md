---
title: Тип ресурса Виндовсидентитипротектионконфигуратион
description: Эта сущность предоставляет описания объявляемых методов, свойств и связей, предоставляемых Windows Hello для бизнеса.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29510dca8eac2713576f847485a9d22d0bedf1d6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168014"
---
# <a name="windowsidentityprotectionconfiguration-resource-type"></a>Тип ресурса Виндовсидентитипротектионконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность предоставляет описания объявляемых методов, свойств и связей, предоставляемых Windows Hello для бизнеса.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсидентитипротектионконфигуратионс](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-list.md)|Коллекция [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Список свойств и связей объектов [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|
|[Получение Виндовсидентитипротектионконфигуратион](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-get.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Чтение свойств и связей объекта [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|
|[Создание Виндовсидентитипротектионконфигуратион](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-create.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Создание нового объекта [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|
|[Удаление Виндовсидентитипротектионконфигуратион](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-delete.md)|Нет|Удаляет объект [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).|
|[Обновление Виндовсидентитипротектионконфигуратион](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-update.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Обновление свойств объекта [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Усесекуритикэйфорсигнин|Логический|Логическое значение, используемое для включения ключа безопасности Windows Hello в качестве учетных данных для входа.|
|ЕнханцедантиспуфингфорфаЦиалфеатуресенаблед|Логический|Логическое значение, используемое для включения расширенного средства защиты от спуфинга для распознавания функции лица при проверке подлинности Windows Hello для лиц.|
|pinMinimumLength|Int32|Целочисленное значение, задающее минимальное число символов, необходимое для ПИН-кода Windows Hello для бизнеса. Допустимые значения: от 4 до 127 включительно и меньше или равны набору значений для максимального ПИН-кода. Допустимые значения — от 4 до 127|
|pinMaximumLength|Int32|Целое значение, задающее максимальное количество символов для рабочего ПИН-кода. Допустимые значения: от 4 до 127 включительно и больше или равны значению, заданному для минимального ПИН-кода. Допустимые значения — от 4 до 127|
|pinUppercaseCharactersUsage|[Конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Это значение позволяет настроить использование символов верхнего регистра в ПИН-коде Windows Hello для бизнеса. Возможные значения: `blocked`, `required`, `allowed`.|
|pinLowercaseCharactersUsage|[Конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Это значение позволяет настроить использование символов нижнего регистра в ПИН-коде Windows Hello для бизнеса. Возможные значения: `blocked`, `required`, `allowed`.|
|pinSpecialCharactersUsage|[Конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Управляет возможностью использования специальных символов в ПИН-коде Windows Hello для бизнеса. Возможные значения: `blocked`, `required`, `allowed`.|
|pinExpirationInDays|Int32|Integer value указывает период времени (в днях), в течение которого можно использовать ПИН-код, прежде чем система потребует от пользователя изменить его. Допустимые значения: от 0 до 730 включительно. Допустимые значения: от 0 до 730.|
|pinPreviousBlockCount|Int32|Управляет возможностью запретить пользователям использовать прошлые контакты. Он должен иметь значение от 0 до 50 включительно, а текущий ПИН-код пользователя включен в этот счетчик. Если задано значение 0, предыдущие ПИН-коды не сохраняются. История ПИН-кодов не сохраняется при сбросе ПИН-кода. Допустимые значения: от 0 до 50.|
|Пинрековеренаблед|Логический|Логическое значение, которое позволяет пользователю изменить свой ПИН-код с помощью службы восстановления ПИН-кода Windows Hello для бизнеса.|
|securityDeviceRequired|Логический|Определяет, требуется ли доверенный ПЛАТФОРМЕНный модуль для подготовки Windows Hello для бизнеса. TPM предоставляет дополнительные преимущества безопасности, которые хранятся на нем, не могут использоваться на других устройствах. Если задано значение false, все устройства могут подготавливать Windows Hello для бизнеса, даже если нет пригодного к использованию ДОВЕРЕНного ПЛАТФОРМЕНного модуля.|
|unlockWithBiometricsEnabled|Логический|Управляет использованием биометрических жестов, таких как лицо и отпечаток, в качестве альтернативы ПИН-коду Windows Hello для бизнеса.  Если задано значение false, биометрические жесты не разрешены. Пользователи по-прежнему должны настроить ПИН-код в качестве резервной копии в случае сбоев.|
|Усецертификатесфоронпремисесаусенаблед|Логический|Логическое значение, которое позволяет Windows Hello для бизнеса использовать сертификаты для проверки подлинности локальных ресурсов.|
|windowsHelloForBusinessBlocked|Логический|Логическое значение, блокирующее Windows Hello для бизнеса в качестве способа входа в Windows.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsIdentityProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "pinExpirationInDays": 1024,
  "pinPreviousBlockCount": 1024,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```




