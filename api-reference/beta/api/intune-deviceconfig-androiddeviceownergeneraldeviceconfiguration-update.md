---
title: Обновление объекта androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1fe2258e1cac3a76d92324b72159fa55583c515a
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670444"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a>Обновление объекта androidDeviceOwnerGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в формате JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|Идентификаторы roleScopeTagId|Коллекция строк|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false и сущности не будут видны пользователям с заданной областью. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удалив и повторно создав политику на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|azureAdSharedDeviceDataClearApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, данные которых будут очищены во время глобального входа в режиме общего устройства AAD. Эта коллекция может содержать не более 500 элементов.|
|accountsBlockModification|Логическое|Указывает, отключено ли добавление или удаление учетных записей.|
|appsAllowInstallFromUnknownSources|Логическое|Указывает, разрешено ли пользователю включить параметр неизвестных источников.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Указывает значение политики автоматического обновления приложения. Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Указывает политику разрешений для запросов на разрешения среды выполнения, если она не определена для конкретного приложения. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Логическое|Следует ли рекомендовать всем приложениям пропускать указания о первом использовании, которые они могли добавить.|
|BluetoothBlockConfiguration|Логическое|Указывает, следует ли запретить пользователю настраивать Bluetooth.|
|BluetoothBlockContactSharing|Логическое|Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.|
|cameraBlocked|Boolean|Указывает, следует ли отключить использование камеры.|
|cellularBlockWiFiTethering|Boolean|Указывает, следует ли заблокировать модем Wi-Fi.|
|CertificateCredentialConfigurationDisabled|Логическое|Указывает, следует ли запретить пользователям какие-либо настройки учетных данных сертификата.|
|crossProfilePoliciesAllowCopyPaste|Логическое|Указывает, можно ли вставить текст, скопированный из одного профиля (личного или рабочего), в другой.|
|crossProfilePoliciesAllowDataSharing|[androidDeviceOwnerCrossProfileDataSharing](../resources/intune-deviceconfig-androiddeviceownercrossprofiledatasharing.md)|Указывает, можно ли совместно использовать данные из одного профиля (личного или рабочего) с приложениями в другом профиле. Возможные значения: `notConfigured`, `crossProfileDataSharingBlocked`, `dataSharingFromWorkToPersonalBlocked`, `crossProfileDataSharingAllowed`, `unkownFutureValue`.|
|crossProfilePoliciesShowWorkContactsInPersonalProfile|Логическое|Указывает, отображаются ли контакты, хранящиеся в рабочем профиле, в личном профиле при поиске контактов или входящих вызовах.|
|microsoftLauncherConfigurationEnabled|Логическое|Указывает, нужно ли настраивать Microsoft Launcher.|
|microsoftLauncherCustomWallpaperEnabled|Логическое|Указывает, следует ли настраивать фоновый рисунок на целевых устройствах.|
|microsoftLauncherCustomWallpaperImageUrl|String|Указывает URL-адрес файла изображения, используемого в качестве фонового рисунка на целевых устройствах.|
|microsoftLauncherCustomWallpaperAllowUserModification|Логическое|Указывает, может ли пользователь изменить фоновый рисунок для персонализации устройства.|
|microsoftLauncherFeedEnabled|Логическое|Указывает, следует ли включить веб-канал запуска на устройстве.|
|microsoftLauncherFeedAllowUserModification|Логическое|Указывает, может ли пользователь изменить веб-канал средства запуска на устройстве.|
|microsoftLauncherDockPresenceConfiguration|[microsoftLauncherDockPresence](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|Указывает, нужно ли настраивать док-станцию устройства. Возможные значения: `notConfigured`, `show`, `hide`, `disabled`.|
|microsoftLauncherDockPresenceAllowUserModification|Логическое|Указывает, может ли пользователь изменить конфигурацию док-станции устройства на устройстве.|
|microsoftLauncherSearchBarPlacementConfiguration|[microsoftLauncherSearchBarPlacement](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|Указывает конфигурацию размещения панели поиска на устройстве. Возможные значения: `notConfigured`, `top`, `bottom`, `hide`.|
|enrollmentProfile|[androidDeviceOwnerEnrollmentProfileType](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|Указывает, какой профиль регистрации необходимо настроить. Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.|
|dataRoamingBlocked|Логическое|Указывает, следует ли запретить пользователю роуминг данных.|
|dateTimeConfigurationBlocked|Логическое|Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.|
|detailedHelpText|[androidDeviceOwnerUserFacingMessage](../resources/intune-deviceconfig-androiddeviceowneruserfacingmessage.md)|Представляет настраиваемый подробный текст справки, предоставленный пользователям при попытке изменить управляемые параметры на устройстве.|
|deviceOwnerLockScreenMessage|[androidDeviceOwnerUserFacingMessage](../resources/intune-deviceconfig-androiddeviceowneruserfacingmessage.md)|Представляет настроенное сообщение экрана блокировки, предоставляемого пользователям при попытке изменить управляемые параметры на устройстве.|
|securityCommonCriteriaModeEnabled|Логическое|Представляет режим общих критериев безопасности, который предоставляется пользователям при попытке изменить управляемые параметры на устройстве.|
|factoryResetDeviceAdministratorEmails|Коллекция String|Список сообщений электронной почты учетной записи Google, которые будут необходимы для проверки подлинности после сброса заводских настроек устройства перед его настройкой.|
|factoryResetBlocked|Boolean|Указывает, отключен ли параметр сброса заводских настроек в параметрах.|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|Прокси-сервер настраивается непосредственно с узлами, портами и исключенными узлами.|
|googleAccountsBlocked|Логический|Указывает, будут ли заблокированы учетные записи Google.|
|kioskCustomizationDeviceSettingsBlocked|Логическое|Указывает, может ли пользователь получить доступ к приложению "Параметры" устройства в режиме киоска.|
|kioskCustomizationPowerButtonActionsBlocked|Логическое|Отображается ли меню питания, когда пользователь долго нажимает кнопку питания устройства в режиме киоска.|
|kioskCustomizationStatusBar|[androidDeviceOwnerKioskCustomizationStatusBar](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|Указывает, отключены ли системные сведения и уведомления в режиме киоска. Возможные значения: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.|
|kioskCustomizationSystemErrorWarnings|Логическое|Указывает, отображаются ли диалоговые окна системных ошибок для приложений, завершившегося сбоем или не отвечая на запросы, в режиме киоска.|
|kioskCustomizationSystemNavigation|[androidDeviceOwnerKioskCustomizationSystemNavigation](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|Указывает, какие функции навигации включены в режиме киоска. Возможные значения: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.|
|kioskModeScreenSaverConfigurationEnabled|Логическое|Следует ли включить режим сохранения экрана или нет в режиме киоска.|
|kioskModeScreenSaverImageUrl|String|URL-адрес изображения, которое будет сохранять экран устройства в режиме киоска.|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|Количество секунд, в течение которых устройство отобразит средство сохранения экрана в режиме киоска. Допустимые значения от 0 до 9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|Время в секундах, в течение которого устройство должно быть неактивным, прежде чем средство сохранения экрана отобразится в режиме киоска. Допустимые значения от 1 до 9999999|
|kioskModeScreenSaverDetectMediaDisabled|Boolean|Указывает, должен ли экран устройства отображать средство сохранения экрана, если звук или видео воспроизводится в режиме киоска.|
|kioskModeApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeWallpaperUrl|String|URL-адрес общедоступного изображения, используемого для фонового рисунка, когда устройство находится в режиме киоска.|
|kioskModeExitCode|String|Код выхода, позволяющий пользователю выйти из режима киоска, когда устройство находится в режиме киоска.|
|kioskModeVirtualHomeButtonEnabled|Логическое|Указывает, следует ли отображать виртуальную домашнюю кнопку, когда устройство находится в режиме киоска.|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|Указывает, является ли виртуальная домашняя кнопка кнопкой прокрутки вверх или плавающей кнопкой дома. Возможные значения: `notConfigured`, `swipeUp`, `floating`.|
|kioskModeBluetoothConfigurationEnabled|Логический|Указывает, разрешено ли пользователю настраивать параметры Bluetooth в режиме киоска.|
|kioskModeWiFiConfigurationEnabled|Логическое|Указывает, следует ли разрешить пользователю настраивать Wi-Fi в режиме киоска.|
|kioskModeFlashlightConfigurationEnabled|Логическое|Указывает, следует ли разрешить пользователю использовать flashlight в режиме киоска.|
|kioskModeMediaVolumeConfigurationEnabled|Логический|Указывает, следует ли разрешить пользователю изменять том мультимедиа в режиме киоска.|
|kioskModeShowDeviceInfo|Логическое|Указывает, следует ли разрешить пользователю доступ к основным сведениям об устройстве.|
|kioskModeManagedSettingsEntryDisabled|Логическое|Указывает, следует ли отображать точку входа управляемых параметров на управляемом начальном экране в режиме киоска.|
|kioskModeDebugMenuEasyAccessEnabled|Логическое|Указывает, следует ли разрешить пользователю простой доступ к меню отладки в режиме киоска.|
|kioskModeShowAppNotificationBadge|Логическое|Указывает, следует ли отображать индикаторы уведомлений приложения в режиме киоска.|
|kioskModeScreenOrientation|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|Настройка ориентации экрана для управляемого начального экрана в режиме киоска. Возможные значения: `notConfigured`, `portrait`, `landscape`, `autoRotate`.|
|kioskModeIconSize|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|Настройка размера значка для управляемого начального экрана в режиме киоска. Возможные значения: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.|
|kioskModeFolderIcon|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|Конфигурация значка папки для управляемого начального экрана в режиме киоска. Возможные значения: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.|
|kioskModeWifiAllowedSsids|Коллекция String|Ограниченный набор идентификаторов SSID WIFI, доступных пользователю для настройки в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeAppOrderEnabled|Логическое|Указывает, следует ли включить упорядочение приложений в режиме киоска.|
|kioskModeAppsInFolderOrderedByName|Логическое|Указывает, следует ли в алфавитном порядке использовать приложения в папке в режиме киоска.|
|kioskModeGridHeight|Int32|Количество строк для сетки Управляемый главный экран с включенным порядком приложений в режиме киоска. Допустимые значения от 1 до 9999999|
|kioskModeGridWidth|Int32|Количество столбцов для Управляемый главный экран с включенным порядком приложений в режиме киоска. Допустимые значения от 1 до 9999999|
|kioskModeLockHomeScreen|Логический|Указывает, следует ли заблокировать начальный экран для конечного пользователя в режиме киоска.|
|kioskModeManagedFolders|[Коллекция androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)|Список управляемых папок для устройства в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeAppPositions|[Коллекция androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)|Порядок элементов в режиме киоска Управляемый главный экран. Эта коллекция может содержать не более 500 элементов.|
|kioskModeManagedHomeScreenAutoSignout|Логическое|Указывает, следует ли автоматически выйти из приложений MHS и режима общего устройства после неактивности для Управляемый главный экран.|
|kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds|Int32|Количество секунд, в течение которого пользователь должен получить уведомление перед автоматическим выходом Управляемый главный экран. Допустимые значения от 0 до 9999999|
|kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds|Int32|Устройство в секундах неактивно перед автоматическим выходом пользователя Управляемый главный экран. Допустимые значения от 0 до 9999999|
|kioskModeManagedHomeScreenPinComplexity|[kioskModeManagedHomeScreenPinComplexity](../resources/intune-deviceconfig-kioskmodemanagedhomescreenpincomplexity.md)|Сложность ПИН-кода для сеанса входа для Управляемый главный экран. Возможные значения: `notConfigured`, `simple`, `complex`.|
|kioskModeManagedHomeScreenPinRequired|Логическое|Указывает, требуется ли пользователю задавать ПИН-код для сеанса входа для Управляемый главный экран.|
|kioskModeManagedHomeScreenPinRequiredToResume|Логическое|Указывает, должен ли пользователь вводить ПИН-код сеанса, если для Управляемый главный экран.|
|kioskModeManagedHomeScreenSignInBackground|String|Фон настраиваемого URL-адреса для экрана входа Управляемый главный экран.|
|kioskModeManagedHomeScreenSignInBrandingLogo|String|Логотип пользовательской фирменной символики URL-адреса для экрана входа и страницы закрепления сеанса для Управляемый главный экран.|
|kioskModeManagedHomeScreenSignInEnabled|Логическое|Указывает, отображается ли экран входа для Управляемый главный экран.|
|kioskModeUseManagedHomeScreenApp|[kioskModeType](../resources/intune-deviceconfig-kioskmodetype.md)|Следует ли использовать режим киоска с одним приложением или режим киоска с несколькими приложениями. Возможные значения: `notConfigured`, `singleAppMode`, `multiAppMode`.|
|microphoneForceMute|Логический|Указывает, следует ли блокировать отключение микрофона на устройстве.|
|networkEscapeHatchAllowed|Логическое|Указывает, разрешает ли устройство подключаться к временному сетевому подключению во время загрузки.|
|nfcBlockOutgoingBeam|Логическое|Указывает, следует ли блокировать исходящий луч NFC.|
|passwordBlockKeyguard|Логический|Указывает, отключен ли keyguard.|
|passwordBlockKeyguardFeatures|[Коллекция androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Список функций keyguard устройства для блокировки. Эта коллекция может содержать не более 7 элементов. Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`, `face`, `iris`, `biometrics`.|
|passwordExpirationDays|Int32|Указывает время, в течение которого пароль может быть задано до истечения срока его действия, и потребуется новый пароль. Допустимые значения: от 1 до 365.|
|passwordMinimumLength|Int32|Указывает минимальную длину пароля, необходимого на устройстве. Допустимые значения: от 4 до 16.|
|passwordMinimumLetterCharacters|Int32|Указывает минимальное количество букв, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumLowerCaseCharacters|Int32|Указывает минимальное количество символов нижнего регистра, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumNonLetterCharacters|Int32|Указывает минимальное количество небуквенные символы, необходимые для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumNumericCharacters|Int32|Указывает минимальное количество числовых символов, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumSymbolCharacters|Int32|Указывает минимальное количество символов, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumUpperCaseCharacters|Int32|Указывает минимальное количество символов прописных букв, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passwordPreviousPasswordCountToBlock|Int32|Указывает длину журнала паролей, где пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале. Допустимые значения: от 0 до 24.|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Указывает минимальное качество пароля, необходимое на устройстве. Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|
|passwordRequireUnlock|[androidDeviceOwnerRequiredPasswordUnlock](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordunlock.md)|Указывает период времени ожидания, по истечении которого устройство должно быть разблокировано с помощью строгой проверки подлинности. Возможные значения: `deviceDefault`, `daily`, `unkownFutureValue`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Указывает, сколько раз пользователь может ввести неправильный пароль перед очисткой устройства. Допустимые значения: от 4 до 11.|
|playStoreMode|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|Указывает режим магазина воспроизведения устройства. Возможные значения: `notConfigured`, `allowList`, `blockList`.|
|screenCaptureBlocked|Boolean|Указывает, следует ли отключить возможность создания снимков экрана.|
|securityDeveloperSettingsEnabled|Boolean|Указывает, разрешен ли пользователю доступ к параметрам разработчика, таким как параметры разработчика и безопасная загрузка на устройстве.|
|securityRequireVerifyApps|Boolean|Указывает, требуются ли приложения.|
|shortHelpText|[androidDeviceOwnerUserFacingMessage](../resources/intune-deviceconfig-androiddeviceowneruserfacingmessage.md)|Представляет настраиваемый короткий текст справки, предоставленный пользователям при попытке изменить управляемые параметры на устройстве.|
|statusBarBlocked|Логическое|Указывает, отключена ли строка состояния, включая уведомления, быстрые параметры и другие наложения экрана.|
|stayOnModes|[Коллекция androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Список режимов, в которых экран устройства будет оставаться активным. Эта коллекция может содержать не более 4 элементов. Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.|
|storageAllowUsb|Логический|Указывает, следует ли разрешить usb-накопитель.|
|storageBlockExternalMedia|Логическое|Указывает, следует ли блокировать внешний носитель.|
|storageBlockUsbFileTransfer|Логическое|Указывает, следует ли блокировать передачу USB-файлов.|
|systemUpdateFreezePeriods|[Коллекция androidDeviceOwnerSystemUpdateFreezePeriod](../resources/intune-deviceconfig-androiddeviceownersystemupdatefreezeperiod.md)|Указывает периоды времени, повторяющиеся ежегодно, в течение которых обновления системы откладываются. Эта коллекция может содержать не более 500 элементов.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Указывает количество минут после полуночи, в течение которых запускается окно обновления системы. Допустимые значения от 0 до 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Указывает количество минут после полуночи, в течение которых заканчивается окно обновления системы. Допустимые значения от 0 до 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|Тип конфигурации обновления системы. Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|systemWindowsBlocked|Логический|Следует ли блокировать окна системных запросов Android, такие как всплывающие уведомления, действия с телефоном и системные оповещения.|
|usersBlockAdd|Логическое|Указывает, отключено ли добавление пользователей и профилей.|
|usersBlockRemove|Логическое|Указывает, следует ли отключить удаление других пользователей с устройства.|
|volumeBlockAdjustment|Логическое|Указывает, отключена ли настройка главного тома.|
|VpnAlwaysOnLockdownMode|Логическое|Если указано имя пакета VPN always on, следует ли блокировать сетевой трафик при отключении vpn.|
|vpnAlwaysOnPackageIdentifier|String|Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.|
|WifiBlockEditConfigurations|Boolean|Указывает, следует ли запретить пользователю изменять параметры подключения Wi-Fi.|
|WifiBlockEditPolicyDefinedConfigurations|Логическое|Указывает, следует ли запретить пользователю изменять только сети, определенные политикой.|
|personalProfileAppsAllowInstallFromUnknownSources|Логическое|Указывает, может ли пользователь устанавливать приложения из неизвестных источников в личном профиле.|
|personalProfileCameraBlocked|Логическое|Указывает, следует ли отключить использование камеры в личном профиле.|
|personalProfileScreenCaptureBlocked|Логическое|Указывает, следует ли отключить возможность создания снимков экрана в личном профиле.|
|personalProfilePlayStoreMode|[personalProfilePersonalPlayStoreMode](../resources/intune-deviceconfig-personalprofilepersonalplaystoremode.md)|Используется вместе с PersonalProfilePersonalApplications для управления тем, как приложения в личном профиле разрешены или заблокированы. Возможные значения: `notConfigured`, `blockedApps`, `allowedApps`.|
|personalProfilePersonalApplications|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Политика, применяемая к приложениям в личном профиле. Эта коллекция может содержать не более 500 элементов.|
|workProfilePasswordExpirationDays|Int32|Указывает количество дней, в течение которых можно задать пароль рабочего профиля до истечения срока его действия, и потребуется новый пароль. Допустимые значения: от 1 до 365.|
|workProfilePasswordMinimumLength|Int32|Указывает минимальную длину пароля рабочего профиля. Допустимые значения: от 4 до 16.|
|workProfilePasswordMinimumNumericCharacters|Int32|Указывает минимальное число числовых символов, необходимое для пароля рабочего профиля. Допустимые значения от 1 до 16|
|workProfilePasswordMinimumNonLetterCharacters|Int32|Указывает минимальное количество небуквенные символы, необходимые для пароля рабочего профиля. Допустимые значения от 1 до 16|
|workProfilePasswordMinimumLetterCharacters|Int32|Указывает минимальное количество букв, необходимых для пароля рабочего профиля. Допустимые значения от 1 до 16|
|workProfilePasswordMinimumLowerCaseCharacters|Int32|Указывает минимальное количество символов нижнего регистра, необходимых для пароля рабочего профиля. Допустимые значения от 1 до 16|
|WorkProfilePasswordMinimumUpperCaseCharacters|Int32|Указывает минимальное количество символов прописных букв, необходимых для пароля рабочего профиля. Допустимые значения от 1 до 16|
|workProfilePasswordMinimumSymbolCharacters|Int32|Указывает минимальное количество символов, необходимых для пароля рабочего профиля. Допустимые значения от 1 до 16|
|workProfilePasswordPreviousPasswordCountToBlock|Int32|Указывает длину журнала паролей рабочего профиля, где пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале. Допустимые значения: от 0 до 24.|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Указывает, сколько раз пользователь может ввести неправильный пароль рабочего профиля перед очисткой устройства. Допустимые значения: от 4 до 11.|
|WorkProfilePasswordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Указывает минимальное качество пароля, необходимое для пароля рабочего профиля. Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|
|workProfilePasswordRequireUnlock|[androidDeviceOwnerRequiredPasswordUnlock](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordunlock.md)|Указывает период времени ожидания, по истечении которого рабочий профиль должен быть разблокирован с помощью строгой проверки подлинности. Возможные значения: `deviceDefault`, `daily`, `unkownFutureValue`.|



## <a name="response"></a>Отклик
В случае успешного `200 OK` выполнения этот метод возвращает код отклика и обновленный объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 10090

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureAdSharedDeviceDataClearApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "crossProfilePoliciesAllowCopyPaste": true,
  "crossProfilePoliciesAllowDataSharing": "crossProfileDataSharingBlocked",
  "crossProfilePoliciesShowWorkContactsInPersonalProfile": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "detailedHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "deviceOwnerLockScreenMessage": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "securityCommonCriteriaModeEnabled": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
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
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
  ],
  "kioskModeManagedHomeScreenAutoSignout": true,
  "kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds": 7,
  "kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds": 8,
  "kioskModeManagedHomeScreenPinComplexity": "simple",
  "kioskModeManagedHomeScreenPinRequired": true,
  "kioskModeManagedHomeScreenPinRequiredToResume": true,
  "kioskModeManagedHomeScreenSignInBackground": "Kiosk Mode Managed Home Screen Sign In Background value",
  "kioskModeManagedHomeScreenSignInBrandingLogo": "Kiosk Mode Managed Home Screen Sign In Branding Logo value",
  "kioskModeManagedHomeScreenSignInEnabled": true,
  "kioskModeUseManagedHomeScreenApp": "singleAppMode",
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordRequireUnlock": "daily",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "screenCaptureBlocked": true,
  "securityDeveloperSettingsEnabled": true,
  "securityRequireVerifyApps": true,
  "shortHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateFreezePeriods": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod",
      "startMonth": 10,
      "startDay": 8,
      "endMonth": 8,
      "endDay": 6
    }
  ],
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "personalProfilePlayStoreMode": "blockedApps",
  "personalProfilePersonalApplications": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required",
  "workProfilePasswordRequireUnlock": "daily"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10262

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureAdSharedDeviceDataClearApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "crossProfilePoliciesAllowCopyPaste": true,
  "crossProfilePoliciesAllowDataSharing": "crossProfileDataSharingBlocked",
  "crossProfilePoliciesShowWorkContactsInPersonalProfile": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "detailedHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "deviceOwnerLockScreenMessage": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "securityCommonCriteriaModeEnabled": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
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
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
  ],
  "kioskModeManagedHomeScreenAutoSignout": true,
  "kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds": 7,
  "kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds": 8,
  "kioskModeManagedHomeScreenPinComplexity": "simple",
  "kioskModeManagedHomeScreenPinRequired": true,
  "kioskModeManagedHomeScreenPinRequiredToResume": true,
  "kioskModeManagedHomeScreenSignInBackground": "Kiosk Mode Managed Home Screen Sign In Background value",
  "kioskModeManagedHomeScreenSignInBrandingLogo": "Kiosk Mode Managed Home Screen Sign In Branding Logo value",
  "kioskModeManagedHomeScreenSignInEnabled": true,
  "kioskModeUseManagedHomeScreenApp": "singleAppMode",
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordRequireUnlock": "daily",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "screenCaptureBlocked": true,
  "securityDeveloperSettingsEnabled": true,
  "securityRequireVerifyApps": true,
  "shortHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "defaultMessage": "Default Message value"
  },
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateFreezePeriods": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod",
      "startMonth": 10,
      "startDay": 8,
      "endMonth": 8,
      "endDay": 6
    }
  ],
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "personalProfilePlayStoreMode": "blockedApps",
  "personalProfilePersonalApplications": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required",
  "workProfilePasswordRequireUnlock": "daily"
}
```




