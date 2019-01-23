---
title: Тип ресурса iosGeneralDeviceConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом iosGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 055abce38989d5d49f1f009ac38b6a5aac548ac2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410891"
---
# <a name="iosgeneraldeviceconfiguration-resource-type"></a>Тип ресурса iosGeneralDeviceConfiguration

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом iosGeneralDeviceConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов IosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-list.md)|Коллекция [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|Перечисление свойств и связей объектов [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).|
|[Получение объекта iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-get.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|Чтение свойств и связей объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).|
|[Создание объекта iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-create.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|Создание объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).|
|[Удаление объекта iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-delete.md)|Нет|Удаление объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).|
|[Обновление объекта iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-update.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).|

## <a name="properties"></a>Свойства
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
|accountBlockModification|Логический|Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.|
|activationLockAllowWhenSupervised|Логический|Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.|
|airDropBlocked|Логический|Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.|
|airDropForceUnmanagedDropTarget|Логический|Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).|
|airPlayForcePairingPasswordForOutgoingRequests|Логический|Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.|
|appleWatchBlockPairing|Логический|Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|appleWatchForceWristDetection|Логический|Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).|
|appleNewsBlocked|Логический|Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|appsSingleAppModeList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы. Только в защищенном режиме. iOS 7.0 и более поздних версий. Эта коллекция может содержать не более 500 элементов.|
|appsVisibilityList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий). Эта коллекция может содержать не более 10 000 элементов.|
|appsVisibilityListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Тип списка, определенного свойством AppsVisibilityList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Логический|Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|appStoreBlocked|Логический|Указывает, следует ли запретить использовать App Store.|
|appStoreBlockInAppPurchases|Логический|Указывает, следует ли запретить пользователю совершать покупки из приложения.|
|appStoreBlockUIAppInstallation|Логический|Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения. Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).|
|appStoreRequirePassword|Логический|Указывает, требуется ли пароль, когда вы используете приложение App Store.|
|bluetoothBlockModification|Логический|Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).|
|cameraBlocked|Логический|Указывает, следует ли запретить доступ к камере устройства.|
|cellularBlockDataRoaming|Логический|Указывает, следует ли блокировать передачу данных в роуминге.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Логический|Указывает, следует ли заблокировать получение фоновых данных в роуминге.|
|cellularBlockPerAppDataModification|Логический|Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.|
|cellularBlockPersonalHotspot|Логический|Указывает, следует ли заблокировать личный хот-спот.|
|cellularBlockVoiceRoaming|Логический|Указывает, следует ли заблокировать голосовой роуминг.|
|certificatesBlockUntrustedTlsCertificates|Логический|Указывает, следует ли заблокировать ненадежные сертификаты TLS.|
|classroomAppBlockRemoteScreenObservation|Логический|Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).|
|classroomAppForceUnpromptedScreenObservation|Логический|Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.|
|compliantAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType). Эта коллекция может содержать не более 10 000 элементов.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Список, указанный с помощью свойства AppComplianceList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|configurationProfileBlockChanges|Логический|Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.|
|definitionLookupBlocked|Логический|Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|deviceBlockEnableRestrictions|Логический|Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.|
|deviceBlockEraseContentAndSettings|Логический|Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.|
|deviceBlockNameModification|Логический|Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|diagnosticDataBlockSubmission|Логический|Указывает, следует ли заблокировать отправку диагностических данных.|
|diagnosticDataBlockSubmissionModification|Логический|Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).|
|documentsBlockManagedDocumentsInUnmanagedApps|Логический|Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.|
|documentsBlockUnmanagedDocumentsInManagedApps|Логический|Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.|
|emailInDomainSuffixes|Коллекция String|Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.|
|enterpriseAppBlockTrust|Логический|Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.|
|enterpriseAppBlockTrustModification|Логический|Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.|
|faceTimeBlocked|Логический|Указывает, следует ли запретить использовать FaceTime.|
|findMyFriendsBlocked|Логический|Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в защищенном режиме.|
|gamingBlockGameCenterFriends|Логический|Указывает, следует ли запретить пользователю добавлять друзей в Game Center.|
|gamingBlockMultiplayer|Логический|Указывает, следует ли запретить пользователю играть с несколькими игроками.|
|gameCenterBlocked|Логический|Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.|
|hostPairingBlocked|Логический|Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.|
|iBooksStoreBlocked|Логический|Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.|
|iBooksStoreBlockErotica|Логический|Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".|
|iCloudBlockActivityContinuation|Логический|Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве с iOS или macOS.|
|iCloudBlockBackup|Логический|Указывает, следует ли заблокировать резервное копирование iCloud.|
|iCloudBlockDocumentSync|Логический|Указывает, следует ли заблокировать синхронизацию документов iCloud.|
|iCloudBlockManagedAppsSync|Логический|Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.|
|iCloudBlockPhotoLibrary|Логический|Указывает, следует ли заблокировать медиатеку iCloud.|
|iCloudBlockPhotoStreamSync|Логический|Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.|
|iCloudBlockSharedPhotoStream|Логический|Указывает, следует ли заблокировать общий фотопоток.|
|iCloudRequireEncryptedBackup|Логический|Указывает, обязательно ли шифровать резервные копии iCloud.|
|iTunesBlockExplicitContent|Логический|Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.|
|iTunesBlockMusicService|Логический|Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).|
|iTunesBlockRadio|Логический|Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).|
|keyboardBlockAutoCorrect|Логический|Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|keyboardBlockDictation|Логический|Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.|
|keyboardBlockPredictive|Логический|Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|keyboardBlockShortcuts|Логический|Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|keyboardBlockSpellCheck|Логический|Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|kioskModeAllowAssistiveSpeak|Логический|Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.|
|kioskModeAllowAssistiveTouchSettings|Логический|Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.|
|kioskModeAllowAutoLock|Логический|Указывает, следует ли запретить автоблокировку устройства в режиме киоска.|
|kioskModeAllowColorInversionSettings|Логический|Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.|
|kioskModeAllowRingerSwitch|Логический|Указывает, можно ли использовать переключатель звонка в режиме киоска.|
|kioskModeAllowScreenRotation|Логический|Указывает, следует ли запретить поворот экрана в режиме киоска.|
|kioskModeAllowSleepButton|Логический|Указывает, можно ли использовать кнопку "Сон" в режиме киоска.|
|kioskModeAllowTouchscreen|Логический|Указывает, можно ли использовать сенсорный экран в режиме киоска.|
|kioskModeAllowVoiceOverSettings|Логический|Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.|
|kioskModeAllowVolumeButtons|Логический|Указывает, можно ли использовать кнопки громкости в режиме киоска.|
|kioskModeBlockVolumeButtons|Boolean|Указывает, следует ли блокировать кнопки громкости в режиме терминала.|
|kioskModeAllowZoomSettings|Логический|Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.|
|kioskModeAppStoreUrl|String|URL-адрес приложения в App Store для использования в режиме киоска. Используйте, если свойство KioskModeManagedAppId не известно.|
|kioskModeBuiltInAppId|String|КОД для встроенных приложений для использования в полноэкранном режиме. Используется при KioskModeManagedAppId и KioskModeAppStoreUrl не установлен.|
|kioskModeRequireAssistiveTouch|Логический|Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.|
|kioskModeRequireColorInversion|Логический|Указывает, обязательно ли использовать инверсию цвета в режиме киоска.|
|kioskModeRequireMonoAudio|Логический|Указывает, обязательно ли использовать монозвук в режиме киоска.|
|kioskModeRequireVoiceOver|Логический|Указывает, обязательно ли использовать VoiceOver в режиме киоска.|
|kioskModeRequireZoom|Логический|Указывает, обязательно ли использовать масштабирование в режиме киоска.|
|kioskModeManagedAppId|String|Идентификатор управляемого приложения для использования в режиме киоска. Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.|
|lockScreenBlockControlCenter|Логический|Указывает, следует ли запретить использовать центр управления на заблокированном экране.|
|lockScreenBlockNotificationView|Логический|Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.|
|lockScreenBlockPassbook|Логический|Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.|
|lockScreenBlockTodayView|Логический|Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.|
|mediaContentRatingAustralia|[mediaContentRatingAustralia](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|Настройки возрастных ограничений для Австралии|
|mediaContentRatingCanada|[mediaContentRatingCanada](../resources/intune-deviceconfig-mediacontentratingcanada.md)|Настройки возрастных ограничений для Канады|
|mediaContentRatingFrance|[mediaContentRatingFrance](../resources/intune-deviceconfig-mediacontentratingfrance.md)|Настройки возрастных ограничений для Франции|
|mediaContentRatingGermany|[mediaContentRatingGermany](../resources/intune-deviceconfig-mediacontentratinggermany.md)|Настройки возрастных ограничений для Германии|
|mediaContentRatingIreland|[mediaContentRatingIreland](../resources/intune-deviceconfig-mediacontentratingireland.md)|Настройки возрастных ограничений для Ирландии|
|mediaContentRatingJapan|[mediaContentRatingJapan](../resources/intune-deviceconfig-mediacontentratingjapan.md)|Настройки возрастных ограничений для Японии|
|mediaContentRatingNewZealand|[mediaContentRatingNewZealand](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|Настройки возрастных ограничений для Новой Зеландии|
|mediaContentRatingUnitedKingdom|[mediaContentRatingUnitedKingdom](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|Настройки возрастных ограничений для Соединенного Королевства|
|mediaContentRatingUnitedStates|[mediaContentRatingUnitedStates](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|Настройки возрастных ограничений для Соединенных Штатов|
|networkUsageRules|Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)|Список управляемых приложений и сетевых правил, которые к ним применяются. Эта коллекция может содержать не более 1000 элементов.|
|mediaContentRatingApps|[ratingAppsType](../resources/intune-deviceconfig-ratingappstype.md)|Оценка параметры для приложений контента мультимедиа. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.|
|messagesBlocked|Логический|Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.|
|notificationsBlockSettingsModification|Логический|Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).|
|passcodeBlockFingerprintUnlock|Логический|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passcodeBlockFingerprintModification|Логический|Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.|
|passcodeBlockModification|Логический|Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).|
|passcodeBlockSimple|Логический|Указывает, следует ли блокировать простые секретные коды.|
|passcodeExpirationDays|Int32|Количество дней до окончания срока действия секретного кода. Допустимые значения: от 1 до 65 535.|
|passcodeMinimumLength|Int32|Минимальная длина секретного кода. Допустимые значения: от 4 до 14.|
|passcodeMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах) до запроса пароля.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passcodeMinimumCharacterSetCount|Int32|Количество наборов символов, которые должен содержать секретный код. Допустимые значения: от 0 до 4.|
|passcodePreviousPasscodeBlockCount|Int32|Количество предыдущих секретных кодов, которые следует блокировать. Допустимые значения: от 1 до 24.|
|passcodeSignInFailureCountBeforeWipe|Int32|Количество неудачных попыток входа до очистки устройства. Допустимые значения: от 4 до 11|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Необходимый тип секретного кода. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Логический|Указывает, обязательно ли использовать секретный код.|
|podcastsBlocked|Логический|Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).|
|safariBlockAutofill|Логический|Указывает, следует ли запретить использовать автозаполнение в Safari.|
|safariBlockJavaScript|Логический|Указывает, следует ли заблокировать JavaScript в Safari.|
|safariBlockPopups|Логический|Указывает, следует ли блокировать всплывающие окна в Safari.|
|safariBlocked|Логический|Указывает, следует ли запретить использовать Safari.|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Настройки файлов cookie для Safari. Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|Коллекция String|URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.|
|safariPasswordAutoFillDomains|Коллекция String|Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам. Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).|
|safariRequireFraudWarning|Логический|Указывает, обязательно ли предупреждение о мошенничестве в Safari.|
|screenCaptureBlocked|Логический|Указывает, следует ли запретить пользователю делать снимки экрана.|
|siriBlocked|Логический|Указывает, следует ли запретить использовать Siri.|
|siriBlockedWhenLocked|Логический|Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.|
|siriBlockUserGeneratedContent|Логический|Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.|
|siriRequireProfanityFilter|Логический|Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.|
|spotlightBlockInternetResults|Логический|Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.|
|voiceDialingBlocked|Логический|Указывает, следует ли заблокировать голосовой набор.|
|wallpaperBlockModification|Логический|Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).|
|wiFiConnectOnlyToConfiguredNetworks|Логический|Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.|
|classroomForceRequestPermissionToLeaveClasses|Логический|Указывает, будет ли студента участвуют в неуправляемых курс с помощью аудиторий запрашивающих разрешение из преподаватель при попытке оставьте курс (операций ввода-вывода 11.3 и более поздних версий).|
|keychainBlockCloudSync|Логический|Указывает, заблокирован ли iCloud ключей синхронизации.|
|pkiBlockOTAUpdates|Логический|Указывает ли беспроводной PKI заблокированы. Задание ограничения значение false, не отключает проверки списка отзыва Сертификатов и OCSP (операций ввода-вывода 7.0 и более поздних версий).|
|privacyForceLimitAdTracking|Логический|Указывает, является ли ограниченный ad отслеживания. (операций ввода-вывода 7.0 и более поздних версий).|
|enterpriseBookBlockBackup|Логический|Указывает, что заблокирован ли Enterprise книги резервного копирования.|
|enterpriseBookBlockMetadataSync|Логический|Указывает, заблокирован ли Enterprise книги notes и основные сведения о синхронизации.|
|airPrintBlocked|Логический|Указывает, является ли AirPrint заблокированных (операций ввода-вывода 11.0 и более поздних версий).|
|airPrintBlockCredentialsStorage|Логический|Указывает, является ли хранилища ключей имя пользователя и пароль для Airprint заблокированных (операций ввода-вывода 11.0 и более поздних версий).|
|airPrintForceTrustedTLS|Логический|Указывает, являются ли доверенные сертификаты для печати обмена данными TLS (операций ввода-вывода 11.0 и более поздних версий).|
|airPrintBlockiBeaconDiscovery|Логический|Указывает, заблокирован ли обнаружения iBeacon AirPrint принтеров. Это позволяет предотвратить ложных маяки AirPrint Bluetooth от фишинга для сетевого трафика (операций ввода-вывода 11.0 и более поздних версий).|
|blockSystemAppRemoval|Логический|Указывает, заблокирован ли удаления приложений системы с устройства на контролируемом устройства (операций ввода-вывода 11.0 и более поздних версий).|
|vpnBlockCreation|Логический|Указывает, является ли создание конфигурации VPN заблокированных (операций ввода-вывода 11.0 и более поздних версий).|
|appRemovalBlocked|Логический|Указывает, разрешено ли удаление приложений.|
|usbRestrictedModeBlocked|Логический|Указывает, разрешено ли подключение стандартные USB, хотя устройство заблокировано (операций ввода-вывода 11.4.1 и более поздних версий).|
|passwordBlockAutoFill|Логический|Указывает, разрешено ли функцию автозаполнения паролей (операций ввода-вывода 12.0 и более поздних версий).|
|passwordBlockProximityRequests|Логический|Указывает, следует ли блокировать запрашивающая пароли с рядом устройств (операций ввода-вывода 12.0 и более поздних версий).|
|passwordBlockAirDropSharing|Логический|Указывает ли блокировать общего доступа пароли с AirDrop iOS компонента пароли 12.0 и более поздних версий).|
|dateAndTimeForceSetAutomatically|Логический|Указывает ли даты и времени «Задать автоматически» компонент включен и не может быть отключена пользователем (операций ввода-вывода 12.0 и более поздних версий).|
|contactsAllowManagedToUnmanagedWrite|Логический|Указывает, следует ли управляемых приложений можно записи контактов к учетным записям неуправляемые контакты (операций ввода-вывода 12.0 и более поздних версий).|
|contactsAllowUnmanagedToManagedRead|Логический|Указывает ли неуправляемые приложения может выполнять чтение из контактов управляемых учетных записей (операций ввода-вывода 12.0 или более поздней версии).|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) коллекции|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsVisibilityListType": "String",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "String"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "String",
  "kioskModeBuiltInAppId": "String",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "String",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "String",
    "tvRating": "String"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "String",
          "publisher": "String",
          "appStoreUrl": "String",
          "appId": "String"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "String",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 1024,
  "passcodeMinimumLength": 1024,
  "passcodeMinutesOfInactivityBeforeLock": 1024,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passcodeMinimumCharacterSetCount": 1024,
  "passcodePreviousPasscodeBlockCount": 1024,
  "passcodeSignInFailureCountBeforeWipe": 1024,
  "passcodeRequiredType": "String",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "String",
  "safariManagedDomains": [
    "String"
  ],
  "safariPasswordAutoFillDomains": [
    "String"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true
}
```




