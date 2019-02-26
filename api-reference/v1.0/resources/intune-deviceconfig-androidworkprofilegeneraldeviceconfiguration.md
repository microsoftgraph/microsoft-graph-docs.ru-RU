---
title: Тип ресурса androidWorkProfileGeneralDeviceConfiguration
description: Рабочий профиль Android Общая конфигурация устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39c9a9ee5d995df6ee54809b07d70d347c6a9aea
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254445"
---
# <a name="androidworkprofilegeneraldeviceconfiguration-resource-type"></a>Тип ресурса androidWorkProfileGeneralDeviceConfiguration

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Рабочий профиль Android Общая конфигурация устройства.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроидворкпрофилеженералдевицеконфигуратионс](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-list.md)|Коллекция [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|Список свойств и связей объектов [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .|
|[Получение androidWorkProfileGeneralDeviceConfiguration](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-get.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|Чтение свойств и связей объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .|
|[Создание androidWorkProfileGeneralDeviceConfiguration](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-create.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|Создание нового объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .|
|[Удаление androidWorkProfileGeneralDeviceConfiguration](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-delete.md)|Нет|Удаляет объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).|
|[Обновление androidWorkProfileGeneralDeviceConfiguration](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-update.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|Обновление свойств объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|passwordBlockFingerprintUnlock|Логический|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passwordBlockTrustAgents|Boolean|Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.|
|passwordExpirationDays|Int32|Количество дней до окончания срока действия пароля. Допустимые значения: от 1 до 365.|
|passwordMinimumLength|Int32|Минимальная длина паролей. Допустимые значения: от 4 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, которые требуется блокировать. Допустимые значения: от 0 до 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек. Допустимые значения — от 1 до 16.|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|Воркпрофиледаташарингтипе|[androidWorkProfileCrossProfileDataSharingType](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|Тип разрешенного общего доступа к данным. Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.|
|Воркпрофилеблоккнотификатионсвхиледевицелоккед|Логический|Указывает, следует ли блокировать уведомления, когда устройство заблокировано.|
|Воркпрофилеблоккаддингаккаунтс|Логический|Запретить пользователям добавлять и удалять учетные записи в рабочем профиле.|
|Воркпрофилеблуетусенаблеконтактшаринг|Логический|Разрешить устройствам Bluetooth получать доступ к корпоративным контактам.|
|Воркпрофилеблоккскринкаптуре|Логический|Блокировать снимок экрана в рабочем профиле.|
|Воркпрофилеблокккросспрофилекаллерид|Логический|Блокировать отображение идентификатора исполнителя рабочего профиля в личном профиле.|
|Свойства workprofileblockcamera|Логический|Блокировать камеру рабочего профиля.|
|workProfileBlockCrossProfileContactsSearch|Логический|Блокировать доступность контактов для рабочих профилей в личном профиле.|
|Воркпрофилеблокккросспрофилекопипасте|Логический|Логическое значение, которое указывает, включено ли для параметра возможность копирования и вставки в нескольких профилях.|
|Воркпрофиледефаултапппермиссионполици|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|Свойства workprofilepasswordblockfingerprintunlock|Логический|Указывает, следует ли заблокировать разблокировку отпечатков пальцев для рабочего профиля.|
|workProfilePasswordBlockTrustAgents|Логический|Указывает, следует ли заблокировать для рабочего профиля интеллектуальную блокировку и другие агенты доверия.|
|workProfilePasswordExpirationDays|Int32|Количество дней до истечения срока действия пароля рабочего профиля. Допустимые значения: от 1 до 365.|
|workProfilePasswordMinimumLength|Int32|Минимальная длина пароля рабочего профиля. Допустимые значения: от 4 до 16.|
|Воркпрофилепассвордминнумерикчарактерс|Int32|Минимальное количество числовых символов в пароле рабочего профиля. Допустимые значения — от 1 до 10|
|Воркпрофилепассвордминнонлеттерчарактерс|Int32|Минимальное количество небуквенных символов, необходимых в пароле рабочего профиля. Допустимые значения — от 1 до 10|
|Воркпрофилепассвордминлеттерчарактерс|Int32|Минимальное количество символов в пароле рабочего профиля. Допустимые значения — от 1 до 10|
|Воркпрофилепассвордминловеркасечарактерс|Int32|Минимальное количество символов нижнего регистра в пароле рабочего профиля. Допустимые значения — от 1 до 10|
|Воркпрофилепассвордминупперкасечарактерс|Int32|Минимальное количество символов верхнего регистра в пароле рабочего профиля. Допустимые значения — от 1 до 10|
|Воркпрофилепассвордминсимболчарактерс|Int32|Минимальное количество символов в пароле рабочего профиля. Допустимые значения — от 1 до 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|workProfilePasswordPreviousPasswordBlockCount|Int32|Число паролей предыдущих рабочих профилей, которые необходимо заблокировать. Допустимые значения: от 0 до 24|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа, разрешенных до удаления профиля работы и удаления всех корпоративных данных. Допустимые значения — от 1 до 16.|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Тип требуемого пароля рабочего профиля. Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileRequirePassword|Логический|Пароль обязателен или не для рабочего профиля|
|securityRequireVerifyApps|Boolean|Обязательное включение функции Android "Проверка приложений".|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
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
  "@odata.type": "microsoft.graph.androidWorkProfileGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "workProfileDataSharingType": "String",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "String",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1024,
  "workProfilePasswordMinimumLength": 1024,
  "workProfilePasswordMinNumericCharacters": 1024,
  "workProfilePasswordMinNonLetterCharacters": 1024,
  "workProfilePasswordMinLetterCharacters": 1024,
  "workProfilePasswordMinLowerCaseCharacters": 1024,
  "workProfilePasswordMinUpperCaseCharacters": 1024,
  "workProfilePasswordMinSymbolCharacters": 1024,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "workProfilePasswordPreviousPasswordBlockCount": 1024,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 1024,
  "workProfilePasswordRequiredType": "String",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```



