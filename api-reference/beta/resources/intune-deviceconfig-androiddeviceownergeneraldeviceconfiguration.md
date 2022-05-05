---
title: Тип ресурса androidDeviceOwnerGeneralDeviceConfiguration
description: В этом разделе приводятся описания объявленных методов, свойств и связей, предоставляемых ресурсом androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c20d7b658362ca5f05d79e6450019dc06c48fbe3
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203227"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>Тип ресурса androidDeviceOwnerGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этом разделе приводятся описания объявленных методов, свойств и связей, предоставляемых ресурсом androidDeviceOwnerGeneralDeviceConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[Коллекция androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Список свойств и связей объектов [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Получение объекта androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md);|Чтение свойств и связей объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Создание объекта androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md);|Создайте объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Удаление объекта androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|Нет|Удаляет объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).|
|[Обновление объекта androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md);|Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|

## <a name="properties"></a>Свойства
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
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|azureAdSharedDeviceDataClearApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, данные которых будут удалены во время глобального входа в AAD режиме общего устройства. Эта коллекция может содержать не более 500 элементов.|
|accountsBlockModification|Логический|Указывает, отключено ли добавление или удаление учетных записей.|
|appsAllowInstallFromUnknownSources|Логическое|Указывает, разрешено ли пользователю включить параметр неизвестных источников.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Указывает значение политики автоматического обновления приложения. Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Указывает политику разрешений для запросов на разрешения среды выполнения, если она не определена для конкретного приложения. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Логический|Следует ли рекомендовать всем приложениям пропускать указания о первом использовании, которые они могли добавить.|
|BluetoothBlockConfiguration|Логическое|Указывает, следует ли запретить пользователю настраивать Bluetooth.|
|BluetoothBlockContactSharing|Логическое|Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.|
|cameraBlocked|Boolean|Указывает, следует ли отключить использование камеры.|
|cellularBlockWiFiTethering|Boolean|Указывает, следует ли заблокировать модем Wi-Fi.|
|CertificateCredentialConfigurationDisabled|Логическое|Указывает, следует ли запретить пользователям какие-либо настройки учетных данных сертификата.|
|crossProfilePoliciesAllowCopyPaste|Логический|Указывает, можно ли вставить текст, скопированный из одного профиля (личного или рабочего), в другой.|
|crossProfilePoliciesAllowDataSharing|[androidDeviceOwnerCrossProfileDataSharing](../resources/intune-deviceconfig-androiddeviceownercrossprofiledatasharing.md)|Указывает, можно ли совместно использовать данные из одного профиля (личного или рабочего) с приложениями в другом профиле. Возможные значения: `notConfigured`, `crossProfileDataSharingBlocked`, `dataSharingFromWorkToPersonalBlocked`, `crossProfileDataSharingAllowed`, `unkownFutureValue`.|
|crossProfilePoliciesShowWorkContactsInPersonalProfile|Логическое|Указывает, отображаются ли контакты, хранящиеся в рабочем профиле, в личном профиле при поиске контактов или входящих вызовах.|
|microsoftLauncherConfigurationEnabled|Логическое|Указывает, нужно ли настраивать Microsoft Launcher.|
|microsoftLauncherCustomWallpaperEnabled|Логическое|Указывает, следует ли настраивать фоновый рисунок на целевых устройствах.|
|microsoftLauncherCustomWallpaperImageUrl|Строка|Указывает URL-адрес файла изображения, используемого в качестве фонового рисунка на целевых устройствах.|
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
|factoryResetDeviceAdministratorEmails|Коллекция String|Список сообщений электронной почты учетной записи Google, которые будут необходимы для проверки подлинности после сброса заводских настроек устройства перед его настройкой.|
|factoryResetBlocked|Boolean|Указывает, отключен ли параметр сброса заводских настроек в параметрах.|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|Прокси-сервер настраивается непосредственно с узлами, портами и исключенными узлами.|
|googleAccountsBlocked|Логический|Указывает, будут ли заблокированы учетные записи Google.|
|kioskCustomizationDeviceSettingsBlocked|Логическое|Указывает, может ли пользователь получить доступ к приложению Параметры устройства в режиме киоска.|
|kioskCustomizationPowerButtonActionsBlocked|Логическое|Отображается ли меню питания, когда пользователь долго нажимает кнопку питания устройства в режиме киоска.|
|kioskCustomizationStatusBar|[androidDeviceOwnerKioskCustomizationStatusBar](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|Указывает, отключены ли системные сведения и уведомления в режиме киоска. Возможные значения: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.|
|kioskCustomizationSystemErrorWarnings|Логическое|Указывает, отображаются ли диалоговые окна системных ошибок для приложений, завершившегося сбоем или не отвечая на запросы, в режиме киоска.|
|kioskCustomizationSystemNavigation|[androidDeviceOwnerKioskCustomizationSystemNavigation](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|Указывает, какие функции навигации включены в режиме киоска. Возможные значения: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.|
|kioskModeScreenSaverConfigurationEnabled|Логическое|Следует ли включить режим сохранения экрана или нет в режиме киоска.|
|kioskModeScreenSaverImageUrl|Строка|URL-адрес изображения, которое будет сохранять экран устройства в режиме киоска.|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|Количество секунд, в течение которых устройство отобразит средство сохранения экрана в режиме киоска. Допустимые значения от 0 до 9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|Время в секундах, в течение которого устройство должно быть неактивным, прежде чем средство сохранения экрана отобразится в режиме киоска. Допустимые значения от 1 до 9999999|
|kioskModeScreenSaverDetectMediaDisabled|Логическое|Указывает, должен ли экран устройства отображать средство сохранения экрана, если звук или видео воспроизводится в режиме киоска.|
|kioskModeApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeWallpaperUrl|Строка|URL-адрес общедоступного изображения, используемого для фонового рисунка, когда устройство находится в режиме киоска.|
|kioskModeExitCode|Строка|Код выхода, позволяющий пользователю выйти из режима киоска, когда устройство находится в режиме киоска.|
|kioskModeVirtualHomeButtonEnabled|Логическое|Указывает, следует ли отображать виртуальную домашнюю кнопку, когда устройство находится в режиме киоска.|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|Указывает, является ли виртуальная домашняя кнопка кнопкой прокрутки вверх или плавающей кнопкой дома. Возможные значения: `notConfigured`, `swipeUp`, `floating`.|
|kioskModeBluetoothConfigurationEnabled|Логическое|Указывает, следует ли разрешить пользователю настраивать Bluetooth в режиме киоска.|
|kioskModeWiFiConfigurationEnabled|Логическое|Указывает, следует ли разрешить пользователю настраивать Wi-Fi в режиме киоска.|
|kioskModeFlashlightConfigurationEnabled|Логическое|Указывает, следует ли разрешить пользователю использовать flashlight в режиме киоска.|
|kioskModeMediaVolumeConfigurationEnabled|Логическое|Указывает, следует ли разрешить пользователю изменять том мультимедиа в режиме киоска.|
|kioskModeShowDeviceInfo|Логический|Указывает, следует ли разрешить пользователю доступ к основным сведениям об устройстве.|
|kioskModeManagedSettingsEntryDisabled|Логическое|Указывает, следует ли отображать управляемую Параметры точку входа на управляемом начальном экране в режиме киоска.|
|kioskModeDebugMenuEasyAccessEnabled|Логическое|Указывает, следует ли разрешить пользователю простой доступ к меню отладки в режиме киоска.|
|kioskModeShowAppNotificationBadge|Логическое|Указывает, следует ли отображать индикаторы уведомлений приложения в режиме киоска.|
|kioskModeScreenOrientation|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|Настройка ориентации экрана для управляемого начального экрана в режиме киоска. Возможные значения: `notConfigured`, `portrait`, `landscape`, `autoRotate`.|
|kioskModeIconSize|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|Настройка размера значка для управляемого начального экрана в режиме киоска. Возможные значения: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.|
|kioskModeFolderIcon|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|Конфигурация значка папки для управляемого начального экрана в режиме киоска. Возможные значения: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.|
|kioskModeWifiAllowedSsids|Коллекция объектов string|Ограниченный набор идентификаторов SSID WIFI, доступных пользователю для настройки в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeAppOrderEnabled|Логическое|Указывает, следует ли включить упорядочение приложений в режиме киоска.|
|kioskModeAppsInFolderOrderedByName|Логическое|Указывает, следует ли в алфавитном порядке использовать приложения в папке в режиме киоска.|
|kioskModeGridHeight|Int32|Количество строк для сетки управляемого начального экрана с включенным порядком приложений в режиме киоска. Допустимые значения от 1 до 9999999|
|kioskModeGridWidth|Int32|Количество столбцов для сетки управляемого начального экрана с включенным порядком приложений в режиме киоска. Допустимые значения от 1 до 9999999|
|kioskModeLockHomeScreen|Логический|Указывает, следует ли заблокировать начальный экран для конечного пользователя в режиме киоска.|
|kioskModeManagedFolders|[Коллекция androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)|Список управляемых папок для устройства в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeAppPositions|[Коллекция androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)|Порядок элементов на управляемом начальном экране режима киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeManagedHomeScreenAutoSignout|Логическое|Указывает, следует ли автоматически выйти из приложений MHS и общего режима устройства после неактивности для управляемого начального экрана.|
|kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds|Int32|Количество секунд, в течение которого пользователь должен получить уведомление перед автоматическим выходом на управляемый начальный экран. Допустимые значения от 0 до 9999999|
|kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds|Int32|Устройство в секундах неактивно перед автоматическим выходом пользователя на управляемый начальный экран. Допустимые значения от 0 до 9999999|
|kioskModeManagedHomeScreenPinComplexity|[kioskModeManagedHomeScreenPinComplexity](../resources/intune-deviceconfig-kioskmodemanagedhomescreenpincomplexity.md)|Сложность ПИН-кода для сеанса входа для управляемого начального экрана. Возможные значения: `notConfigured`, `simple`, `complex`.|
|kioskModeManagedHomeScreenPinRequired|Логическое|Указывает, требуется ли пользователю задавать ПИН-код для сеанса входа для управляемого начального экрана.|
|kioskModeManagedHomeScreenPinRequiredToResume|Логическое|Указывает, должен ли пользователь вводить ПИН-код сеанса, если для управляемого начального экрана появился экран.|
|kioskModeManagedHomeScreenSignInBackground|Строка|Фон настраиваемого URL-адреса для экрана входа для управляемого начального экрана.|
|kioskModeManagedHomeScreenSignInBrandingLogo|Строка|Логотип пользовательской фирменной символики URL-адреса для экрана входа и страницы закрепления сеанса для управляемого начального экрана.|
|kioskModeManagedHomeScreenSignInEnabled|Логическое|Указывает, отображается ли экран входа для управляемого начального экрана.|
|kioskModeUseManagedHomeScreenApp|[kioskModeType](../resources/intune-deviceconfig-kioskmodetype.md)|Следует ли использовать режим киоска с одним приложением или режим киоска с несколькими приложениями. Возможные значения: `notConfigured`, `singleAppMode`, `multiAppMode`.|
|microphoneForceMute|Логическое|Указывает, следует ли блокировать отключение микрофона на устройстве.|
|networkEscapeHatchAllowed|Логическое|Указывает, разрешает ли устройство подключаться к временному сетевому подключению во время загрузки.|
|nfcBlockOutgoingBeam|Логическое|Указывает, следует ли блокировать исходящий луч NFC.|
|passwordBlockKeyguard|Логический|Указывает, отключен ли keyguard.|
|passwordBlockKeyguardFeatures|[Коллекция androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Список функций keyguard устройства для блокировки. Эта коллекция может содержать не более 7 элементов.|
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
|securityDeveloperSettingsEnabled|Логическое|Указывает, разрешен ли пользователю доступ к параметрам разработчика, таким как параметры разработчика и безопасная загрузка на устройстве.|
|securityRequireVerifyApps|Boolean|Указывает, требуются ли приложения.|
|shortHelpText|[androidDeviceOwnerUserFacingMessage](../resources/intune-deviceconfig-androiddeviceowneruserfacingmessage.md)|Представляет настраиваемый короткий текст справки, предоставленный пользователям при попытке изменить управляемые параметры на устройстве.|
|statusBarBlocked|Логическое|Указывает, отключена ли строка состояния, включая уведомления, быстрые параметры и другие наложения экрана.|
|stayOnModes|[Коллекция androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Список режимов, в которых экран устройства будет оставаться активным. Эта коллекция может содержать не более 4 элементов.|
|storageAllowUsb|Логическое|Указывает, следует ли разрешить usb-накопитель.|
|storageBlockExternalMedia|Логическое|Указывает, следует ли блокировать внешний носитель.|
|storageBlockUsbFileTransfer|Логический|Указывает, следует ли блокировать передачу USB-файлов.|
|systemUpdateFreezePeriods|[Коллекция androidDeviceOwnerSystemUpdateFreezePeriod](../resources/intune-deviceconfig-androiddeviceownersystemupdatefreezeperiod.md)|Указывает периоды времени, повторяющиеся ежегодно, в течение которых обновления системы откладываются. Эта коллекция может содержать не более 500 элементов.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Указывает количество минут после полуночи, в течение которых запускается окно обновления системы. Допустимые значения от 0 до 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Указывает количество минут после полуночи, в течение которых заканчивается окно обновления системы. Допустимые значения от 0 до 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|Тип конфигурации обновления системы. Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|systemWindowsBlocked|Логическое|Следует ли блокировать окна системных запросов Android, такие как всплывающие уведомления, действия с телефоном и системные оповещения.|
|usersBlockAdd|Логическое|Указывает, отключено ли добавление пользователей и профилей.|
|usersBlockRemove|Логическое|Указывает, следует ли отключить удаление других пользователей с устройства.|
|volumeBlockAdjustment|Логическое|Указывает, отключена ли настройка главного тома.|
|VpnAlwaysOnLockdownMode|Логическое|Если указано имя пакета VPN always on, следует ли блокировать сетевой трафик при отключении vpn.|
|vpnAlwaysOnPackageIdentifier|Строка|Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.|
|WifiBlockEditConfigurations|Логическое|Указывает, следует ли запретить пользователю изменять параметры подключения Wi-Fi.|
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

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[Коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства по пользователю. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
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
  "azureAdSharedDeviceDataClearApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
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
  "crossProfilePoliciesAllowCopyPaste": true,
  "crossProfilePoliciesAllowDataSharing": "String",
  "crossProfilePoliciesShowWorkContactsInPersonalProfile": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "String",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "String",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "String",
  "enrollmentProfile": "String",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "detailedHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "String",
        "value": "String"
      }
    ],
    "defaultMessage": "String"
  },
  "factoryResetDeviceAdministratorEmails": [
    "String"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "String"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "String",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "String",
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
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "String",
  "kioskModeIconSize": "String",
  "kioskModeFolderIcon": "String",
  "kioskModeWifiAllowedSsids": [
    "String"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 1024,
  "kioskModeGridWidth": 1024,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "String",
      "folderIdentifier": "String",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "String",
          "link": "String"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 1024,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "String",
        "link": "String"
      }
    }
  ],
  "kioskModeManagedHomeScreenAutoSignout": true,
  "kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds": 1024,
  "kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds": 1024,
  "kioskModeManagedHomeScreenPinComplexity": "String",
  "kioskModeManagedHomeScreenPinRequired": true,
  "kioskModeManagedHomeScreenPinRequiredToResume": true,
  "kioskModeManagedHomeScreenSignInBackground": "String",
  "kioskModeManagedHomeScreenSignInBrandingLogo": "String",
  "kioskModeManagedHomeScreenSignInEnabled": true,
  "kioskModeUseManagedHomeScreenApp": "String",
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
  "passwordRequireUnlock": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "playStoreMode": "String",
  "screenCaptureBlocked": true,
  "securityDeveloperSettingsEnabled": true,
  "securityRequireVerifyApps": true,
  "shortHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "String",
        "value": "String"
      }
    ],
    "defaultMessage": "String"
  },
  "statusBarBlocked": true,
  "stayOnModes": [
    "String"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateFreezePeriods": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod",
      "startMonth": 1024,
      "startDay": 1024,
      "endMonth": 1024,
      "endDay": 1024
    }
  ],
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
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "personalProfilePlayStoreMode": "String",
  "personalProfilePersonalApplications": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "workProfilePasswordExpirationDays": 1024,
  "workProfilePasswordMinimumLength": 1024,
  "workProfilePasswordMinimumNumericCharacters": 1024,
  "workProfilePasswordMinimumNonLetterCharacters": 1024,
  "workProfilePasswordMinimumLetterCharacters": 1024,
  "workProfilePasswordMinimumLowerCaseCharacters": 1024,
  "workProfilePasswordMinimumUpperCaseCharacters": 1024,
  "workProfilePasswordMinimumSymbolCharacters": 1024,
  "workProfilePasswordPreviousPasswordCountToBlock": 1024,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 1024,
  "workProfilePasswordRequiredType": "String"
}
```




