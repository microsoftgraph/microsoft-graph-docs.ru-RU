---
title: тип ресурса androidWorkProfileGeneralDeviceConfiguration
description: Общая конфигурация устройства профиля android work.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aaac8d4342f5a1d019c57b946c9eb0b9feb832ab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148028"
---
# <a name="androidworkprofilegeneraldeviceconfiguration-resource-type"></a>тип ресурса androidWorkProfileGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Общая конфигурация устройства профиля android work.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список androidWorkProfileGeneralDeviceConfigurations](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-list.md)|[коллекция androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|Список свойств и связей объектов [AndroidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|
|[Get AndroidWorkProfileGeneralDeviceConfiguration](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-get.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|Чтение свойств и связей [объекта AndroidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|
|[Создание androidWorkProfileGeneralDeviceConfiguration](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-create.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|Создайте новый [объект AndroidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|
|[Удаление androidWorkProfileGeneralDeviceConfiguration](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-delete.md)|Нет|Удаляет [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).|
|[Обновление androidWorkProfileGeneralDeviceConfiguration](../api/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration-update.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|Обновление свойств объекта [AndroidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция объектов string|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|passwordBlockFaceUnlock|Логическое|Указывает, следует ли блокировать разблокирование лица.|
|passwordBlockFingerprintUnlock|Boolean|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passwordBlockIrisUnlock|Логический|Указывает, следует ли блокировать разблокировку радужной оболочки радужной оболочки.|
|passwordBlockTrustAgents|Boolean|Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.|
|passwordExpirationDays|Int32|Количество дней до окончания срока действия пароля. Допустимые значения: от 1 до 365.|
|passwordMinimumLength|Int32|Минимальная длина паролей. Допустимые значения: от 4 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, которые следует заблокировать. Допустимые значения: от 0 до 24.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек. Допустимые значения от 1 до 16|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileAllowAppInstallsFromUnknownSources|Логическое|Указывает, следует ли разрешить установку приложений из неизвестных источников.|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|Тип разрешенного обмена данными. Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.|
|workProfileBlockNotificationsWhileDeviceLocked|Логическое|Указывает, следует ли блокировать уведомления во время блокировки устройства.|
|workProfileBlockAddingAccounts|Логическое|Блокировать добавление и удаление учетных записей в профиле работы.|
|workProfileBluetoothEnableContactSharing|Логический|Разрешить устройствам Bluetooth доступ к корпоративным контактам.|
|workProfileBlockScreenCapture|Логический|Блокировка захвата экрана в профиле работы.|
|workProfileBlockCrossProfileCallerId|Логическое|Блокировка ИД вызываемой личности вызываемой на экране работы в личном профиле.|
|workProfileBlockCamera|Логическое|Блокировка камеры профиля работы.|
|workProfileBlockCrossProfileContactsSearch|Логический|Блокировка доступности контактов профилей работы в личном профиле.|
|workProfileBlockCrossProfileCopyPaste|Логическое|Boolean, который указывает, включен ли параметр, который не позволяет копировать/вклеить перекрестный профиль.|
|workProfileDefaultAppPermissionPolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|workProfilePasswordBlockFaceUnlock|Логический|Указывает, следует ли блокировать разблокировку лица для профиля работы.|
|workProfilePasswordBlockFingerprintUnlock|Логический|Указывает, следует ли блокировать разблокировку отпечатков пальцев для профиля работы.|
|workProfilePasswordBlockIrisUnlock|Логическое|Указывает, следует ли блокировать разблокировку радужной оболочки радужной оболочки для профиля работы.|
|workProfilePasswordBlockTrustAgents|Логическое|Указывает, следует ли блокировать Smart Lock и другие агенты доверия для профиля работы.|
|workProfilePasswordExpirationDays|Int32|Количество дней до истечения срока действия пароля профиля работы. Допустимые значения: от 1 до 365.|
|workProfilePasswordMinimumLength|Int32|Минимальная длина пароля профиля работы. Допустимые значения: от 4 до 16.|
|workProfilePasswordMinNumericCharacters|Int32|Минимум # числимые символы, необходимые в пароле профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinNonLetterCharacters|Int32|Минимальное количество символов без букв, необходимых в пароле профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinLetterCharacters|Int32|Минимальный # буквы символов, необходимых в пароле профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinLowerCaseCharacters|Int32|Минимальное количество символов нижнего уровня, необходимых для пароля профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinUpperCaseCharacters|Int32|Минимальный # символов верхнего уровня, необходимых в пароле профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinSymbolCharacters|Int32|Минимальный # символов, необходимых в пароле профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|workProfilePasswordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей профилей работы для блокировки. Допустимые значения: от 0 до 24.|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Количество входов в сбои, разрешенные до удаления профиля работы и удаления всех корпоративных данных. Допустимые значения от 1 до 16|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Тип необходимого пароля профиля работы. Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileRequirePassword|Логический|Пароль требуется или не требуется для профиля работы|
|securityRequireVerifyApps|Boolean|Указывает, что требуется включить функцию проверки приложений для Android.|
|vpnAlwaysOnPackageIdentifier|String|Включить режим блокировки для всегда на VPN.|
|VPNEnableAlwaysOnLockdownMode|Логическое|Включить режим блокировки для всегда на VPN.|
|workProfileAllowWidgets|Логическое|Разрешить виджеты из приложений профиля работы.|
|workProfileBlockPersonalAppInstallsFromUnknownSources|Логический|Предотвращение установок приложений из неизвестных источников в личном профиле.|

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
  "@odata.type": "microsoft.graph.androidWorkProfileGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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
  "passwordBlockFaceUnlock": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockIrisUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "workProfileAllowAppInstallsFromUnknownSources": true,
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
  "workProfilePasswordBlockFaceUnlock": true,
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockIrisUnlock": true,
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
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```



