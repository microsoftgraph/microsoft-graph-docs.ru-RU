---
title: Тип ресурса androidDeviceOwnerGeneralDeviceConfiguration
description: В этом разделе описаны объявляемые методы, свойства и связи, предоставляемые ресурсом androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ea9c2d0d344833a45c3f112f1f0af8d7d5ffb00d
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163670"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>Тип ресурса androidDeviceOwnerGeneralDeviceConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этом разделе описаны объявляемые методы, свойства и связи, предоставляемые ресурсом androidDeviceOwnerGeneralDeviceConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

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
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|аккаунтсблоккмодификатион|Boolean|Указывает, отключено ли добавление или удаление учетных записей.|
|аппсалловинсталлфромункновнсаурцес|Boolean|Указывает, может ли пользователь включить параметр "неизвестные источники".|
|аппсаутаупдатеполици|[андроиддевицеовнераппаутаупдатеполицитипе](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Указывает значение политики автоматического обновления приложения. Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|аппсдефаултпермиссионполици|[андроиддевицеовнердефаултапппермиссионполицитипе](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|аппсрекоммендскиппингфирстусехинтс|Boolean|Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.|
|блуетусблоккконфигуратион|Boolean|Указывает, следует ли запретить пользователю настраивать Bluetooth.|
|блуетусблоккконтактшаринг|Boolean|Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.|
|cameraBlocked|Логический|Указывает, следует ли отключить использование камеры.|
|cellularBlockWiFiTethering|Boolean|Указывает, следует ли заблокировать модем Wi-Fi.|
|цертификатекредентиалконфигуратиондисаблед|Boolean|Указывает, следует ли запретить пользователям настраивать учетные данные сертификатов.|
|датароамингблоккед|Boolean|Указывает, следует ли запретить пользователю перемещать данные.|
|датетимеконфигуратионблоккед|Boolean|Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.|
|факториресетдевицеадминистраторемаилс|Коллекция строк|Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.|
|factoryResetBlocked|Boolean|Указывает, отключен ли параметр Reset фабрики в параметрах.|
|глобалпрокси|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.|
|гуглеаккаунтсблоккед|Boolean|Указывает, будут ли блокироваться учетные записи Google.|
|киоскмодескринсаверконфигуратионенаблед|Boolean|Указывает, следует ли включить режим экранной заставки или не в режиме киоска.|
|киоскмодескринсаверимажеурл|String|URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.|
|киоскмодескринсавердисплайтимеинсекондс|Int32|Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска. Допустимые значения — от 0 до 9999999|
|киоскмодескринсаверстартделайинсекондс|Int32|Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска. Допустимые значения — от 1 до 9999999|
|киоскмодескринсавердетектмедиадисаблед|Boolean|Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.|
|kioskModeApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|киоскмодеваллпаперурл|String|URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.|
|киоскмодикситкоде|String|Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.|
|киоскмодевиртуалхомебуттоненаблед|Boolean|Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.|
|киоскмодевиртуалхомебуттонтипе|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой". Возможные значения: `notConfigured`, `swipeUp`, `floating`.|
|киоскмодеблуетусконфигуратионенаблед|Boolean|Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.|
|киоскмодевификонфигуратионенаблед|Boolean|Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.|
|киоскмодефлашлигхтконфигуратионенаблед|Boolean|Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.|
|киоскмодемедиаволумеконфигуратионенаблед|Boolean|Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.|
|микрофонефорцемуте|Boolean|Указывает, следует ли запретить разблокирование микрофона устройства.|
|нетворкескапехатчалловед|Boolean|Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.|
|нфкблоккаутгоингбеам|Boolean|Указывает, следует ли заблокировать исходящую форму NFC.|
|пассвордблокккэйгуард|Boolean|Указывает, отключен ли кэйгуард.|
|пассвордблокккэйгуардфеатурес|Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Список компонентов кэйгуард устройств, которые необходимо заблокировать. Эта коллекция может содержать не более 7 элементов.|
|passwordExpirationDays|Int32|Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль. Допустимые значения: от 1 до 365.|
|passwordMinimumLength|Int32|Указывает минимальную длину пароля, необходимого для устройства. Допустимые значения: от 4 до 16.|
|пассвордминимумлеттерчарактерс|Int32|Указывает минимальное число символов, необходимых для пароля устройства. Допустимые значения — от 1 до 16.|
|пассвордминимумловеркасечарактерс|Int32|Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства. Допустимые значения — от 1 до 16.|
|пассвордминимумнонлеттерчарактерс|Int32|Указывает минимальное количество небуквенных символов, необходимых для пароля устройства. Допустимые значения — от 1 до 16.|
|пассвордминимумнумерикчарактерс|Int32|Указывает минимальное количество числовых символов, необходимое для пароля устройства. Допустимые значения — от 1 до 16.|
|пассвордминимумсимболчарактерс|Int32|Указывает минимальное число символов, необходимых для пароля устройства. Допустимые значения — от 1 до 16.|
|пассвордминимумупперкасечарактерс|Int32|Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства. Допустимые значения — от 1 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Миллисекунды бездействия до истечения времени ожидания экрана.|
|пассвордпревиауспассвордкаунттоблокк|Int32|Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале. Допустимые значения: от 0 до 24.|
|passwordRequiredType|[андроиддевицеовнеррекуиредпассвордтипе](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Указывает минимальное качество пароля, необходимое для устройства. Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства. Допустимые значения: от 4 до 11.|
|плайсторемоде|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|Указывает режим проигрывания устройства в хранилище. Возможные значения: `notConfigured`, `allowList`, `blockList`.|
|сафебутблоккед|Boolean|Указывает, отключена ли загрузка устройства в "безопасная загрузка".|
|screenCaptureBlocked|Boolean|Указывает, следует ли отключить возможность использования снимков экрана.|
|секуритялловдебуггингфеатурес|Boolean|Указывает, следует ли запретить пользователю включать функции отладки на устройстве.|
|securityRequireVerifyApps|Boolean|Указывает, требуется ли проверка приложений.|
|статусбарблоккед|Boolean|Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.|
|стайонмодес|Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Список режимов, в которых дисплей устройства остается включенным. Эта коллекция может содержать не более 4 элементов.|
|сторажеалловусб|Boolean|Указывает, следует ли разрешить запоминающее устройство USB.|
|сторажеблоккекстерналмедиа|Boolean|Указывает, следует ли заблокировать внешний носитель.|
|сторажеблоккусбфилетрансфер|Boolean|Указывает, следует ли запретить передачу файлов через USB.|
|системупдатевиндовстартминутесафтермиднигхт|Int32|Указывает количество минут после полуночи, когда запустится окно обновления системы. Допустимые значения — от 0 до 1440|
|системупдатевиндовендминутесафтермиднигхт|Int32|Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы. Допустимые значения — от 0 до 1440|
|системупдатеинсталлтипе|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|Тип конфигурации обновления системы. Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|системвиндовсблоккед|Boolean|Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.|
|усерсблоккадд|Boolean|Указывает, отключено ли добавление пользователей и профилей.|
|усерсблоккремове|Boolean|Указывает, следует ли отключить удаление других пользователей с устройства.|
|волумеблоккаджустмент|Boolean|Указывает, отключена ли настройка главного тома.|
|впналвайсонлоккдовнмоде|Boolean|Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.|
|Свойства vpnalwaysonpackageidentifier|String|Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.|
|вифиблоккедитконфигуратионс|Boolean|Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.|
|вифиблоккедитполицидефинедконфигуратионс|Boolean|Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|

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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "String",
  "appsDefaultPermissionPolicy": "String",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "String"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "String"
  },
  "googleAccountsBlocked": true,
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "String",
  "kioskModeScreenSaverDisplayTimeInSeconds": 1024,
  "kioskModeScreenSaverStartDelayInSeconds": 1024,
  "kioskModeScreenSaverDetectMediaDisabled": true,
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
  "kioskModeVirtualHomeButtonType": "String",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "String"
  ],
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumLetterCharacters": 1024,
  "passwordMinimumLowerCaseCharacters": 1024,
  "passwordMinimumNonLetterCharacters": 1024,
  "passwordMinimumNumericCharacters": 1024,
  "passwordMinimumSymbolCharacters": 1024,
  "passwordMinimumUpperCaseCharacters": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordCountToBlock": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "playStoreMode": "String",
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
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```



