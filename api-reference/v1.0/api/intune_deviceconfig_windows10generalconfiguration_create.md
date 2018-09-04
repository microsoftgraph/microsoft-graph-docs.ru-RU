# <a name="create-windows10generalconfiguration"></a>Создание windows10GeneralConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Создание объекта [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md).
## <a name="prerequisites"></a>Необходимые разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

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
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В теле запроса добавьте представление объекта windows10GeneralConfiguration в формате JSON.

Ниже показаны свойства, которые необходимо указывать при создании объекта windows10GeneralConfiguration.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|String (строка)|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|String (строка)|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|enterpriseCloudPrintDiscoveryEndPoint|String (строка)|Конечная точка для обнаружения облачных принтеров.|
|enterpriseCloudPrintOAuthAuthority|String (строка)|Конечная точка аутентификации для получения токенов OAuth.|
|enterpriseCloudPrintOAuthClientIdentifier|String (строка)|GUID клиентского приложения, которому разрешено получать токены OAuth из системы OAuth.|
|enterpriseCloudPrintResourceIdentifier|String (строка)|URI ресурса OAuth для службы печати, настроенный на портале Azure.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Максимальное количество принтеров, запрашиваемых с конечной точки обнаружения. Этот параметр применяется только к мобильным устройствам. Допустимые значения: от 1 до 65 535.|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String (строка)|URI ресурса OAuth для службы обнаружения принтеров, настроенный на портале Azure.|
|searchBlockDiacritics|Boolean (логический)|Указывает, можно ли использовать диакритические знаки в поиске.|
|searchDisableAutoLanguageDetection|Boolean (логический)|Указывает, следует ли использовать автоматическое определение языка при индексировании контента и свойств.|
|searchDisableIndexingEncryptedItems|Boolean (логический)|Указывает, следует ли запретить индексирование защищенных WIP элементов, чтобы они не отображались в результатах поиска Кортаны или проводника.|
|searchEnableRemoteQueries|Boolean (логический)|Указывает, следует ли заблокировать удаленные запросы к индексу этого компьютера.|
|searchDisableIndexerBackoff|Boolean (логический)|Указывает, следует ли отключить функцию отхода индексатора поиска.|
|searchDisableIndexingRemovableDrive|Boolean (логический)|Указывает, могут ли пользователи добавлять расположения на съемных дисках в библиотеки и для индексирования.|
|searchEnableAutomaticIndexSizeManangement|Boolean (логический)|Указывает минимальный объем памяти на жестком диске с индексом до остановки индексирования.|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune_deviceconfig_diagnosticdatasubmissionmode.md)|Возвращает или задает значение, позволяющее устройству отправлять данные диагностики и телеметрии использования, как, например, Watson. Возможные значения: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Boolean (логический)|Возвращает или задает значение, позволяющее ИТ-администраторам запретить работу приложений и функций с файлами в OneDrive.|
|smartScreenEnableAppInstallControl|Boolean (логический)|Позволяет ИТ-администраторам разрешать или запрещать установку приложений из мест, отличных от Store.|
|personalizationDesktopImageUrl|String (строка)|Начинающийся с http или https URL-адрес изображения в формате JPG, JPEG или PNG, которое необходимо скачать и разместить на рабочем столе, или URL-адрес локального изображения в файловой системе, которое нужно разместить на рабочем столе.|
|personalizationLockScreenImageUrl|String (строка)|Начинающийся с http или https URL-адрес изображения в формате JPG, JPEG или PNG, которое необходимо скачать и разместить на экране блокировки, или URL-адрес локального изображения в файловой системе, которое нужно разместить на экране блокировки.|
|bluetoothAllowedServices|Коллекция String|Укажите список разрешенных служб и профилей Bluetooth в шестнадцатеричном формате.|
|bluetoothBlockAdvertising|Boolean (логический)|Указывает, следует ли запретить использовать рекламу по Bluetooth.|
|bluetoothBlockDiscoverableMode|Boolean (логический)|Указывает, следует ли запретить использовать режим обнаружения по Bluetooth.|
|bluetoothBlockPrePairing|Boolean (логический)|Указывает, следует ли заблокировать автоматическое связывание отдельных пакетных периферийных устройств Bluetooth с главным устройством.|
|edgeBlockAutofill|Boolean (логический)|Указывает, следует ли заблокировать автозаполнение.|
|edgeBlocked|Boolean (логический)|Указывает, следует ли запретить использовать браузер Edge.|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune_deviceconfig_edgecookiepolicy.md)|Указывает, какие файлы cookie следует блокировать в браузере Edge. Возможные значения: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeBlockDeveloperTools|Boolean (логический)|Указывает, следует ли заблокировать средства разработчика в браузере Edge.|
|edgeBlockSendingDoNotTrackHeader|Boolean (логический)|Указывает, следует ли запретить пользователю отправлять заголовок DNT.|
|edgeBlockExtensions|Boolean (логический)|Указывает, следует ли заблокировать расширения в браузере Edge.|
|edgeBlockInPrivateBrowsing|Boolean (логический)|Указывает, следует ли заблокировать просмотр InPrivate в корпоративных сетях в браузере Edge.|
|edgeBlockJavaScript|Boolean (логический)|Указывает, следует ли запретить использовать JavaScript.|
|edgeBlockPasswordManager|Boolean (логический)|Указывает, следует ли заблокировать диспетчер паролей.|
|edgeBlockAddressBarDropdown|Boolean (логический)|Позволяет заблокировать раскрывающийся список адресной строки в Microsoft Edge. Отключите этот параметр, чтобы уменьшить количество сетевых подключений Microsoft Edge к службам Майкрософт.|
|edgeBlockCompatibilityList|Boolean (логический)|Позволяет заблокировать список совместимости Майкрософт в Microsoft Edge. Этот список помогает Edge правильно отображать сайты с известными проблемами совместимости.|
|edgeClearBrowsingDataOnExit|Boolean (логический)|Указывает, следует ли удалять данные просмотра при выходе из Microsoft Edge.|
|edgeAllowStartPagesModification|Boolean (логический)|Указывает, могут ли пользователи изменять начальные страницы в Edge. Используйте свойство EdgeHomepageUrls, чтобы указать начальные страницы по умолчанию, отображаемые при открытии Edge.|
|edgeDisableFirstRunPage|Boolean (логический)|Позволяет заблокировать веб-страницу Майкрософт, которая открывается при первом запуске Microsoft Edge. Эта политика позволяет предприятиям, зарегистрированным в конфигурациях с нулевым выбросом, блокировать эту страницу.|
|edgeBlockLiveTileDataCollection|Boolean (логический)|Позволяет запретить Майкрософт собирать информацию о создании живых плиток, когда пользователи закрепляют сайты из Microsoft Edge на начальном экране.|
|edgeSyncFavoritesWithInternetExplorer|Boolean (логический)|Указывает, следует ли включить синхронизацию избранного между Internet Explorer и Microsoft Edge. Браузеры обмениваются данными о добавлении, удалении и изменении избранных элементов, а также их порядка.|
|cellularBlockDataWhenRoaming|Boolean (логический)|Указывает, следует ли запретить использовать мобильные данные в роуминге.|
|cellularBlockVpn|Boolean (логический)|Указывает, следует ли запретить использовать VPN по сотовой сети.|
|cellularBlockVpnWhenRoaming|Boolean (логический)|Указывает, следует ли запретить использовать VPN по сотовой сети в роуминге.|
|defenderBlockEndUserAccess|Boolean (логический)|Указывает, следует ли заблокировать доступ пользователей к Защитнику.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Время до удаления вредоносного ПО на карантине (в днях). Допустимые значения: от 0 до 90.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune_deviceconfig_defenderdetectedmalwareactions.md)|Возвращает или задает действия Защитника в отношении обнаруженного вредоносного ПО для каждого уровня угрозы.|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune_deviceconfig_weeklyschedule.md)|День проверки системы Защитником. Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|defenderFilesAndFoldersToExclude|Коллекция String|Файлы и папки, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderFileExtensionsToExclude|Коллекция String|Расширения файлов, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderScanMaxCpu|Int32|Максимальный процент загрузки ЦП во время проверки. Допустимые значения: от 0 до 100|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune_deviceconfig_defendermonitorfileactivity.md)|Значение для отслеживания действий с файлами. Возможные значения: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderProcessesToExclude|Коллекция String|Процессы, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune_deviceconfig_defenderpromptforsamplesubmission.md)|Позволяет указать, нужно ли спрашивать пользователя перед отправкой образцов. Возможные значения: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderRequireBehaviorMonitoring|Boolean (логический)|Указывает, обязательно ли использовать наблюдение за поведением.|
|defenderRequireCloudProtection|Boolean (логический)|Указывает, обязательно ли использовать облачную защиту.|
|defenderRequireNetworkInspectionSystem|Boolean (логический)|Указывает, обязательно ли использовать систему проверки сети.|
|defenderRequireRealTimeMonitoring|Boolean (логический)|Указывает, обязательно ли использовать мониторинг в режиме реального времени.|
|defenderScanArchiveFiles|Boolean (логический)|Указывает, следует ли проверять архивные файлы.|
|defenderScanDownloads|Boolean (логический)|Указывает, следует ли проверять загрузки.|
|defenderScanNetworkFiles|Boolean (логический)|Указывает, следует ли сканировать файлы, открытые из сетевой папки.|
|defenderScanIncomingMail|Boolean (логический)|Указывает, следует ли проверять входящую почту.|
|defenderScanMappedNetworkDrivesDuringFullScan|Boolean (логический)|Указывает, следует ли сканировать подключенные сетевые диски во время полной проверки.|
|defenderScanRemovableDrivesDuringFullScan|Boolean (логический)|Указывает, следует ли сканировать съемные диски во время полной проверки.|
|defenderScanScriptsLoadedInInternetExplorer|Boolean (логический)|Указывает, следует ли проверять сценарии, загружаемые в браузере Internet Explorer.|
|defenderSignatureUpdateIntervalInHours|Int32|Интервал обновления сигнатур (в часах). Укажите 0, чтобы не проверять. Допустимые значения: от 0 до 24.|
|defenderScanType|[defenderScanType](../resources/intune_deviceconfig_defenderscantype.md)|Тип проверки системы Защитником. Возможные значения: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledScanTime|TimeOfDay|Время проверки системы Защитником.|
|defenderScheduledQuickScanTime|TimeOfDay|Время ежедневной быстрой проверки.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune_deviceconfig_defendercloudblockleveltype.md)|Определяет уровень облачной защиты. Возможные значения: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|lockScreenAllowTimeoutConfiguration|Boolean (логический)|Указывает, следует ли отображать настройку, позволяющую определить время до отключения экрана на экране блокировки мобильных устройств с Windows 10. Если для этой политики установлено значение Allow, значение, заданное свойством lockScreenTimeoutInSeconds, игнорируется.|
|lockScreenBlockActionCenterNotifications|Boolean (логический)|Указывает, следует ли запретить показ уведомлений из центра уведомлений на экране блокировки.|
|lockScreenBlockCortana|Boolean (логический)|Указывает, может ли пользователь взаимодействовать с Кортаной с помощью голоса при заблокированной системе.|
|lockScreenBlockToastNotifications|Boolean (логический)|Указывает, следует ли показывать всплывающие уведомления на экране блокировки устройства.|
|lockScreenTimeoutInSeconds|Int32|Установите время (в секундах) от блокировки экрана до его выключения для мобильных устройств с Windows 10. Поддерживаемые значения: от 11 до 1800. Допустимые значения: от 11 до 1800.|
|passwordBlockSimple|Boolean (логический)|Укажите, разрешены ли такие ПИН-коды или пароли, как "1111" или "1234". Это свойство также контролирует использование графических паролей на компьютерах с Windows 10.|
|passwordExpirationDays|Int32|Срок действия пароля (в днях). Допустимые значения: от 0 до 730.|
|passwordMinimumLength|Int32|Минимальная длина пароля. Допустимые значения: от 4 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые требуются для пароля.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, повторное использование которых необходимо запретить. Допустимые значения: от 0 до 50.|
|passwordRequired|Boolean (логический)|Указывает, обязательно ли использовать пароль.|
|passwordRequireWhenResumeFromIdleState|Boolean (логический)|Указывает, следует ли запрашивать пароль при выходе из состояния простоя.|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек. Допустимые значения: от 0 до 999.|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Указывает, можно ли использовать идентификатор рекламы. Добавлено в Windows 10 версии 1607. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Boolean (логический)|Указывает, следует ли запретить автоматическое принятие примечаний о связывании и конфиденциальности при запуске приложений.|
|privacyBlockInputPersonalization|Boolean (логический)|Указывает, следует ли запретить использовать облачные службы распознавания речи для приложений "Кортана", "Диктофон" или Store.|
|startBlockUnpinningAppsFromTaskbar|Boolean (логический)|Указывает, следует ли запретить пользователю откреплять приложения с панели задач.|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune_deviceconfig_windowsstartmenuapplistvisibilitytype.md)|Эта политика позволяет свернуть список приложений, полностью удалить этот список или отключить соответствующий переключатель в приложении "Параметры". Возможные значения: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
|startMenuHideChangeAccountSettings|Boolean (логический)|Эта политика позволяет скрыть параметр для смены учетной записи на плитке пользователя в меню "Пуск".|
|startMenuHideFrequentlyUsedApps|Boolean (логический)|Эта политика позволяет скрыть наиболее часто используемые приложения в меню "Пуск" и отключить соответствующий переключатель в приложении "Параметры".|
|startMenuHideHibernate|Boolean (логический)|Эта политика позволяет скрыть параметр кнопки питания для перехода в режим гибернации в меню "Пуск".|
|startMenuHideLock|Boolean (логический)|Эта политика позволяет скрыть параметр для блокировки экрана на плитке пользователя в меню "Пуск".|
|startMenuHidePowerButton|Boolean (логический)|Эта политика позволяет скрыть кнопку питания в меню "Пуск".|
|startMenuHideRecentJumpLists|Boolean (логический)|Эта политика позволяет скрыть списки последних переходов в меню "Пуск" и на панели задач, а также отключить соответствующий переключатель в приложении "Параметры".|
|startMenuHideRecentlyAddedApps|Boolean (логический)|Эта политика позволяет скрыть недавно добавленные приложения в меню "Пуск" и отключить соответствующий переключатель в приложении "Параметры".|
|startMenuHideRestartOptions|Boolean (логический)|Эта политика позволяет скрыть параметр кнопки питания "Перезагрузить" или "Обновить и перезагрузить" в меню "Пуск".|
|startMenuHideShutDown|Boolean (логический)|Эта политика позволяет скрыть параметр кнопки питания "Завершить работу" или "Обновить и завершить работу" в меню "Пуск".|
|startMenuHideSignOut|Boolean (логический)|Эта политика позволяет скрыть параметр для выхода из учетной записи на плитке пользователя в меню "Пуск".|
|startMenuHideSleep|Boolean (логический)|Эта политика позволяет скрыть параметр кнопки питания для перехода в спящий режим в меню "Пуск".|
|startMenuHideSwitchAccount|Boolean (логический)|Эта политика позволяет скрыть параметр для переключения между учетными записями на плитке пользователя в меню "Пуск".|
|startMenuHideUserTile|Boolean (логический)|Эта политика позволяет скрыть плитку пользователя в меню "Пуск".|
|startMenuLayoutEdgeAssetsXml|Binary|Этот параметр политики позволяет импортировать ресурсы Edge для использования с политикой startMenuLayoutXml. Макет меню "Пуск" может содержать вспомогательную плитку из приложения Edge для поиска файла локального ресурса Edge. Так как локальный ресурс Edge не существует, вспомогательная плитка Edge будет пустой. Эта политика применяется только при изменении политики startMenuLayoutXml. Значение должно быть в формате массива байтов в кодировке Base64 UTF-8.|
|startMenuLayoutXml|Binary|Позволяет администраторам переопределять стандартный макет меню "Пуск" и блокировать его изменение пользователями. Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета. XML-файл должен быть в формате массива байтов в кодировке UTF8.|
|startMenuMode|[windowsStartMenuModeType](../resources/intune_deviceconfig_windowsstartmenumodetype.md)|Позволяет администраторам определить вид меню "Пуск". Возможные значения: `userDefined`, `fullScreen`, `nonFullScreen`.|
|startMenuPinnedFolderDocuments|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Определяет, виден ли ярлык папки "Документы" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderDownloads|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Определяет, виден ли ярлык папки "Загрузки" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderFileExplorer|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Определяет, виден ли ярлык проводника в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderHomeGroup|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Определяет, виден ли ярлык папки "Домашняя группа" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderMusic|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Определяет, виден ли ярлык папки "Музыка" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderNetwork|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Определяет, виден ли ярлык папки "Сеть" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPersonalFolder|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Определяет, виден ли ярлык личной папки в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPictures|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Определяет, виден ли ярлык папки "Изображения" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderSettings|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Определяет, виден ли ярлык папки "Параметры" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderVideos|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Определяет, виден ли ярлык папки "Видео" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|settingsBlockSettingsApp|Boolean (логический)|Указывает, следует ли заблокировать доступ к приложению "Параметры".|
|settingsBlockSystemPage|Boolean (логический)|Указывает, следует ли заблокировать доступ к разделу "Система" в приложении "Параметры".|
|settingsBlockDevicesPage|Boolean (логический)|Указывает, следует ли заблокировать доступ к разделу "Устройства" в приложении "Параметры".|
|settingsBlockNetworkInternetPage|Boolean (логический)|Указывает, следует ли заблокировать доступ к разделу "Сеть и Интернет" в приложении "Параметры".|
|settingsBlockPersonalizationPage|Boolean (логический)|Указывает, следует ли заблокировать доступ к разделу "Персонализация" в приложении "Параметры".|
|settingsBlockAccountsPage|Boolean (логический)|Указывает, следует ли заблокировать доступ к разделу "Учетные записи" в приложении "Параметры".|
|settingsBlockTimeLanguagePage|Boolean (логический)|Указывает, следует ли заблокировать доступ к разделу "Время и язык" в приложении "Параметры".|
|settingsBlockEaseOfAccessPage|Boolean (логический)|Указывает, следует ли заблокировать доступ к разделу "Специальные возможности" в приложении "Параметры".|
|settingsBlockPrivacyPage|Boolean (логический)|Указывает, следует ли заблокировать доступ к разделу "Конфиденциальность" в приложении "Параметры".|
|settingsBlockUpdateSecurityPage|Boolean (логический)|Указывает, следует ли заблокировать доступ к разделу "Обновление и безопасность" в приложении "Параметры".|
|settingsBlockAppsPage|Boolean (логический)|Указывает, следует ли заблокировать доступ к разделу "Приложения" в приложении "Параметры".|
|settingsBlockGamingPage|Boolean (логический)|Указывает, следует ли заблокировать доступ к разделу "Игры" в приложении "Параметры".|
|windowsSpotlightBlockConsumerSpecificFeatures|Boolean (логический)|Позволяет ИТ-администраторам заблокировать функции, обычно доступные только для потребителей, такие как рекомендации в меню "Пуск", уведомления, связанные с членством в группе, установка приложений после запуска при первом включении компьютера и плитки перенаправления.|
|windowsSpotlightBlocked|Boolean (логический)|Позволяет ИТ-администраторам отключить все функции "Windows: интересное".|
|windowsSpotlightBlockOnActionCenter|Boolean (логический)|Позволяет запретить Майкрософт показывать информацию о новых возможностях или изменениях после каждой чистой установки операционной системы, обновления или на постоянной основе.|
|windowsSpotlightBlockTailoredExperiences|Boolean (логический)|Позволяет заблокировать персонализацию контента на экране "Windows: интересное" на основе данных об использовании устройства.|
|windowsSpotlightBlockThirdPartyNotifications|Boolean (логический)|Позволяет заблокировать сторонний контент на экране "Windows: интересное".|
|windowsSpotlightBlockWelcomeExperience|Boolean (логический)|Позволяет заблокировать экран приветствия "Windows: интересное".|
|windowsSpotlightBlockWindowsTips|Boolean (логический)|Позволяет ИТ-администраторам отключать всплывающие советы по использованию Windows.|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune_deviceconfig_windowsspotlightenablementsettings.md)|Указывает тип "в центре внимания". Возможные значения: `notConfigured`, `disabled`, `enabled`.|
|networkProxyApplySettingsDeviceWide|Boolean (логический)|Если этот параметр включен, настройки прокси-сервера применяются ко всем процессам и учетным записям на устройстве. В противном случае они применяются к учетной записи пользователя, зарегистрированной в системе MDM.|
|networkProxyDisableAutoDetect|Boolean (логический)|Позволяет отключить автоматическое обнаружение настроек. Если этот параметр включен, система попытается найти путь к сценарию автонастройки прокси-сервера (PAC).|
|networkProxyAutomaticConfigurationUrl|String (строка)|Адрес сценария автонастройки прокси-сервера (PAC).|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune_deviceconfig_windows10networkproxyserver.md)|Определяет ручные настройки прокси-сервера.|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean (логический)|Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.|
|antiTheftModeBlocked|Boolean (логический)|Указывает, следует ли запретить пользователю выбирать режим AntiTheft (только для Windows 10 Mobile).|
|bluetoothBlocked|Boolean (логический)|Указывает, следует ли запретить использовать Bluetooth.|
|cameraBlocked|Boolean (логический)|Определяет, следует ли запретить доступ к камере устройства.|
|connectedDevicesServiceBlocked|Boolean (логический)|Указывает, следует ли блокировать службу подключенных устройств, которая позволяет находить другие устройства и подключаться к ним, удаленно обмениваться сообщениями и работать с приложениями, а также выполнять другие действия.|
|certificatesBlockManualRootCertificateInstallation|Boolean (логический)|Указывает, следует ли запретить пользователю вручную устанавливать корневой сертификат.|
|copyPasteBlocked|Boolean (логический)|Указывает, следует ли запретить пользователю копировать данные.|
|cortanaBlocked|Boolean (логический)|Указывает, следует ли запретить использовать Кортану.|
|deviceManagementBlockFactoryResetOnMobile|Boolean (логический)|Указывает, следует ли запретить пользователю сбрасывать настройки телефона.|
|deviceManagementBlockManualUnenroll|Boolean (логический)|Указывает, следует ли запретить пользователю вручную отменять регистрацию в системе управления устройствами.|
|safeSearchFilter|[safeSearchFilterType](../resources/intune_deviceconfig_safesearchfiltertype.md)|Определяет необходимый уровень фильтрации для безопасного поиска. Возможные значения: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Boolean (логический)|Указывает, следует ли блокировать всплывающие окна.|
|edgeBlockSearchSuggestions|Boolean (логический)|Указывает, следует ли запретить использовать варианты поиска в адресной строке.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Boolean (логический)|Указывает, следует ли запретить пользователю отправлять трафик интрасети в Internet Explorer из Edge.|
|edgeRequireSmartScreen|Boolean (логический)|Указывает, обязательно ли использовать фильтр Smart Screen.|
|edgeEnterpriseModeSiteListLocation|String (строка)|Указывает расположение списка сайтов, запускаемых в корпоративном режиме. Это может быть локальный файл, локальная сеть или http-адрес.|
|edgeFirstRunUrl|String (строка)|URL-адрес, открываемый в браузере Edge при первом запуске.|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)|Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для управляемых с помощью системы MDM устройств. Пользователи могут переопределять эту настройку и изменять поисковую систему по умолчанию, если не установлена политика AllowSearchEngineCustomization.|
|edgeHomepageUrls|Коллекция String|Список URL-адресов домашних страниц, показываемых на зарегистрированных в системе MDM устройствах в браузере Edge.|
|edgeBlockAccessToAboutFlags|Boolean (логический)|Указывает, следует ли запретить доступ к странице about flags в браузере Edge.|
|smartScreenBlockPromptOverride|Boolean (логический)|Указывает, могут ли пользователи игнорировать предупреждения фильтра SmartScreen о потенциально вредоносных веб-сайтах.|
|smartScreenBlockPromptOverrideForFiles|Boolean (логический)|Указывает, могут ли пользователи игнорировать предупреждения фильтра SmartScreen о скачивании непроверенных файлов.|
|webRtcBlockLocalhostIpAddress|Boolean (логический)|Указывает, отображается ли IP-адрес пользователя localhost при совершении телефонных звонков с помощью WebRTC.|
|internetSharingBlocked|Boolean (логический)|Указывает, следует ли запретить использовать Общий Интернет.|
|settingsBlockAddProvisioningPackage|Boolean (логический)|Указывает, следует ли запретить пользователю устанавливать пакеты подготовки.|
|settingsBlockRemoveProvisioningPackage|Boolean (логический)|Указывает, следует ли запретить агенту конфигурации среды выполнения удалять пакеты подготовки.|
|settingsBlockChangeSystemTime|Boolean (логический)|Указывает, следует ли запретить пользователю изменять настройки даты и времени.|
|settingsBlockEditDeviceName|Boolean (логический)|Указывает, следует ли запретить пользователю изменять имя устройства.|
|settingsBlockChangeRegion|Boolean (логический)|Указывает, следует ли запретить пользователю изменять региональные стандарты.|
|settingsBlockChangeLanguage|Boolean (логический)|Указывает, следует ли запретить пользователю изменять параметры языка.|
|settingsBlockChangePowerSleep|Boolean (логический)|Указывает, следует ли запретить пользователю изменять параметры питания и спящего режима.|
|locationServicesBlocked|Boolean (логический)|Указывает, следует ли запретить использовать службы определения местоположения.|
|microsoftAccountBlocked|Boolean (логический)|Указывает, следует ли запретить использовать учетную запись Майкрософт.|
|microsoftAccountBlockSettingsSync|Boolean (логический)|Указывает, следует ли запретить синхронизировать настройки учетной записи Майкрософт.|
|nfcBlocked|Boolean (логический)|Указывает, следует ли запретить использовать NFC.|
|resetProtectionModeBlocked|Boolean (логический)|Указывает, следует ли запретить пользователю сбрасывать режим защиты.|
|screenCaptureBlocked|Boolean (логический)|Указывает, следует ли запретить пользователю делать снимки экрана.|
|storageBlockRemovableStorage|Boolean (логический)|Указывает, следует ли запретить использовать съемные носители.|
|storageRequireMobileDeviceEncryption|Boolean (логический)|Указывает, обязательно ли шифровать данные на мобильном устройстве.|
|usbBlocked|Boolean (логический)|Указывает, следует ли запретить пользователю подключать USB-устройства.|
|voiceRecordingBlocked|Boolean (логический)|Указывает, следует ли запретить пользователю записывать речь.|
|wiFiBlockAutomaticConnectHotspots|Boolean (логический)|Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi. Ни на что не влияет, если Wi-Fi заблокирован.|
|wiFiBlocked|Boolean (логический)|Указывает, следует ли запретить использовать Wi-Fi.|
|wiFiBlockManualConfiguration|Boolean (логический)|Указывает, следует ли запретить пользователю настраивать Wi-Fi вручную.|
|wiFiScanInterval|Int32|Указывает частоту поиска сетей Wi-Fi. Поддерживаемые значения: 1–500, где 100 — значение по умолчанию, а 500 — низкая частота. Допустимые значения: от 1 до 500.|
|wirelessDisplayBlockProjectionToThisDevice|Boolean (логический)|Указывает, могут ли другие устройства находить этот компьютер для проецирования контента.|
|wirelessDisplayBlockUserInputFromReceiver|Boolean (логический)|Указывает, следует ли блокировать запросы пользователя с беспроводного дисплея.|
|wirelessDisplayRequirePinForPairing|Boolean (логический)|Указывает, обязательно ли использовать ПИН-код для связывания с новыми устройствами.|
|windowsStoreBlocked|Boolean (логический)|Указывает, следует ли запретить использовать Microsoft Store.|
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Указывает, можно ли загружать неопубликованные приложения из пакетов AppX с доверенным сертификатом. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|windowsStoreBlockAutoUpdate|Boolean (логический)|Указывает, следует ли заблокировать автоматическое обновление приложений из Microsoft Store.|
|developerUnlockSetting|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Указывает, следует ли разрешить разблокировку для разработки. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|sharedUserAppDataAllowed|Boolean (логический)|Указывает, следует ли запретить общий доступ к данным для пользователей одного приложения.|
|appsBlockWindowsStoreOriginatedApps|Boolean (логический)|Указывает, следует ли отключить запуск всех предустановленных или скачанных приложений из Microsoft Store.|
|windowsStoreEnablePrivateStoreOnly|Boolean (логический)|Указывает, следует ли включить только частный магазин.|
|storageRestrictAppDataToSystemVolume|Boolean (логический)|Указывает, можно ли хранить данные приложения не на системном диске.|
|storageRestrictAppInstallToSystemVolume|Boolean (логический)|Указывает, можно ли устанавливать приложения не на системном диске.|
|gameDvrBlocked|Boolean (логический)|Указывает, следует ли блокировать DVR и трансляцию контента.|
|experienceBlockDeviceDiscovery|Boolean (логический)|Указывает, следует ли блокировать обнаружение устройств.|
|experienceBlockErrorDialogWhenNoSIM|Boolean (логический)|Указывает, следует ли запретить отображение диалогового окна ошибки, если SIM-карта не обнаружена.|
|experienceBlockTaskSwitcher|Boolean (логический)|Указывает, следует ли заблокировать переключение задач на устройстве.|
|logonBlockFastUserSwitching|Boolean (логический)|Отключает возможность быстрого переключения между учетными записями пользователей, вошедших в систему, без выхода из системы.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) в теле ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 9767

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9875

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true
}
```



