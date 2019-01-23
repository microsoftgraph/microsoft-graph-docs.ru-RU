---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93df53db7c19df9134370f9dbd703d99f631b688
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421223"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a>Создание androidDeviceOwnerGeneralDeviceConfiguration

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .

## <a name="prerequisites"></a>Предварительные требования
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление JSON для объекта androidDeviceOwnerGeneralDeviceConfiguration.

В следующей таблице показаны свойства, которые необходимы для создания androidDeviceOwnerGeneralDeviceConfiguration.

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
|accountsBlockModification|Логический|Указывает, отключена ли добавлять и удалять учетные записи.|
|appsAllowInstallFromUnknownSources|Логический|Указывает, может ли пользователь для включения неизвестных источников установки.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Указывает значение политики app автоматическое обновление. Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Указывает политику разрешений для запросов для разрешения среды выполнения, если один не определен для приложения, в частности. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Логический|Рекомендуется все приложения или не пропустить все первого время использования подсказки, которые могут добавлены.|
|bluetoothBlockConfiguration|Логический|Указывает, следует ли запретить пользователю Настройка bluetooth.|
|bluetoothBlockContactSharing|Логический|Указывает, следует ли запретить совместное использование контактов с помощью bluetooth пользователю.|
|cameraBlocked|Логический|Указывает, следует ли отключить использование камеры.|
|cellularBlockWiFiTethering|Boolean|Указывает, следует ли заблокировать модем Wi-Fi.|
|dataRoamingBlocked|Логический|Указывает, следует ли запретить пользователю перемещение данных.|
|dateTimeConfigurationBlocked|Логический|Указывает ли пользователь вручную изменение даты и времени на устройстве|
|factoryResetDeviceAdministratorEmails|Коллекция String|Список Google учетной записи по электронной почте, которые понадобятся для проверки подлинности после фабрики сбросить, прежде чем выполнить настройку устройства.|
|factoryResetBlocked|Boolean|Указывает, отключена ли параметр сброса фабрики в параметрах.|
|kioskModeApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, которые будут отображаться, если устройство находится в полноэкранном режиме. Эта коллекция может содержать не более 500 элементов.|
|kioskModeWallpaperUrl|String|URL-адрес в образ общего доступа для использования для фонового рисунка, когда устройство в полноэкранном режиме.|
|kioskModeExitCode|String|Выйдите из кода, чтобы позволить пользователю для выхода в полноэкранном режиме, когда устройство в полноэкранном режиме.|
|kioskModeVirtualHomeButtonEnabled|Логический|Следует ли отображение виртуальных Домашняя страница кнопки, если устройство находится в полноэкранном режиме.|
|microphoneForceMute|Логический|Указывает, следует ли блокировать выключения звука микрофона на устройстве.|
|networkEscapeHatchAllowed|Логический|Указывает, будет ли устройства разрешить подключение к временной сетевое подключение во время загрузки.|
|nfcBlockOutgoingBeam|Логический|Указывает, следует ли блокировать исходящей балки NFC.|
|passwordBlockKeyguard|Логический|Указывает, отключена ли keyguard.|
|passwordBlockKeyguardFeatures|[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) коллекции|Список компонентов keyguard устройства для блокировки. Эта коллекция может содержать не более 7 элементов. Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.|
|passwordExpirationDays|Int32|Указывает время в секундах, пароль может быть задан для до истечения срока действия и требуется указать новый пароль. Допустимые значения: от 1 до 365.|
|passwordMinimumLength|Int32|Указывает минимальную длину пароля на устройстве. Допустимые значения: от 4 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Простоя перед экрана времени ожидания в миллисекундах.|
|passwordPreviousPasswordCountToBlock|Int32|Длина журнал паролей, где пользователь не сможет ввести новый пароль, которые совпадают с любой пароль в журнале. Допустимые значения: от 0 до 24|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Указывает минимальную качество, необходимые на устройстве. Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Указывает, сколько раз для ввода неправильного пароля перед Очистить устройство. Допустимые значения: от 4 до 11|
|safeBootBlocked|Логический|Указывает, следует ли перезагрузка отключенные устройства в безопасной загрузки.|
|screenCaptureBlocked|Логический|Указывает, следует ли отключить возможность использовать снимки экрана.|
|securityAllowDebuggingFeatures|Логический|Указывает, следует ли пользователь не Включение функции отладки на устройстве.|
|securityRequireVerifyApps|Boolean|Указывает ли проверка приложений является обязательным.|
|statusBarBlocked|Логический|Указывает, будет ли или состояние панели не действует, включая уведомления, параметры быстрого и других перекрытий экрана.|
|stayOnModes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) коллекции|Список режимы, в которых хранятся устройства отображения включении. Эта коллекция может содержать до 4 элементов. Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.|
|storageAllowUsb|Логический|Указывает, следует ли разрешить USB запоминающих устройств.|
|storageBlockExternalMedia|Логический|Указывает, следует ли блокировать внешний носитель.|
|storageBlockUsbFileTransfer|Логический|Указывает, следует ли блокировать USB передачи файлов.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Указывает количество минут после полуночи, начинающимся окно обновление системы. Допустимые значения 0 до 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Указывает количество минут после полуночи, завершающей окне обновление системы. Допустимые значения 0 до 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|Тип обновления конфигурации системы. Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|systemWindowsBlocked|Логический|Блокировать Android системы или не запрашивать пользователя windows, как всплывающие уведомления, phone действия и оповещения системы.|
|usersBlockAdd|Логический|Указывает, отключена ли добавление пользователей и профилей.|
|usersBlockRemove|Логический|Указывает, следует ли отключить удаление других пользователей с устройства.|
|volumeBlockAdjustment|Логический|Указывает, следует ли настройка отключенные громкости.|
|vpnAlwaysOnPackageIdentifier|String|Имя пакета приложения для Android для приложения, которое будет обрабатывать всегда на через VPN.|
|vpnAlwaysOnLockdownMode|Логический|Если всегда на VPN упаковка имя заданной, ли для блокировки сетевого трафика при отключении этого VPN.|
|wifiBlockEditConfigurations|Логический|Указывает, следует ли пользователь не может изменять параметры подключения wifi.|
|wifiBlockEditPolicyDefinedConfigurations|Логический|Указывает, следует ли пользователь не может изменять только что сетей, определенные политикой.|



## <a name="response"></a>Отклик
Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2517

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2689

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




