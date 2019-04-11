---
title: Тип ресурса windowsPhone81GeneralConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f574701f3da86fe59cb4322315ab273a16d1f0d6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807814"
---
# <a name="windowsphone81generalconfiguration-resource-type"></a>Тип ресурса windowsPhone81GeneralConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windowsPhone81GeneralConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windowsPhone81GeneralConfiguration](../api/intune-deviceconfig-windowsphone81generalconfiguration-list.md)|Коллекция [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md)|Перечисление свойств и связей объектов [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).|
|[Get windowsPhone81GeneralConfiguration](../api/intune-deviceconfig-windowsphone81generalconfiguration-get.md)|[windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md)|Чтение свойств и связей объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).|
|[Создание объекта windowsPhone81GeneralConfiguration](../api/intune-deviceconfig-windowsphone81generalconfiguration-create.md)|[windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md)|Создает объект [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).|
|[Удаление объекта windowsPhone81GeneralConfiguration](../api/intune-deviceconfig-windowsphone81generalconfiguration-delete.md)|Нет|Удаление объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).|
|[Обновление windowsPhone81GeneralConfiguration](../api/intune-deviceconfig-windowsphone81generalconfiguration-update.md)|[windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md)|Обновление свойств объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|applyOnlyToWindowsPhone81|Boolean|Указывает, применяется ли эта политика только к Windows Phone 8.1. Это свойство доступно только для чтения.|
|appsBlockCopyPaste|Boolean|Указывает, следует ли заблокировать копирование данных.|
|bluetoothBlocked|Boolean|Указывает, следует ли заблокировать Bluetooth.|
|cameraBlocked|Boolean|Указывает, следует ли заблокировать камеру.|
|cellularBlockWifiTethering|Boolean|Указывает, следует ли заблокировать модем Wi-Fi. Ни на что не влияет, если Wi-Fi заблокирован.|
|compliantAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType). Эта коллекция может содержать не более 10 000 элементов.|
|compliantAppListType|[Апплисттипе](../resources/intune-deviceconfig-applisttype.md)|Список, указанный с помощью свойства AppComplianceList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|diagnosticDataBlockSubmission|Логический|Указывает, следует ли заблокировать отправку диагностических данных.|
|emailBlockAddingAccounts|Boolean|Указывает, следует ли заблокировать пользовательские учетные записи электронной почты.|
|locationServicesBlocked|Boolean|Указывает, следует ли заблокировать службы определения местоположения.|
|microsoftAccountBlocked|Boolean|Указывает, следует ли запретить использовать учетную запись Майкрософт.|
|nfcBlocked|Логический|Указывает, следует ли заблокировать NFC.|
|passwordBlockSimple|Boolean|Указывает, следует ли заблокировать синхронизацию календаря.|
|passwordExpirationDays|Int32|Количество дней до окончания срока действия пароля.|
|passwordMinimumLength|Int32|Минимальная длина паролей.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые должен содержать пароль.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, которые следует заблокировать. Допустимые значения: от 0 до 24.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек.|
|passwordRequiredType|[Рекуиредпассвордтипе](../resources/intune-deviceconfig-requiredpasswordtype.md)|Необходимый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordRequired|Boolean|Указывает, обязательно ли использовать пароль.|
|screenCaptureBlocked|Boolean|Указывает, следует ли запретить делать снимки экрана.|
|storageBlockRemovableStorage|Boolean|Указывает, следует ли запретить использовать съемные носители.|
|storageRequireEncryption|Boolean|Указывает, обязательно ли шифрование.|
|webBrowserBlocked|Boolean|Указывает, следует ли заблокировать веб-браузер.|
|wifiBlocked|Boolean|Указывает, следует ли заблокировать Wi-Fi.|
|wifiBlockAutomaticConnectHotspots|Boolean|Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi. Ни на что не влияет, если Wi-Fi заблокирован.|
|wifiBlockHotspotReporting|Boolean|Указывает, следует ли запретить устройству сообщать об обнаруженных хот-спотах Wi-Fi. Ни на что не влияет, если Wi-Fi заблокирован.|
|windowsStoreBlocked|Boolean|Указывает, следует ли заблокировать Microsoft Store.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81GeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```





