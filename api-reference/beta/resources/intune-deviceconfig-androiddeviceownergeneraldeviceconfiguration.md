---
title: тип ресурса androidDeviceOwnerGeneralDeviceConfiguration
description: В этом разделе описаны объявленные методы, свойства и связи, открытые ресурсом androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0bb4b046893bb4023a8bbf5550f501822bca9d68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148062"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>тип ресурса androidDeviceOwnerGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этом разделе описаны объявленные методы, свойства и связи, открытые ресурсом androidDeviceOwnerGeneralDeviceConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[коллекция androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Список свойств и связей [объектов androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|
|[Get androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Чтение свойств и связей [объекта AndroidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|
|[Создание androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Создайте новый [объект androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|
|[Удаление androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|Нет|Удаляет [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).|
|[Обновление androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Обновление свойств объекта [AndroidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|

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
|azureAdSharedDeviceDataClearApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, которые будут очищать свои данные во время глобальной регистрации в режиме общего устройства AAD. Эта коллекция может содержать не более 500 элементов.|
|accountsBlockModification|Логическое|Указывает, отключена ли добавление или удаление учетных записей.|
|appsAllowInstallFromUnknownSources|Логический|Указывает, разрешено ли пользователю включить параметр неизвестных источников.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Указывает значение политики автоматического обновления приложения. Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Указывает политику разрешений для запросов на разрешения на время запуска, если она не определена специально для приложения. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Логическое|Следует ли рекомендовать всем приложениям пропускать добавленные в первый раз подсказки.|
|BluetoothBlockConfiguration|Логический|Указывает, следует ли блокировать пользователю настройку Bluetooth.|
|BluetoothBlockContactSharing|Логическое|Указывает, следует ли блокировать пользователю доступ к контактам по Bluetooth.|
|cameraBlocked|Boolean|Указывает, следует ли отключить использование камеры.|
|cellularBlockWiFiTethering|Boolean|Указывает, следует ли заблокировать модем Wi-Fi.|
|certificateCredentialConfigurationDisabled|Логический|Указывает, следует ли блокировать пользователям любую конфигурацию учетных данных сертификатов.|
|MicrosoftLauncherConfigurationEnabled|Логическое|Указывает, нужно ли настраивать Microsoft Launcher.|
|MicrosoftLauncherCustomWallpaperEnabled|Логическое|Указывает, следует ли настраивать обои на целевых устройствах.|
|MicrosoftLauncherCustomWallpaperImageUrl|String|Указывает URL-адрес для файла изображений, который будет использовать в качестве обои на целевых устройствах.|
|MicrosoftLauncherCustomWallpaperAllowUserModification|Логическое|Указывает, может ли пользователь изменить обои, чтобы персонализировать свое устройство.|
|microsoftLauncherFeedEnabled|Логический|Указывает, хотите ли вы включить канал запуска на устройстве.|
|MicrosoftLauncherFeedAllowUserModification|Логический|Указывает, может ли пользователь изменить канал запуска на устройстве.|
|MicrosoftLauncherDockPresenceConfiguration|[microsoftLauncherDockPresence](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|Указывает, нужно ли настраивать док-станцию устройства. Возможные значения: `notConfigured`, `show`, `hide`, `disabled`.|
|MicrosoftLauncherDockPresenceAllowUserModification|Логическое|Указывает, может ли пользователь изменить конфигурацию док-станции устройства на устройстве.|
|MicrosoftLauncherSearchBarPlacementConfiguration|[microsoftLauncherSearchBarPlacement](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|Указывает конфигурацию размещения панели поиска на устройстве. Возможные значения: `notConfigured`, `top`, `bottom`, `hide`.|
|enrollmentProfile|[androidDeviceOwnerEnrollmentProfileType](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|Указывает, какой профиль регистрации необходимо настроить. Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.|
|dataRoamingBlocked|Логическое|Указывает, следует ли блокировать пользователю роуминг данных.|
|dateTimeConfigurationBlocked|Логическое|Указывает, следует ли блокировать пользователю вручную изменять дату или время на устройстве|
|factoryResetDeviceAdministratorEmails|Коллекция объектов string|Список электронных писем учетной записи Google, которые необходимо будет проверить подлинность после сброса устройства перед его настройками.|
|factoryResetBlocked|Boolean|Указывает, отключен ли параметр сброса фабрики в параметрах.|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|Прокси настроен непосредственно с хостом, портом и исключенными хостами.|
|GoogleAccountsBlocked|Логическое|Указывает, будут ли заблокированы учетные записи Google.|
|kioskCustomizationDeviceSettingsBlocked|Логический|Указывает, может ли пользователь получить доступ к приложению Параметры в режиме киоска.|
|kioskCustomizationPowerButtonActionsBlocked|Логический|Отображается ли меню питания при длительном нажатии кнопки Power устройства в режиме киоска.|
|kioskCustomizationStatusBar|[androidDeviceOwnerKioskCustomizationStatusBar](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|Указывает отключение системных данных и уведомлений в режиме киоска. Возможные значения: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.|
|kioskCustomizationSystemErrorWarnings|Логическое|Указывает, показаны ли в режиме киоска диалоги системных ошибок для сбоя или безответных приложений.|
|kioskCustomizationSystemNavigation|[androidDeviceOwnerKioskCustomizationSystemNavigation](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|Указывает, какие функции навигации включены в режиме киоска. Возможные значения: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.|
|kioskModeScreenSaverConfigurationEnabled|Логическое|Включить или не включить режим сохранения экрана или нет в режиме киоска.|
|kioskModeScreenSaverImageUrl|String|URL-адрес для изображения, которое будет сохранения экрана устройства в режиме киоска.|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|Количество секунд, за которые устройство будет отображать за исключением экрана в режиме киоска. Допустимые значения от 0 до 9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|Количество секунд, за которые устройство должно быть неактивным до того, как забереговка экрана будет показана в режиме киоска. Допустимые значения от 1 до 9999999|
|kioskModeScreenSaverDetectMediaDisabled|Логическое|Должен ли на экране устройства показываться закаверка экрана, если звук/видео играет в режиме киоска.|
|kioskModeApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, которые будут показаны, когда устройство находится в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeWallpaperUrl|String|URL-адрес общедоступных изображений, которые можно использовать для обоев, когда устройство находится в режиме киоска.|
|kioskModeExitCode|String|Код выхода, чтобы позволить пользователю выйти из режима киоска, когда устройство находится в режиме киоска.|
|kioskModeVirtualHomeButtonEnabled|Логическое|Следует ли отображать виртуальную домашняя кнопка, когда устройство находится в режиме киоска.|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|Указывает, является ли виртуальная домашняя кнопка пальцем вверх по домашней кнопке или плавающей домашней кнопкой. Возможные значения: `notConfigured`, `swipeUp`, `floating`.|
|kioskModeBluetoothConfigurationEnabled|Логический|Следует ли разрешить пользователю настраивать Bluetooth в режиме киоска.|
|kioskModeWiFiConfigurationEnabled|Логический|Разрешить пользователю настраивать параметры Wi-Fi в режиме киоска.|
|kioskModeFlashlightConfigurationEnabled|Логическое|Разрешить или не разрешить пользователю использовать фонарик в режиме киоска.|
|kioskModeMediaVolumeConfigurationEnabled|Логическое|Разрешить или не разрешить пользователю изменять объем мультимедиа в режиме киоска.|
|kioskModeShowDeviceInfo|Логический|Разрешить пользователю доступ к основным сведениям об устройстве.|
|kioskModeManagedSettingsEntryDisabled|Логический|Отображение управляемой Параметры на управляемом домашнем экране в режиме киоска.|
|kioskModeDebugMenuEasyAccessEnabled|Логическое|Следует ли разрешить пользователю легкий доступ к меню отлаживания в режиме киоска.|
|kioskModeShowAppNotificationBadge|Логический|Отображение значков уведомлений приложений в режиме киоска.|
|kioskModeScreenOrientation|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|Конфигурация ориентации экрана для управляемого домашнего экрана в режиме киоска. Возможные значения: `notConfigured`, `portrait`, `landscape`, `autoRotate`.|
|kioskModeIconSize|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|Конфигурация размера значка для управляемого домашнего экрана в режиме киоска. Возможные значения: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.|
|kioskModeFolderIcon|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|Конфигурация значка папки для управляемого домашнего экрана в режиме киоска. Возможные значения: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.|
|kioskModeWifiAllowedSsids|Коллекция объектов string|Ограниченный набор SSID WIFI, доступный пользователю для настройки в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeAppOrderEnabled|Логическое|Включить или не включить заказ приложений в режиме киоска.|
|kioskModeAppsInFolderOrderedByName|Логический|Следует ли алфавитизировать приложения в папке в режиме киоска.|
|kioskModeGridHeight|Int32|Количество строк для сетки управляемого домашнего экрана с включенной в режиме киоска упорядочением приложений. Допустимые значения от 1 до 9999999|
|kioskModeGridWidth|Int32|Количество столбцов для сетки управляемого домашнего экрана с включенной в режиме киоска упорядочением приложений. Допустимые значения от 1 до 9999999|
|kioskModeLockHomeScreen|Логический|Следует ли заблокировать домашний экран конечному пользователю в режиме киоска.|
|kioskModeManagedFolders|[коллекция androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)|Список управляемых папок для устройства в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeAppPositions|[коллекция androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)|Упорядочение элементов на управляемом домашнем экране режима киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeManagedHomeScreenAutoSignout|Логическое|Следует ли автоматически выписывать приложения режима MHS и общих устройств после неактивного для управляемого домашнего экрана.|
|kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds|Int32|Количество секунд для уведомления пользователя перед автоматическим подписанием для управляемого домашнего экрана. Допустимые значения от 1 до 9999999|
|kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds|Int32|Устройство количество секунд неактивно, прежде чем автоматически подписывать пользователя для управляемого домашнего экрана. Допустимые значения от 1 до 9999999|
|kioskModeManagedHomeScreenPinComplexity|[kioskModeManagedHomeScreenPinComplexity](../resources/intune-deviceconfig-kioskmodemanagedhomescreenpincomplexity.md)|Сложность ПИН-кода для сеанса входов для управляемого домашнего экрана. Возможные значения: `notConfigured`, `simple`, `complex`.|
|kioskModeManagedHomeScreenPinRequired|Логическое|Требуется ли пользователю устанавливать ПИН-код для сеанса регистрации для управляемого домашнего экрана.|
|kioskModeManagedHomeScreenPinRequiredToResume|Логический|Требуется ли пользователю вводить ПИН-код сеанса, если для управляемого домашнего экрана появился зарисовка.|
|kioskModeManagedHomeScreenSignInBackground|String|Настраиваемый фон URL-адреса для экрана регистрации для управляемого домашнего экрана.|
|kioskModeManagedHomeScreenSignInBrandingLogo|String|Пользовательский логотип брендинга URL-адресов для страницы пин-кода для экрана и пин-кода сеанса для управляемого домашнего экрана.|
|kioskModeManagedHomeScreenSignInEnabled|Логический|Показывается ли экран регистрации для управляемого домашнего экрана.|
|microphoneForceMute|Логический|Указывает, следует ли блокировать разгрузку микрофона на устройстве.|
|networkEscapeHatchAllowed|Логическое|Указывает, разрешит ли устройство подключаться к временному сетевому подключению во время загрузки.|
|nfcBlockOutgoingBeam|Логическое|Указывает, следует ли блокировать исходяющий луч NFC.|
|passwordBlockKeyguard|Логический|Указывает, отключен ли ключ-гарант.|
|passwordBlockKeyguardFeatures|[коллекция androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Список функций keyguard устройства, которые необходимо заблокировать. Эта коллекция может содержать не более 7 элементов.|
|passwordExpirationDays|Int32|Указывает время, за которое может быть установлен пароль до истечения срока его действия, и потребуется новый пароль. Допустимые значения: от 1 до 365.|
|passwordMinimumLength|Int32|Указывает минимальную длину пароля, необходимого на устройстве. Допустимые значения: от 4 до 16.|
|passwordMinimumLetterCharacters|Int32|Указывает минимальное количество букв, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumLowerCaseCharacters|Int32|Указывает минимальное число символов более низкого уровня, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumNonLetterCharacters|Int32|Указывает минимальное количество символов без букв, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumNumericCharacters|Int32|Указывает минимальное число числимые символы, необходимые для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumSymbolCharacters|Int32|Указывает минимальное количество символов, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumUpperCaseCharacters|Int32|Указывает минимальное количество символов верхней буквы, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passwordPreviousPasswordCountToBlock|Int32|Указывает длину истории паролей, в которой пользователь не сможет ввести новый пароль, который будет таким же, как любой пароль в истории. Допустимые значения: от 0 до 24.|
|passwordRequiredType|[AndroidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Указывает минимальное качество пароля, необходимое на устройстве. Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Указывает количество случаев, когда пользователь может ввести неправильный пароль до стирки устройства. Допустимые значения: от 4 до 11.|
|playStoreMode|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|Указывает режим Play Store устройства. Возможные значения: `notConfigured`, `allowList`, `blockList`.|
|safeBootBlocked|Логическое|Указывает, отключена ли перезагрузка устройства в безопасную загрузку.|
|screenCaptureBlocked|Boolean|Указывает, следует ли отключить возможность делать снимки экрана.|
|securityAllowDebuggingFeatures|Логический|Указывает, следует ли блокировать пользователю включение функций отладки на устройстве.|
|securityDeveloperSettingsEnabled|Логическое|Указывает, разрешен ли пользователю доступ к настройкам разработчика, например к вариантам разработчика и безопасной загрузке на устройстве.|
|securityRequireVerifyApps|Boolean|Указывает, требуется ли проверка приложений.|
|statusBarBlocked|Логическое|Указывает, отключена ли или отключена планка состояния, включая уведомления, быстрые параметры и другие экранные наложения.|
|stayOnModes|[коллекция androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Список режимов, в которых дисплей устройства будет работать с питанием. Эта коллекция может содержать не более 4 элементов.|
|storageAllowUsb|Логический|Указывает, следует ли разрешить массовое хранилище USB.|
|storageBlockExternalMedia|Логическое|Указывает, следует ли блокировать внешние носитли.|
|storageBlockUsbFileTransfer|Логическое|Указывает, следует ли блокировать передачу usb-файлов.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Указывает количество минут после полуночи, когда начинается окно обновления системы. Допустимые значения от 0 до 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Указывает количество минут после полуночи, когда заканчивается окно обновления системы. Допустимые значения от 0 до 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|Тип конфигурации обновления системы. Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|systemWindowsBlocked|Логический|Блокировка windows системы Android, например всплывающие уведомления, телефонные действия и системные оповещения.|
|usersBlockAdd|Логический|Указывает, отключено ли добавление пользователей и профилей.|
|usersBlockRemove|Логическое|Указывает, следует ли отключить удаление других пользователей с устройства.|
|volumeBlockAdjustment|Логическое|Указывает, отключена ли настройка магистрали.|
|VPNAlwaysOnLockdownMode|Логический|Если всегда указано имя пакета VPN, следует ли заблокировать сетевой трафик при отключении VPN.|
|vpnAlwaysOnPackageIdentifier|String|Имя пакета приложений для Android для приложения, которое будет обрабатывать всегда на VPN-подключение.|
|wifiBlockEditConfigurations|Логический|Указывает, следует ли блокировать пользователю редактирование параметров подключения к Wi-Fi.|
|wifiBlockEditPolicyDefinedConfigurations|Логический|Указывает, следует ли блокировать пользователю редактирование только сетей, определенных политикой.|
|personalProfileAppsAllowInstallFromUnknownSources|Логическое|Указывает, может ли пользователь устанавливать приложения из неизвестных источников в личном профиле.|
|personalProfileCameraBlocked|Логическое|Указывает, следует ли отключить использование камеры в личном профиле.|
|personalProfileScreenCaptureBlocked|Логический|Указывает, следует ли отключить возможность делать скриншоты в личном профиле.|
|workProfilePasswordExpirationDays|Int32|Указывает количество дней, в течение которых можно установить пароль профиля работы до истечения срока его действия, и потребуется новый пароль. Допустимые значения: от 1 до 365.|
|workProfilePasswordMinimumLength|Int32|Указывает минимальную длину пароля профиля работы. Допустимые значения: от 4 до 16.|
|workProfilePasswordMinimumNumericCharacters|Int32|Указывает минимальное число числимые символы, необходимые для пароля профиля работы. Допустимые значения от 1 до 16|
|workProfilePasswordMinimumNonLetterCharacters|Int32|Указывает минимальное количество символов без букв, необходимых для пароля профиля работы. Допустимые значения от 1 до 16|
|workProfilePasswordMinimumLetterCharacters|Int32|Указывает минимальное количество букв, необходимых для пароля профиля работы. Допустимые значения от 1 до 16|
|workProfilePasswordMinimumLowerCaseCharacters|Int32|Указывает минимальное количество символов нижнего уровня, необходимое для пароля профиля работы. Допустимые значения от 1 до 16|
|workProfilePasswordMinimumUpperCaseCharacters|Int32|Указывает минимальное количество символов буквы верхнего уровня, необходимое для пароля профиля работы. Допустимые значения от 1 до 16|
|workProfilePasswordMinimumSymbolCharacters|Int32|Указывает минимальное количество символов, необходимых для пароля профиля работы. Допустимые значения от 1 до 16|
|workProfilePasswordPreviousPasswordCountToBlock|Int32|Указывает длину истории паролей профиля работы, в которой пользователь не сможет ввести новый пароль, который будет таким же, как любой пароль в истории. Допустимые значения: от 0 до 24.|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Указывает количество случаев, когда пользователь может ввести неправильный пароль профиля работы до стирки устройства. Допустимые значения: от 4 до 11.|
|workProfilePasswordRequiredType|[AndroidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Указывает минимальное качество пароля, необходимое для пароля профиля работы. Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|

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
  "securityDeveloperSettingsEnabled": true,
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
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
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



