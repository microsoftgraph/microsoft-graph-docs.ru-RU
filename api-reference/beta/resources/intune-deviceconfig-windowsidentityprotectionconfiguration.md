---
title: Тип ресурса windowsIdentityProtectionConfiguration
description: Этот объект содержит описания объявленные методы, свойства и связи, предоставляемые Windows Hello для бизнеса.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 431e85e0daddb10e2726dd65e5a6770cf80a0452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398599"
---
# <a name="windowsidentityprotectionconfiguration-resource-type"></a>Тип ресурса windowsIdentityProtectionConfiguration

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Этот объект содержит описания объявленные методы, свойства и связи, предоставляемые Windows Hello для бизнеса.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsIdentityProtectionConfigurations](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-list.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) коллекции|Свойства списка и связей объектов [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|
|[Получение windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-get.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Чтение свойства и связи объекта [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|
|[Создание windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-create.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Создание нового объекта [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|
|[Удаление windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-delete.md)|Нет|Удаляет [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).|
|[Обновление windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-update.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Обновление свойства объекта [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия. Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью. Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|useSecurityKeyForSignin|Логический|Логическое значение, используемое для включения Windows Hello безопасности ключа в виде учетные данные входа в систему.|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Логический|Логическое значение, используемое для включения усовершенствованные спуфинг anti для распознавания лица компонента на Windows Hello лицевой проверки подлинности.|
|pinMinimumLength|Int32|Целое значение, задает минимальное число символов, необходимое для Windows Hello для бизнеса ПИН-кода. Допустимые значения: 4 до 127 включительно и меньше или равно значению набор для максимального ПИН-кода. Допустимые значения 4 до 127|
|pinMaximumLength|Int32|Целое значение, которое задает максимальное число символов, допустимое для работы ПИН-кода. Допустимые значения: 4 до 127 включительно и больше или равно значение, установленное для минимальные ПИН-кода. Допустимые значения 4 до 127|
|pinUppercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Это значение настраивается использование прописные буквы в Windows Hello для бизнеса ПИН-кода. Возможные значения: `blocked`, `required`, `allowed`.|
|pinLowercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Это значение настраивается использование строчные буквы в Windows Hello для бизнеса ПИН-кода. Возможные значения: `blocked`, `required`, `allowed`.|
|pinSpecialCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Определяет возможность использования специальных символов в Windows Hello для бизнеса ПИН-кода. Возможные значения: `blocked`, `required`, `allowed`.|
|pinExpirationInDays|Int32|Целое значение указывает период (в днях), можно ли использовать ПИН-код до его обязательного изменения пользователем. Допустимые значения: 0 для 730 включительно. Допустимые значения: от 0 до 730.|
|pinPreviousBlockCount|Int32|Определяет возможность запретить пользователям с помощью предыдущих ПИН-коды. Это должно иметь значение от 0 до 50, включительно, и текущий ПИН-код пользователя включается в этот счетчик. Если значение 0, предыдущих ПИН-коды не сохраняются. ПИН-код не сохраняется через ПИН-код сбросить. Допустимые значения: от 0 до 50.|
|pinRecoveryEnabled|Логический|Логическое значение, которое позволяет пользователям изменять свой ПИН-код с помощью Windows Hello для восстановления службы Business ПИН-кода.|
|securityDeviceRequired|Boolean|Определяет необходимость доверенного платформы модуля (TPM) для подготовки Windows Hello для бизнеса. TPM обеспечивает дополнительных преимуществ для безопасности, в том, что данные, хранящиеся на его нельзя использовать на других устройствах. Если задано значение False, все устройства можно подготовить Windows Hello для бизнеса даже в том случае, если не могут использоваться TPM.|
|unlockWithBiometricsEnabled|Boolean|Управляет Биометрическая жестов, таких как начертание и отпечаток, как альтернативы Windows Hello для бизнеса ПИН-кода.  Если параметр имеет значение False, Биометрическая жесты не разрешены. Пользователи по-прежнему необходимо настроить ПИН-код для резервного копирования в случае сбоев.|
|useCertificatesForOnPremisesAuthEnabled|Логический|Логическое значение, включающее Windows Hello для бизнеса для использования сертификатов для проверки подлинности локальным ресурсам.|
|windowsHelloForBusinessBlocked|Логический|Логическое значение, которое блокирует Windows Hello для бизнеса, как метод для входа в Windows.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) коллекции|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
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




