---
title: тип ресурса windowsIdentityProtectionConfiguration
description: Эта сущность содержит описания объявленных методов, свойств и связей, Windows Hello для бизнеса.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 594417da4102653e4d7c1e4d7653c84967cb83431935585874761c7e6d6da599
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164309"
---
# <a name="windowsidentityprotectionconfiguration-resource-type"></a>тип ресурса windowsIdentityProtectionConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность содержит описания объявленных методов, свойств и связей, Windows Hello для бизнеса.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsIdentityProtectionConfigurations](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-list.md)|[коллекция windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Список свойств и связей [объектов WindowsIdentityProtectionConfiguration.](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|
|[Получить windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-get.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Чтение свойств и связей [объекта WindowsIdentityProtectionConfiguration.](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|
|[Создание windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-create.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Создайте [новый объект WindowsIdentityProtectionConfiguration.](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|
|[Удаление windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-delete.md)|Нет|Удаляет [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).|
|[Обновление windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-update.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Обновление свойств объекта [WindowsIdentityProtectionConfiguration.](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|useSecurityKeyForSignin|Логический|Значение Boolean, используемее для Windows Hello ключа безопасности в качестве учетных данных с логотипом.|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Логический|Значение Boolean, используемого для обеспечения расширенного анти-спуфинга для распознавания лицевых функций Windows Hello проверки подлинности.|
|pinMinimumLength|Int32|Значение Integer, которое задает минимальное количество символов, необходимых для Windows Hello для бизнес-ПИН-кода. Допустимые значения : от 4 до 127 включительно и меньше или меньше значения, установленного для максимального ПИН-кода. Допустимые значения от 4 до 127|
|pinMaximumLength|Int32|Значение Integer, которое задает максимальное количество символов, разрешенных для пин-кода работы. Допустимые значения от 4 до 127 включительно и больше или равны значению, за набором для минимального ПИН-кода. Допустимые значения от 4 до 127|
|pinUppercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Это значение настраивает использование символов верхнего регистра в пин-Windows Hello для бизнеса. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|pinLowercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Это значение настраивает использование символов нижнего регистра в пин-Windows Hello для бизнеса. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|pinSpecialCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Управление возможностью использования специальных символов в Windows Hello для бизнеса PIN-код. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|pinExpirationInDays|Int32|Значение integer указывает период (в днях), который ПИН-код можно использовать до того, как система потребует от пользователя его изменить. Допустимые значения : от 0 до 730 включительно. Допустимые значения: от 0 до 730.|
|pinPreviousBlockCount|Int32|Контролирует возможность предотвращения использования пользователями прошлых ПИН-данных. Это должно быть установлено между 0 и 50 включительно, и текущий ПИН-код пользователя включен в это число. Если установлено 0, предыдущие ПИН-данные не сохраняются. История ПИН-кода не сохраняется с помощью сброса ПИН-кода. Допустимые значения: от 0 до 50.|
|pinRecoveryEnabled|Логический|Значение Boolean, которое позволяет пользователю изменять ПИН-код с помощью Windows Hello службы восстановления ПИН-кода для бизнеса.|
|securityDeviceRequired|Boolean|Управление, необходимо ли требовать доверенный модуль платформы (TPM) для Windows Hello для бизнеса. TPM предоставляет дополнительные преимущества безопасности в том, что данные, хранимые на нем, не могут использоваться на других устройствах. Если установлено false, все устройства могут Windows Hello для бизнеса, даже если нет необходимого TPM.|
|unlockWithBiometricsEnabled|Boolean|Управление использованием биометрических жестов, таких как лицо и отпечатки пальцев, в качестве альтернативы Windows Hello для бизнеса PIN-код.  Если установлено false, биометрические жесты не допускаются. Пользователи по-прежнему должны настраивать ПИН-код в качестве резервного копирования в случае сбоев.|
|useCertificatesForOnPremisesAuthEnabled|Логический|Значение Boolean, Windows Hello для бизнеса использовать сертификаты для проверки подлинности локального ресурса.|
|windowsHelloForBusinessBlocked|Boolean|Значение Boolean, Windows Hello для бизнеса как метод для подписания в Windows.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|

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
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
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




