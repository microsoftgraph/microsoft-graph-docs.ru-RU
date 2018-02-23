# <a name="iosgeneraldeviceconfiguration-resource-type"></a>Тип ресурса iosGeneralDeviceConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом iosGeneralDeviceConfiguration.

Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов IosGeneralDeviceConfiguration](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_list.md)|Коллекция [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|Перечисление свойств и связей объектов [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).|
|[Получение объекта iosGeneralDeviceConfiguration](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_get.md)|[iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|Чтение свойств и связей объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).|
|[Создание объекта iosGeneralDeviceConfiguration](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_create.md)|[iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|Создание объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).|
|[Удаление объекта iosGeneralDeviceConfiguration](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_delete.md)|Нет|Удаление объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).|
|[Обновление объекта iosGeneralDeviceConfiguration](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_update.md)|[iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|accountBlockModification|Boolean|Указывает, можно ли изменять учетную запись, когда устройство находится в контролируемом режиме.|
|activationLockAllowWhenSupervised|Boolean|Указывает, следует ли запретить блокировку активации, когда устройство находится в контролируемом режиме.|
|airDropBlocked|Boolean|Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в контролируемом режиме.|
|airDropForceUnmanagedDropTarget|Boolean|Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и выше).|
|airPlayForcePairingPasswordForOutgoingRequests|Boolean|Указывает, обязательное ли использование пароля для сопряжения на всех устройствах, получающих запросы AirPlay с этого устройства.|
|appleWatchBlockPairing|Boolean|Указывает, следует ли запретить сопряжение с Apple Watch, когда устройство находится в контролируемом режиме (iOS 9.0 и выше).|
|appleWatchForceWristDetection|Boolean|Указывает, обязательно ли использовать функцию распознавания запястья на сопряженном устройстве Apple Watch (iOS 8.2 и выше).|
|appleNewsBlocked|Boolean|Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в контролируемом режиме (iOS 9.0 и выше).|
|appsSingleAppModeList|Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)|Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы. Только в контролируемом режиме. iOS 7.0 и выше. Эта коллекция может содержать не более 500 элементов.|
|appsVisibilityList|Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)|Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и выше). Эта коллекция может содержать не более 10 000 элементов.|
|appsVisibilityListType|String|Тип списка, определенного свойством AppsVisibilityList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Boolean|Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в контролируемом режиме (iOS 9.0 и выше).|
|appStoreBlocked|Boolean|Указывает, следует ли запретить использовать App Store.|
|appStoreBlockInAppPurchases|Boolean|Указывает, следует ли запретить пользователю совершать покупки из приложения.|
|appStoreBlockUIAppInstallation|Boolean|Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения. Применяется только к контролируемому режиму (iOS 9.0 или выше).|
|appStoreRequirePassword|Boolean|Указывает, требуется ли пароль при использовании приложения App Store.|
|bluetoothBlockModification|Boolean|Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в контролируемом режиме (iOS 10.0 и выше).|
|cameraBlocked|Boolean|Указывает, следует ли запретить доступ к камере устройства.|
|cellularBlockDataRoaming|Boolean|Указывает, следует ли блокировать передачу данных в роуминге.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolean|Указывает, следует ли заблокировать получение фоновых данных в роуминге.|
|cellularBlockPerAppDataModification|Boolean|Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в контролируемом режиме.|
|cellularBlockPersonalHotspot|Boolean|Указывает, следует ли заблокировать режим модема.|
|cellularBlockVoiceRoaming|Boolean|Указывает, следует ли заблокировать голосовой роуминг.|
|certificatesBlockUntrustedTlsCertificates|Boolean|Указывает, следует ли заблокировать ненадежные сертификаты TLS.|
|classroomAppBlockRemoteScreenObservation|Boolean|Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в контролируемом режиме (iOS 9.3 и выше).|
|classroomAppForceUnpromptedScreenObservation|Boolean|Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в контролируемом режиме.|
|compliantAppsList|Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)|Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType). Эта коллекция может содержать не более 10 000 элементов.|
|compliantAppListType|String|Список, указанный с помощью свойства AppComplianceList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|configurationProfileBlockChanges|Boolean|Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в режиме наблюдения.|
|definitionLookupBlocked|Boolean|Указывает, следует ли заблокировать поиск определений, когда устройство находится в контролируемом режиме (iOS 8.1.3 и выше).|
|deviceBlockEnableRestrictions|Boolean|Указывает, может ли пользователь включать ограничения в настройках устройства, когда устройство находится в контролируемом режиме.|
|deviceBlockEraseContentAndSettings|Boolean|Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в контролируемом режиме.|
|deviceBlockNameModification|Boolean|Указывает, можно ли изменять имя устройства, когда устройство находится в контролируемом режиме (iOS 9.0 и выше).|
|diagnosticDataBlockSubmission|Boolean|Указывает, следует ли заблокировать отправку диагностических данных.|
|diagnosticDataBlockSubmissionModification|Boolean|Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в контролируемом режиме (iOS 9.3.2 и выше).|
|documentsBlockManagedDocumentsInUnmanagedApps|Boolean|Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.|
|documentsBlockUnmanagedDocumentsInManagedApps|Boolean|Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.|
|emailInDomainSuffixes|Коллекция String|Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.|
|enterpriseAppBlockTrust|Boolean|Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.|
|enterpriseAppBlockTrustModification|Boolean|Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.|
|faceTimeBlocked|Boolean|Указывает, следует ли запретить использовать FaceTime.|
|findMyFriendsBlocked|Boolean|Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в контролируемом режиме.|
|gamingBlockGameCenterFriends|Boolean|Указывает, следует ли запретить пользователю добавлять друзей в Game Center.|
|gamingBlockMultiplayer|Boolean|Указывает, следует ли запретить пользователю играть с несколькими игроками.|
|gameCenterBlocked|Boolean|Указывает, следует ли запретить использовать Game Center, когда устройство находится в контролируемом режиме.|
|hostPairingBlocked|Boolean|Указывает, следует ли запретить сопряжение с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в контролируемом режиме.|
|iBooksStoreBlocked|Boolean|Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в контролируемом режиме.|
|iBooksStoreBlockErotica|Boolean|Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".|
|iCloudBlockActivityContinuation|Boolean|Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.|
|iCloudBlockBackup|Boolean|Указывает, следует ли заблокировать резервное копирование iCloud.|
|iCloudBlockDocumentSync|Boolean|Указывает, следует ли заблокировать синхронизацию документов iCloud.|
|iCloudBlockManagedAppsSync|Boolean|Указывает, следует ли заблокировать облачную синхронизацию управляемых программ.|
|iCloudBlockPhotoLibrary|Boolean|Указывает, следует ли заблокировать медиатеку iCloud.|
|iCloudBlockPhotoStreamSync|Boolean|Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.|
|iCloudBlockSharedPhotoStream|Boolean|Указывает, следует ли заблокировать общий фотопоток.|
|iCloudRequireEncryptedBackup|Boolean|Указывает, обязательно ли шифрование резервных копий iCloud.|
|iTunesBlockExplicitContent|Boolean|Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.|
|iTunesBlockMusicService|Boolean|Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в контролируемом режиме (iOS 9.3 и выше и macOS 10.12 и выше).|
|iTunesBlockRadio|Boolean|Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в контролируемом режиме (iOS 9.3 и выше).|
|keyboardBlockAutoCorrect|Boolean|Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в контролируемом режиме (iOS 8.1.3 и выше).|
|keyboardBlockDictation|Boolean|Указывает, следует ли запретить использовать диктофон, когда устройство находится в контролируемом режиме.|
|keyboardBlockPredictive|Boolean|Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в контролируемом режиме (iOS 8.1.3 и выше).|
|keyboardBlockShortcuts|Boolean|Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в контролируемом режиме (iOS 9.0 и выше).|
|keyboardBlockSpellCheck|Boolean|Указывает, следует ли заблокировать проверку правописания, когда устройство находится в контролируемом режиме (iOS 8.1.3 и выше).|
|kioskModeAllowAssistiveSpeak|Boolean|Указывает, можно ли использовать специальные возможности речеобразования в режиме терминала.|
|kioskModeAllowAssistiveTouchSettings|Boolean|Указывает, следует ли запретить доступ к настройкам Assistive Touch в режиме терминала.|
|kioskModeAllowAutoLock|Boolean|Указывает, следует ли запретить автоблокировку устройства в режиме терминала.|
|kioskModeAllowColorInversionSettings|Boolean|Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме терминала.|
|kioskModeAllowRingerSwitch|Boolean|Указывает, можно ли использовать переключатель звонка в режиме терминала.|
|kioskModeAllowScreenRotation|Boolean|Указывает, следует ли запретить поворот экрана в режиме терминала.|
|kioskModeAllowSleepButton|Boolean|Указывает, можно ли использовать кнопку "Сон" в режиме терминала.|
|kioskModeAllowTouchscreen|Boolean|Указывает, можно ли использовать сенсорный экран в режиме терминала.|
|kioskModeAllowVoiceOverSettings|Boolean|Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме терминала.|
|kioskModeAllowVolumeButtons|Boolean|Указывает, можно ли использовать кнопки громкости в режиме терминала.|
|kioskModeAllowZoomSettings|Boolean|Указывает, следует ли запретить доступ к настройкам масштабирования в режиме терминала.|
|kioskModeAppStoreUrl|String|URL-адрес приложения в App Store для использования в режиме терминала. Используйте, если идентификатор KioskModeManagedAppId не известен.|
|kioskModeRequireAssistiveTouch|Boolean|Указывает, обязательно ли использовать AssistiveTouch в режиме терминала.|
|kioskModeRequireColorInversion|Boolean|Указывает, обязательно ли использовать инверсию цвета в режиме терминала.|
|kioskModeRequireMonoAudio|Boolean|Указывает, обязательно ли использовать монозвук в режиме терминала.|
|kioskModeRequireVoiceOver|Boolean|Указывает, обязательно ли использовать VoiceOver в режиме терминала.|
|kioskModeRequireZoom|Boolean|Указывает, обязательно ли использовать масштабирование в режиме терминала.|
|kioskModeManagedAppId|String|Идентификатор управляемого приложения для использования в режиме терминала. Если указан идентификатор KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.|
|lockScreenBlockControlCenter|Boolean|Указывает, следует ли запретить использовать Пункт управления на заблокированном экране.|
|lockScreenBlockNotificationView|Boolean|Указывает, следует ли запретить использовать Центр уведомлений на заблокированном экране.|
|lockScreenBlockPassbook|Boolean|Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.|
|lockScreenBlockTodayView|Boolean|Указывает, следует ли запретить использовать вид "Сегодня" на заблокированном экране.|
|mediaContentRatingAustralia|[mediaContentRatingAustralia](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|Настройки возрастных ограничений для Австралии|
|mediaContentRatingCanada|[mediaContentRatingCanada](../resources/intune_deviceconfig_mediacontentratingcanada.md)|Настройки возрастных ограничений для Канады|
|mediaContentRatingFrance|[mediaContentRatingFrance](../resources/intune_deviceconfig_mediacontentratingfrance.md)|Настройки возрастных ограничений для Франции|
|mediaContentRatingGermany|[mediaContentRatingGermany](../resources/intune_deviceconfig_mediacontentratinggermany.md)|Настройки возрастных ограничений для Германии|
|mediaContentRatingIreland|[mediaContentRatingIreland](../resources/intune_deviceconfig_mediacontentratingireland.md)|Настройки возрастных ограничений для Ирландии|
|mediaContentRatingJapan|[mediaContentRatingJapan](../resources/intune_deviceconfig_mediacontentratingjapan.md)|Настройки возрастных ограничений для Японии|
|mediaContentRatingNewZealand|[mediaContentRatingNewZealand](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|Настройки возрастных ограничений для Новой Зеландии|
|mediaContentRatingUnitedKingdom|[mediaContentRatingUnitedKingdom](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|Настройки возрастных ограничений для Соединенного Королевства|
|mediaContentRatingUnitedStates|[mediaContentRatingUnitedStates](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|Настройки возрастных ограничений для США|
|networkUsageRules|Коллекция [iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)|Список управляемых приложений и сетевых правил, которые к ним применяются. Эта коллекция может содержать не более 1000 элементов.|
|mediaContentRatingApps|String|Настройки возрастных ограничений для приложений. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.|
|messagesBlocked|Boolean|Указывает, следует ли запретить использовать приложение "Сообщения" на контролируемом устройстве.|
|notificationsBlockSettingsModification|Boolean|Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и выше).|
|passcodeBlockFingerprintUnlock|Boolean|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passcodeBlockFingerprintModification|Boolean|Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в контролируемом режиме.|
|passcodeBlockModification|Boolean|Указывает, можно ли изменять код‑пароль на контролируемом устройстве (iOS 9.0 и выше).|
|passcodeBlockSimple|Boolean|Указывает, следует ли заблокировать простые коды‑пароли.|
|passcodeExpirationDays|Int32|Количество дней до окончания срока действия кода-пароля. Допустимые значения: от 1 до 65 535.|
|passcodeMinimumLength|Int32|Минимальная длина кода-пароля. Допустимые значения: от 4 до 14.|
|passcodeMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах) до запроса пароля.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passcodeMinimumCharacterSetCount|Int32|Количество наборов символов, которые должен содержать код-пароль. Допустимые значения: от 0 до 4.|
|passcodePreviousPasscodeBlockCount|Int32|Количество предыдущих кодов-паролей, которые следует блокировать. Допустимые значения: от 1 до 24.|
|passcodeSignInFailureCountBeforeWipe|Int32|Количество неудачных попыток входа до очистки устройства. Допустимые значения: от 4 до 11|
|passcodeRequiredType|String|Необходимый тип кода-пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Boolean|Указывает, обязательно ли использовать код-пароль.|
|podcastsBlocked|Boolean|Указывает, следует ли запретить использовать подкасты на контролируемом устройстве (iOS 8.0 и выше).|
|safariBlockAutofill|Boolean|Указывает, следует ли запретить использовать автозаполнение в Safari.|
|safariBlockJavaScript|Boolean|Указывает, следует ли заблокировать JavaScript в Safari.|
|safariBlockPopups|Boolean|Указывает, следует ли блокировать всплывающие окна в Safari.|
|safariBlocked|Boolean|Указывает, следует ли запретить использовать Safari.|
|safariCookieSettings|String|Настройки файлов cookie для Safari. Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|Коллекция String|URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.|
|safariPasswordAutoFillDomains|Коллекция String|Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам. Применяется к устройствам в контролируемом режиме (iOS 9.3 и выше).|
|safariRequireFraudWarning|Boolean|Указывает, обязательно ли предупреждение о мошенничестве в Safari.|
|screenCaptureBlocked|Boolean|Указывает, следует ли запретить пользователю делать снимки экрана.|
|siriBlocked|Boolean|Указывает, следует ли запретить использовать Siri.|
|siriBlockedWhenLocked|Boolean|Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.|
|siriBlockUserGeneratedContent|Boolean|Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на контролируемом устройстве.|
|siriRequireProfanityFilter|Boolean|Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на контролируемом устройстве.|
|spotlightBlockInternetResults|Boolean|Указывает, следует ли запретить показывать результаты из Интернета при поиске в Spotlight на контролируемом устройстве.|
|voiceDialingBlocked|Boolean|Указывает, следует ли заблокировать голосовой набор.|
|wallpaperBlockModification|Boolean|Указывает, можно ли изменять обои на контролируемом устройстве (iOS 9.0 и выше).|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в контролируемом режиме.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства для каждого пользователя. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

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
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "String",
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
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```



