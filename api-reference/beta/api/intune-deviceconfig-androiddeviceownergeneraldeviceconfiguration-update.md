---
title: Обновление androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта AndroidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0791feafc97ded4943c566ad08968a01ec1206b9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58807204"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a>Обновление androidDeviceOwnerGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [AndroidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)

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
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса предоставляем представление JSON для [объекта AndroidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)

В следующей таблице показаны свойства, необходимые при создании [androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|azureAdSharedDeviceDataClearApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, которые будут очищать свои данные во время глобальной регистрации в режиме общего устройства AAD. Эта коллекция может содержать не более 500 элементов.|
|accountsBlockModification|Логический|Указывает, отключена ли добавление или удаление учетных записей.|
|appsAllowInstallFromUnknownSources|Boolean|Указывает, разрешено ли пользователю включить параметр неизвестных источников.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Указывает значение политики автоматического обновления приложения. Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Указывает политику разрешений для запросов на разрешения на время запуска, если она не определена специально для приложения. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Логический|Следует ли рекомендовать всем приложениям пропускать добавленные в первый раз подсказки.|
|BluetoothBlockConfiguration|Boolean|Указывает, следует ли блокировать пользователю настройку Bluetooth.|
|BluetoothBlockContactSharing|Логический|Указывает, следует ли блокировать пользователю доступ к контактам по Bluetooth.|
|cameraBlocked|Boolean|Указывает, следует ли отключить использование камеры.|
|cellularBlockWiFiTethering|Boolean|Указывает, следует ли заблокировать модем Wi-Fi.|
|certificateCredentialConfigurationDisabled|Логический|Указывает, следует ли блокировать пользователям любую конфигурацию учетных данных сертификатов.|
|MicrosoftLauncherConfigurationEnabled|Логический|Указывает, нужно ли настраивать Microsoft Launcher.|
|MicrosoftLauncherCustomWallpaperEnabled|Логический|Указывает, следует ли настраивать обои на целевых устройствах.|
|MicrosoftLauncherCustomWallpaperImageUrl|Строка|Указывает URL-адрес для файла изображений, который будет использовать в качестве обои на целевых устройствах.|
|MicrosoftLauncherCustomWallpaperAllowUserModification|Логический|Указывает, может ли пользователь изменить обои, чтобы персонализировать свое устройство.|
|microsoftLauncherFeedEnabled|Логический|Указывает, хотите ли вы включить канал запуска на устройстве.|
|MicrosoftLauncherFeedAllowUserModification|Логический|Указывает, может ли пользователь изменить канал запуска на устройстве.|
|MicrosoftLauncherDockPresenceConfiguration|[microsoftLauncherDockPresence](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|Указывает, нужно ли настраивать док-станцию устройства. Возможные значения: `notConfigured`, `show`, `hide`, `disabled`.|
|MicrosoftLauncherDockPresenceAllowUserModification|Логический|Указывает, может ли пользователь изменить конфигурацию док-станции устройства на устройстве.|
|MicrosoftLauncherSearchBarPlacementConfiguration|[microsoftLauncherSearchBarPlacement](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|Указывает конфигурацию размещения панели поиска на устройстве. Возможные значения: `notConfigured`, `top`, `bottom`, `hide`.|
|enrollmentProfile|[androidDeviceOwnerEnrollmentProfileType](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|Указывает, какой профиль регистрации необходимо настроить. Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.|
|dataRoamingBlocked|Boolean|Указывает, следует ли блокировать пользователю роуминг данных.|
|dateTimeConfigurationBlocked|Boolean|Указывает, следует ли блокировать пользователю вручную изменять дату или время на устройстве|
|factoryResetDeviceAdministratorEmails|Коллекция String|Список электронных писем учетной записи Google, которые необходимо будет проверить подлинность после сброса устройства перед его настройками.|
|factoryResetBlocked|Boolean|Указывает, отключен ли параметр сброса фабрики в параметрах.|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|Прокси настроен непосредственно с хостом, портом и исключенными хостами.|
|GoogleAccountsBlocked|Boolean|Указывает, будут ли заблокированы учетные записи Google.|
|kioskCustomizationDeviceSettingsBlocked|Логический|Указывает, может ли пользователь получить доступ к приложению Параметры в режиме киоска.|
|kioskCustomizationPowerButtonActionsBlocked|Boolean|Отображается ли меню питания при длительном нажатии кнопки Power устройства в режиме киоска.|
|kioskCustomizationStatusBar|[androidDeviceOwnerKioskCustomizationStatusBar](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|Указывает отключение системных данных и уведомлений в режиме киоска. Возможные значения: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.|
|kioskCustomizationSystemErrorWarnings|Логический|Указывает, показаны ли в режиме киоска диалоги системных ошибок для сбоя или безответных приложений.|
|kioskCustomizationSystemNavigation|[androidDeviceOwnerKioskCustomizationSystemNavigation](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|Указывает, какие функции навигации включены в режиме киоска. Возможные значения: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.|
|kioskModeScreenSaverConfigurationEnabled|Логический|Включить или не включить режим сохранения экрана или нет в режиме киоска.|
|kioskModeScreenSaverImageUrl|String|URL-адрес для изображения, которое будет сохранения экрана устройства в режиме киоска.|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|Количество секунд, за которые устройство будет отображать за исключением экрана в режиме киоска. Допустимые значения от 0 до 9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|Количество секунд, за которые устройство должно быть неактивным до того, как забереговка экрана будет показана в режиме киоска. Допустимые значения от 1 до 9999999|
|kioskModeScreenSaverDetectMediaDisabled|Логический|Должен ли на экране устройства показываться закаверка экрана, если звук/видео играет в режиме киоска.|
|kioskModeApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список управляемых приложений, которые будут показаны, когда устройство находится в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeWallpaperUrl|Строка|URL-адрес общедоступных изображений, которые можно использовать для обоев, когда устройство находится в режиме киоска.|
|kioskModeExitCode|Строка|Код выхода, чтобы позволить пользователю выйти из режима киоска, когда устройство находится в режиме киоска.|
|kioskModeVirtualHomeButtonEnabled|Логический|Следует ли отображать виртуальную домашняя кнопка, когда устройство находится в режиме киоска.|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|Указывает, является ли виртуальная домашняя кнопка пальцем вверх по домашней кнопке или плавающей домашней кнопкой. Возможные значения: `notConfigured`, `swipeUp`, `floating`.|
|kioskModeBluetoothConfigurationEnabled|Логический|Следует ли разрешить пользователю настраивать Bluetooth в режиме киоска.|
|kioskModeWiFiConfigurationEnabled|Логический|Разрешить пользователю настраивать параметры Wi-Fi в режиме киоска.|
|kioskModeFlashlightConfigurationEnabled|Логический|Разрешить или не разрешить пользователю использовать фонарик в режиме киоска.|
|kioskModeMediaVolumeConfigurationEnabled|Логический|Разрешить или не разрешить пользователю изменять объем мультимедиа в режиме киоска.|
|kioskModeShowDeviceInfo|Логический|Разрешить пользователю доступ к основным сведениям об устройстве.|
|kioskModeManagedSettingsEntryDisabled|Логический|Отображение управляемой Параметры на управляемом домашнем экране в режиме киоска.|
|kioskModeDebugMenuEasyAccessEnabled|Boolean|Следует ли разрешить пользователю легкий доступ к меню отлаживания в режиме киоска.|
|kioskModeShowAppNotificationBadge|Логический|Отображение значков уведомлений приложений в режиме киоска.|
|kioskModeScreenOrientation|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|Конфигурация ориентации экрана для управляемого домашнего экрана в режиме киоска. Возможные значения: `notConfigured`, `portrait`, `landscape`, `autoRotate`.|
|kioskModeIconSize|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|Конфигурация размера значка для управляемого домашнего экрана в режиме киоска. Возможные значения: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.|
|kioskModeFolderIcon|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|Конфигурация значка папки для управляемого домашнего экрана в режиме киоска. Возможные значения: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.|
|kioskModeWifiAllowedSsids|Коллекция String|Ограниченный набор SSID WIFI, доступный пользователю для настройки в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeAppOrderEnabled|Логический|Включить или не включить заказ приложений в режиме киоска.|
|kioskModeAppsInFolderOrderedByName|Boolean|Следует ли алфавитизировать приложения в папке в режиме киоска.|
|kioskModeGridHeight|Int32|Количество строк для сетки управляемого домашнего экрана с включенной в режиме киоска упорядочением приложений. Допустимые значения от 1 до 9999999|
|kioskModeGridWidth|Int32|Количество столбцов для сетки управляемого домашнего экрана с включенной в режиме киоска упорядочением приложений. Допустимые значения от 1 до 9999999|
|kioskModeLockHomeScreen|Логический|Следует ли заблокировать домашний экран конечному пользователю в режиме киоска.|
|kioskModeManagedFolders|[коллекция androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)|Список управляемых папок для устройства в режиме киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeAppPositions|[коллекция androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)|Упорядочение элементов на управляемом домашнем экране режима киоска. Эта коллекция может содержать не более 500 элементов.|
|kioskModeManagedHomeScreenAutoSignout|Логический|Следует ли автоматически выписывать приложения режима MHS и общих устройств после неактивного для управляемого домашнего экрана.|
|kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds|Int32|Количество секунд для уведомления пользователя перед автоматическим подписанием для управляемого домашнего экрана. Допустимые значения от 1 до 9999999|
|kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds|Int32|Устройство количество секунд неактивно, прежде чем автоматически подписывать пользователя для управляемого домашнего экрана. Допустимые значения от 1 до 9999999|
|kioskModeManagedHomeScreenPinComplexity|[kioskModeManagedHomeScreenPinComplexity](../resources/intune-deviceconfig-kioskmodemanagedhomescreenpincomplexity.md)|Сложность ПИН-кода для сеанса входов для управляемого домашнего экрана. Возможные значения: `notConfigured`, `simple`, `complex`.|
|kioskModeManagedHomeScreenPinRequired|Логический|Требуется ли пользователю устанавливать ПИН-код для сеанса регистрации для управляемого домашнего экрана.|
|kioskModeManagedHomeScreenPinRequiredToResume|Boolean|Требуется ли пользователю вводить ПИН-код сеанса, если для управляемого домашнего экрана появился зарисовка.|
|kioskModeManagedHomeScreenSignInBackground|Строка|Настраиваемый фон URL-адреса для экрана регистрации для управляемого домашнего экрана.|
|kioskModeManagedHomeScreenSignInBrandingLogo|Строка|Пользовательский логотип брендинга URL-адресов для страницы пин-кода для экрана и пин-кода сеанса для управляемого домашнего экрана.|
|kioskModeManagedHomeScreenSignInEnabled|Логический|Показывается ли экран регистрации для управляемого домашнего экрана.|
|microphoneForceMute|Логический|Указывает, следует ли блокировать разгрузку микрофона на устройстве.|
|networkEscapeHatchAllowed|Логический|Указывает, разрешит ли устройство подключаться к временному сетевому подключению во время загрузки.|
|nfcBlockOutgoingBeam|Логический|Указывает, следует ли блокировать исходяющий луч NFC.|
|passwordBlockKeyguard|Логический|Указывает, отключен ли ключ-гарант.|
|passwordBlockKeyguardFeatures|[коллекция androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Список функций keyguard устройства, которые необходимо заблокировать. Эта коллекция может содержать не более 7 элементов. Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.|
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
|safeBootBlocked|Логический|Указывает, отключена ли перезагрузка устройства в безопасную загрузку.|
|screenCaptureBlocked|Boolean|Указывает, следует ли отключить возможность делать снимки экрана.|
|securityAllowDebuggingFeatures|Boolean|Указывает, следует ли блокировать пользователю включение функций отладки на устройстве.|
|securityDeveloperSettingsEnabled|Логический|Указывает, разрешен ли пользователю доступ к настройкам разработчика, например к вариантам разработчика и безопасной загрузке на устройстве.|
|securityRequireVerifyApps|Boolean|Указывает, требуется ли проверка приложений.|
|statusBarBlocked|Логический|Указывает, отключена ли или отключена планка состояния, включая уведомления, быстрые параметры и другие экранные наложения.|
|stayOnModes|[коллекция androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Список режимов, в которых дисплей устройства будет работать с питанием. Эта коллекция может содержать не более 4 элементов. Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.|
|storageAllowUsb|Логический|Указывает, следует ли разрешить массовое хранилище USB.|
|storageBlockExternalMedia|Логический|Указывает, следует ли блокировать внешние носитли.|
|storageBlockUsbFileTransfer|Логический|Указывает, следует ли блокировать передачу usb-файлов.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Указывает количество минут после полуночи, когда начинается окно обновления системы. Допустимые значения от 0 до 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Указывает количество минут после полуночи, когда заканчивается окно обновления системы. Допустимые значения от 0 до 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|Тип конфигурации обновления системы. Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|systemWindowsBlocked|Логический|Блокировка windows системы Android, например всплывающие уведомления, телефонные действия и системные оповещения.|
|usersBlockAdd|Логический|Указывает, отключено ли добавление пользователей и профилей.|
|usersBlockRemove|Логический|Указывает, следует ли отключить удаление других пользователей с устройства.|
|volumeBlockAdjustment|Логический|Указывает, отключена ли настройка магистрали.|
|VPNAlwaysOnLockdownMode|Логический|Если всегда указано имя пакета VPN, следует ли заблокировать сетевой трафик при отключении VPN.|
|vpnAlwaysOnPackageIdentifier|Строка|Имя пакета приложений для Android для приложения, которое будет обрабатывать всегда на VPN-подключение.|
|wifiBlockEditConfigurations|Boolean|Указывает, следует ли блокировать пользователю редактирование параметров подключения к Wi-Fi.|
|wifiBlockEditPolicyDefinedConfigurations|Логический|Указывает, следует ли блокировать пользователю редактирование только сетей, определенных политикой.|
|personalProfileAppsAllowInstallFromUnknownSources|Логический|Указывает, может ли пользователь устанавливать приложения из неизвестных источников в личном профиле.|
|personalProfileCameraBlocked|Логический|Указывает, следует ли отключить использование камеры в личном профиле.|
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



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 8247

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
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityDeveloperSettingsEnabled": true,
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
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
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
  "workProfilePasswordRequiredType": "required"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8419

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
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityDeveloperSettingsEnabled": true,
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
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
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
  "workProfilePasswordRequiredType": "required"
}
```



