---
title: Тип ресурса androidDeviceOwnerGeneralDeviceConfiguration
description: В этом разделе описаны объявляемые методы, свойства и связи, предоставляемые ресурсом androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49e70fb573bc9e2a0f66fc4b17b1cc1c53160c55
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572287"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>Тип ресурса androidDeviceOwnerGeneralDeviceConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этом разделе описаны объявляемые методы, свойства и связи, предоставляемые ресурсом androidDeviceOwnerGeneralDeviceConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроиддевицеовнерженералдевицеконфигуратионс](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|Коллекция [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Список свойств и связей объектов [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Получение androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md);|Чтение свойств и связей объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Создание androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md);|Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Удаление androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|Нет|Удаляет объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).|
|[Обновление androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md);|Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Аккаунтсблоккмодификатион|Boolean|Указывает, отключено ли добавление или удаление учетных записей.|
|Аппсалловинсталлфромункновнсаурцес|Boolean|Указывает, может ли пользователь включить параметр "неизвестные источники".|
|Аппсаутаупдатеполици|[Андроиддевицеовнераппаутаупдатеполицитипе](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Указывает значение политики автоматического обновления приложения. Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|Аппсдефаултпермиссионполици|[Андроиддевицеовнердефаултапппермиссионполицитипе](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|Аппсрекоммендскиппингфирстусехинтс|Boolean|Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.|
|Блуетусблоккконфигуратион|Boolean|Указывает, следует ли запретить пользователю настраивать Bluetooth.|
|Блуетусблоккконтактшаринг|Boolean|Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.|
|cameraBlocked|Логический|Указывает, следует ли отключить использование камеры.|
|cellularBlockWiFiTethering|Boolean|Указывает, следует ли заблокировать модем Wi-Fi.|
|Датароамингблоккед|Boolean|Указывает, следует ли запретить пользователю перемещать данные.|
|Датетимеконфигуратионблоккед|Boolean|Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.|
|Факториресетдевицеадминистраторемаилс|Коллекция строк|Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.|
|factoryResetBlocked|Boolean|Указывает, отключен ли параметр Reset фабрики в параметрах.|
|kioskModeApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|Киоскмодеваллпаперурл|String|URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.|
|Киоскмодикситкоде|String|Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.|
|Киоскмодевиртуалхомебуттоненаблед|Boolean|Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.|
|Микрофонефорцемуте|Boolean|Указывает, следует ли запретить разблокирование микрофона устройства.|
|Нетворкескапехатчалловед|Boolean|Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.|
|Нфкблоккаутгоингбеам|Boolean|Указывает, следует ли заблокировать исходящую форму NFC.|
|Пассвордблокккэйгуард|Boolean|Указывает, отключен ли кэйгуард.|
|Пассвордблокккэйгуардфеатурес|Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Список компонентов кэйгуард устройств, которые необходимо заблокировать. Эта коллекция может содержать не более 7 элементов.|
|passwordExpirationDays|Int32|Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль. Допустимые значения: от 1 до 365.|
|passwordMinimumLength|Int32|Указывает минимальную длину пароля, необходимого для устройства. Допустимые значения: от 4 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Миллисекунды бездействия до истечения времени ожидания экрана.|
|Пассвордпревиауспассвордкаунттоблокк|Int32|Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале. Допустимые значения: от 0 до 24.|
|passwordRequiredType|[Андроиддевицеовнеррекуиредпассвордтипе](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Указывает минимальное качество пароля, необходимое для устройства. Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства. Допустимые значения: от 4 до 11.|
|Сафебутблоккед|Boolean|Указывает, отключена ли загрузка устройства в "безопасная загрузка".|
|screenCaptureBlocked|Boolean|Указывает, следует ли отключить возможность использования снимков экрана.|
|Секуритялловдебуггингфеатурес|Boolean|Указывает, следует ли запретить пользователю включать функции отладки на устройстве.|
|securityRequireVerifyApps|Boolean|Указывает, требуется ли проверка приложений.|
|Статусбарблоккед|Boolean|Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.|
|Стайонмодес|Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Список режимов, в которых дисплей устройства остается включенным. Эта коллекция может содержать не более 4 элементов.|
|Сторажеалловусб|Boolean|Указывает, следует ли разрешить запоминающее устройство USB.|
|Сторажеблоккекстерналмедиа|Boolean|Указывает, следует ли заблокировать внешний носитель.|
|Сторажеблоккусбфилетрансфер|Boolean|Указывает, следует ли запретить передачу файлов через USB.|
|Системупдатевиндовстартминутесафтермиднигхт|Int32|Указывает количество минут после полуночи, когда запустится окно обновления системы. Допустимые значения — от 0 до 1440|
|Системупдатевиндовендминутесафтермиднигхт|Int32|Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы. Допустимые значения — от 0 до 1440|
|Системупдатеинсталлтипе|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|Тип конфигурации обновления системы. Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|Системвиндовсблоккед|Boolean|Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.|
|Усерсблоккадд|Boolean|Указывает, отключено ли добавление пользователей и профилей.|
|Усерсблоккремове|Boolean|Указывает, следует ли отключить удаление других пользователей с устройства.|
|Волумеблоккаджустмент|Boolean|Указывает, отключена ли настройка главного тома.|
|Свойства vpnalwaysonpackageidentifier|String|Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.|
|Впналвайсонлоккдовнмоде|Boolean|Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.|
|Вифиблоккедитконфигуратионс|Boolean|Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.|
|Вифиблоккедитполицидефинедконфигуратионс|Boolean|Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.|

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
  "@odata.type": "microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "String",
  "appsDefaultPermissionPolicy": "String",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "String"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "kioskModeWallpaperUrl": "String",
  "kioskModeExitCode": "String",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "String"
  ],
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordCountToBlock": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "String"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 1024,
  "systemUpdateWindowEndMinutesAfterMidnight": 1024,
  "systemUpdateInstallType": "String",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




