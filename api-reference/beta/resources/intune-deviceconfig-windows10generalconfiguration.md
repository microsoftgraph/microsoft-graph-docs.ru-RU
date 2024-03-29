---
title: Тип ресурса windows10GeneralConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windows10GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 809d9b1b28b922040d80c7a00426f8a2aee8d128
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669541"
---
# <a name="windows10generalconfiguration-resource-type"></a>Тип ресурса windows10GeneralConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windows10GeneralConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов Windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-list.md)|Коллекция [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Перечисление свойств и связей объектов [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Получение объекта windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-get.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Чтение свойств и связей объекта [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Создание объекта windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-create.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Создание объекта [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Удаление объекта windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-delete.md)|Нет|Удаление объекта [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Обновление объекта windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-update.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Обновление свойств объекта [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Идентификаторы roleScopeTagId|Коллекция строк|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false и сущности не будут видны пользователям с заданной областью. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удалив и повторно создав политику на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|taskManagerBlockEndTask|Логический|Укажите, могут ли администраторы использовать диспетчер задач для завершения задач.|
|energySaverOnBatteryThresholdPercentage|Int32|Этот параметр позволяет указать уровень заряда батареи, на котором включена экономия энергии. Во время работы от батареи экономия энергии автоматически включается на указанном уровне заряда батареи (и ниже). Допустимый диапазон входных данных (0–100). Допустимые значения: от 0 до 100|
|energySaverPluggedInThresholdPercentage|Int32|Этот параметр позволяет указать уровень заряда батареи, на котором включена экономия энергии. При подключении энергосохранилка автоматически включается на указанном уровне заряда батареи (и ниже). Допустимый диапазон входных данных (0–100). Допустимые значения: от 0 до 100|
|powerLidCloseActionOnBattery|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр указывает действие, выполняемые Windows, когда пользователь закрывает крышку на мобильном компьютере во время работы от батареи. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerLidCloseActionPluggedIn|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр указывает действие, выполняемые Windows, когда пользователь закрывает крышку на мобильном компьютере при подключении. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerButtonActionOnBattery|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр задает действие, выполняемые Windows, когда пользователь нажимает кнопку питания во время работы от батареи. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerButtonActionPluggedIn|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр указывает действие, выполняемые Windows, когда пользователь нажимает кнопку Питания при подключении. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerSleepButtonActionOnBattery|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр указывает действие, выполняемые Windows, когда пользователь нажимает кнопку "Спящий режим" во время работы от батареи. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerSleepButtonActionPluggedIn|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр указывает действие, выполняемые Windows, когда пользователь нажимает кнопку "Спящий режим" при подключении. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerHybridSleepOnBattery|[Включения](../resources/intune-deviceconfig-enablement.md)|Этот параметр позволяет отключить гибридный спящий режим во время работы от батареи. Если этот параметр отключен, гибернация не создается при переходе системы в спящий режим (в режиме ожидания). Если этот параметр включен или не настроен, пользователи могут управлять этим параметром. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|powerHybridSleepPluggedIn|[Включения](../resources/intune-deviceconfig-enablement.md)|Этот параметр позволяет отключить гибридный спящий режим при подключении. Если этот параметр отключен, гибернация не создается при переходе системы в спящий режим (в режиме ожидания). Если этот параметр включен или не настроен, пользователи могут управлять этим параметром. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|windows10AppsForceUpdateSchedule|[windows10AppsForceUpdateSchedule](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|Windows 10 принудительное обновление приложений.|
|enableAutomaticRedeployment|Логическое|Разрешите пользователям с правами администратора удалять все пользовательские данные и параметры с помощью клавиш CTRL+ Win +R на экране блокировки устройства, чтобы устройство можно было автоматически перенастроить и повторно зарегистрировать в управлении.|
|microsoftAccountSignInAssistantSettings|[signInAssistantOptions](../resources/intune-deviceconfig-signinassistantoptions.md)|Управляет службой NT Sign-In учетной записи Майкрософт (wlidsvc). Возможные значения: `notConfigured`, `disabled`.|
|authenticationAllowSecondaryDevice|Логическое|Позволяет дополнительным устройствам проверки подлинности работать с Windows.|
|authenticationWebSignIn|[Включения](../resources/intune-deviceconfig-enablement.md)|Указывает, будет ли включен поставщик веб-учетных данных. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|authenticationPreferredAzureADTenantDomainName|String|Указывает предпочтительный домен среди доступных доменов в Azure AD клиента.|
|cryptographyAllowFipsAlgorithmPolicy|Логическое|Укажите, следует ли разрешать или запрещать политику FiPS.|
|displayAppListWithGdiDPIScalingTurnedOn|Коллекция String|Список устаревших приложений, для которых включено масштабирование DPI GDI.|
|displayAppListWithGdiDPIScalingTurnedOff|Коллекция объектов string|Список устаревших приложений, для которых отключено масштабирование DPI GDI.|
|enterpriseCloudPrintDiscoveryEndPoint|String|Конечная точка для обнаружения облачных принтеров.|
|enterpriseCloudPrintOAuthAuthority|String|Конечная точка аутентификации для получения токенов OAuth.|
|enterpriseCloudPrintOAuthClientIdentifier|String|GUID клиентского приложения, которому разрешено получать токены OAuth из системы OAuth.|
|enterpriseCloudPrintResourceIdentifier|String|URI ресурса OAuth для службы печати, настроенный на портале Azure.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Максимальное количество принтеров, запрашиваемых с конечной точки обнаружения. Этот параметр применяется только к мобильным устройствам. Допустимые значения: от 1 до 65 535.|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String|URI ресурса OAuth для службы обнаружения принтеров, настроенный на портале Azure.|
|experienceDoNotSyncBrowserSettings|[browserSyncSetting](../resources/intune-deviceconfig-browsersyncsetting.md)|Разрешить или запретить синхронизацию параметров браузера Microsoft Edge. ИТ-администраторы могут запретить синхронизацию между устройствами, но разрешить переопределение пользователей. Возможные значения: `notConfigured`, `blockedWithUserOverride`, `blocked`.|
|messagingBlockSync|Логический|Указывает, следует ли блокировать резервное копирование и восстановление текстовых сообщений и отправку сообщений везде.|
|messagingBlockMMS|Логическое|Указывает, следует ли блокировать функцию отправки и получения MMS на устройстве.|
|messagingBlockRichCommunicationServices|Логическое|Указывает, следует ли блокировать функцию отправки и получения RCS на устройстве.|
|printerNames|Коллекция объектов string|Автоматическая подготовка принтеров на основе их имен (имен сетевых узлов).|
|printerDefaultName|String|Имя (сетевое имя узла) установленного принтера.|
|printerBlockAddition|Логическое|Запретить пользователю установку дополнительных принтеров из параметров принтеров.|
|searchBlockDiacritics|Boolean|Указывает, можно ли использовать диакритические знаки в поиске.|
|searchDisableAutoLanguageDetection|Boolean|Указывает, следует ли использовать автоматическое определение языка при индексировании контента и свойств.|
|searchDisableIndexingEncryptedItems|Boolean|Указывает, следует ли запретить индексирование защищенных WIP элементов, чтобы они не отображались в результатах поиска Кортаны или проводника.|
|searchEnableRemoteQueries|Boolean|Указывает, следует ли заблокировать удаленные запросы к индексу этого компьютера.|
|searchDisableUseLocation|Boolean|Указывает, может ли поиск использовать сведения о расположении.|
|searchDisableLocation|Логическое|Указывает, может ли поиск использовать сведения о расположении.|
|searchDisableIndexerBackoff|Boolean|Указывает, следует ли отключить функцию отхода индексатора поиска.|
|searchDisableIndexingRemovableDrive|Boolean|Указывает, могут ли пользователи добавлять расположения на съемных дисках в библиотеки и для индексирования.|
|searchEnableAutomaticIndexSizeManangement|Boolean|Указывает минимальный объем памяти на жестком диске с индексом до остановки индексирования.|
|searchBlockWebResults|Логическое|Указывает, следует ли блокировать поиск в Интернете.|
|findMyFiles|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, может ли пользователь настроить поиск в режиме поиска "Мои файлы", который выполняет поиск файлов на вторичных жестких дисках, а также за пределами профиля пользователя. Функция "Найти мои файлы" не позволяет пользователям искать файлы или расположения, к которым у них нет доступа. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityBlockAzureADJoinedDevicesAutoEncryption|Логическое|Укажите, следует ли разрешить автоматическое шифрование устройства при первом включении при Azure AD устройства (только для настольных компьютеров).|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|Возвращает или задает значение, позволяющее устройству отправлять данные диагностики и телеметрии использования, такие как Watson. Возможные значения: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Boolean|Возвращает или задает значение, позволяющее ИТ-администраторам запретить работу приложений и функций с файлами в OneDrive.|
|systemTelemetryProxyServer|String|Возвращает или задает полное доменное имя (FQDN) или IP-адрес прокси-сервера для пересылки запросов подключенных пользователей и телеметрии.|
|edgeTelemetryForMicrosoft365Analytics|[edgeTelemetryMode](../resources/intune-deviceconfig-edgetelemetrymode.md)|Указывает, какой тип данных телеметрии (none, intranet, internet, both) отправляется в Аналитику Microsoft 365. Возможные значения: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.|
|inkWorkspaceAccess|[inkAccessSetting](../resources/intune-deviceconfig-inkaccesssetting.md)|Управляет доступом пользователя к рабочей области рукописного ввода с рабочего стола и сверху экрана блокировки. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|inkWorkspaceAccessState|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Управляет доступом пользователя к рабочей области рукописного ввода с рабочего стола и сверху экрана блокировки. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|inkWorkspaceBlockSuggestedApps|Boolean|Укажите, следует ли отображать рекомендуемые предложения приложений в рабочей области рукописного ввода.|
|smartScreenEnableAppInstallControl|Boolean|Это свойство будет нерекомендуемым в июле 2019 г. и будет заменено свойством SmartScreenAppInstallControl. Позволяет ИТ-администраторам разрешать или запрещать установку приложений из мест, отличных от Store.|
|smartScreenAppInstallControl|[appInstallControlType](../resources/intune-deviceconfig-appinstallcontroltype.md)|Добавлено в Windows 10 версии 1703. Позволяет ИТ-администраторам разрешать или запрещать установку приложений из мест, отличных от Store. Возможные значения: `notConfigured`, `anywhere`, `storeOnly`, `recommendations`, `preferStore`.|
|personalizationDesktopImageUrl|String|Начинающийся с http или https URL-адрес изображения в формате JPG, JPEG или PNG, которое необходимо скачать и разместить на рабочем столе, или URL-адрес локального изображения в файловой системе, которое нужно разместить на рабочем столе.|
|personalizationLockScreenImageUrl|String|Начинающийся с http или https URL-адрес изображения в формате JPG, JPEG или PNG, которое необходимо скачать и разместить на экране блокировки, или URL-адрес локального изображения в файловой системе, которое нужно разместить на экране блокировки.|
|bluetoothAllowedServices|Коллекция String|Укажите список разрешенных служб и профилей Bluetooth в шестнадцатеричном формате.|
|bluetoothBlockAdvertising|Boolean|Указывает, следует ли запретить использовать рекламу по Bluetooth.|
|BluetoothBlockPromptedProximalConnections|Логическое|Следует ли запретить пользователям использовать быстрая связь и другие сценарии на основе близкого взаимодействия.|
|bluetoothBlockDiscoverableMode|Boolean|Указывает, следует ли запретить использовать режим обнаружения по Bluetooth.|
|bluetoothBlockPrePairing|Boolean|Указывает, следует ли заблокировать автоматическое связывание отдельных пакетных периферийных устройств Bluetooth с главным устройством.|
|edgeBlockAutofill|Boolean|Указывает, следует ли заблокировать автозаполнение.|
|edgeBlocked|Boolean|Указывает, следует ли запретить использовать браузер Edge.|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune-deviceconfig-edgecookiepolicy.md)|Указывает, какие файлы cookie следует блокировать в браузере Edge. Возможные значения: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeBlockDeveloperTools|Boolean|Указывает, следует ли заблокировать средства разработчика в браузере Edge.|
|edgeBlockSendingDoNotTrackHeader|Boolean|Указывает, следует ли запретить пользователю отправлять заголовок DNT.|
|edgeBlockExtensions|Boolean|Указывает, следует ли заблокировать расширения в браузере Edge.|
|edgeBlockInPrivateBrowsing|Boolean|Указывает, следует ли заблокировать просмотр InPrivate в корпоративных сетях в браузере Edge.|
|edgeBlockJavaScript|Boolean|Указывает, следует ли запретить использовать JavaScript.|
|edgeBlockPasswordManager|Boolean|Указывает, следует ли заблокировать диспетчер паролей.|
|edgeBlockAddressBarDropdown|Boolean|Позволяет заблокировать раскрывающийся список адресной строки в Microsoft Edge. Отключите этот параметр, чтобы уменьшить количество сетевых подключений Microsoft Edge к службам Майкрософт.|
|edgeBlockCompatibilityList|Boolean|Позволяет заблокировать список совместимости Майкрософт в Microsoft Edge. Этот список помогает Edge правильно отображать сайты с известными проблемами совместимости.|
|edgeClearBrowsingDataOnExit|Boolean|Указывает, следует ли удалять данные просмотра при выходе из Microsoft Edge.|
|edgeAllowStartPagesModification|Boolean|Указывает, могут ли пользователи изменять начальные страницы в Edge. Используйте свойство EdgeHomepageUrls, чтобы указать начальные страницы по умолчанию, отображаемые при открытии Edge.|
|edgeDisableFirstRunPage|Boolean|Позволяет заблокировать веб-страницу Майкрософт, которая открывается при первом запуске Microsoft Edge. Эта политика позволяет предприятиям, зарегистрированным в конфигурациях с нулевым выбросом, блокировать эту страницу.|
|edgeBlockLiveTileDataCollection|Boolean|Позволяет запретить Майкрософт собирать информацию о создании живых плиток, когда пользователи закрепляют сайты из Microsoft Edge на начальном экране.|
|edgeSyncFavoritesWithInternetExplorer|Boolean|Указывает, следует ли включить синхронизацию избранного между Internet Explorer и Microsoft Edge. Браузеры обмениваются данными о добавлении, удалении и изменении избранных элементов, а также их порядка.|
|edgeFavoritesListLocation|String|Расположение списка избранного для подготовки. Это может быть локальный файл, локальная сеть или HTTP-адрес.|
|edgeBlockEditFavorites|Логический|Указывает, следует ли запретить пользователю вносить изменения в избранное.|
|edgeNewTabPageURL|String|Укажите страницу, открываемую при создании новых вкладок.|
|edgeHomeButtonConfiguration|[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|Приводит к скрытию кнопки "Главная", загрузке начальной страницы по умолчанию, загрузке страницы вкладки "Создать" или пользовательскому URL-адресу|
|edgeHomeButtonConfigurationEnabled|Логическое|Включите конфигурацию кнопки "Главная".|
|edgeOpensWith|[edgeOpenOptions](../resources/intune-deviceconfig-edgeopenoptions.md)|Укажите, какие страницы открыты в начале. Возможные значения: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.|
|edgeBlockSideloadingExtensions|Логический|Указывает, может ли пользователь загрузить расширения неопубликованных приложений.|
|edgeRequiredExtensionPackageFamilyNames|Коллекция String|Укажите список имен семейств пакетов расширений браузера, которые являются обязательными и не могут быть отключены пользователем.|
|edgeBlockPrinting|Логическое|Настройте Edge для разрешения или блокировки печати.|
|edgeFavoritesBarVisibility|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Возвращает или задает значение, указывающее, следует ли всегда отображать или скрывать панель избранного на любой странице. Возможные значения: `notConfigured`, `hide`, `show`.|
|edgeBlockSavingHistory|Логическое|Настройте Edge, чтобы разрешить сохранение журнала браузера или никогда не сохранять журнал браузера.|
|edgeBlockFullScreenMode|Логическое|Разрешить или запретить edge вводить полноэкранный режим.|
|edgeBlockWebContentOnNewTabPage|Логическое|Настройте загрузку пустой страницы в Edge вместо страницы новой вкладки по умолчанию и запретить пользователям изменять ее.|
|edgeBlockTabPreloading|Логическое|Настройте, будет ли Edge предварительно загрузить новую страницу вкладки при запуске Windows.|
|edgeBlockPrelaunch|Логическое|Решите, будет ли Microsoft Edge предварительно запущен при запуске Windows.|
|edgeShowMessageWhenOpeningInternetExplorerSites|[internetExplorerMessageSetting](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|Управляет сообщением, отображаемое edge, перед переходом на Internet Explorer. Возможные значения: `notConfigured`, `disabled`, `enabled`, `keepGoing`.|
|edgePreventCertificateErrorOverride|Логическое|Разрешить или запретить пользователям переопределять ошибки сертификата.|
|edgeKioskModeRestriction|[edgeKioskModeRestrictionType](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|Управляет ограничением параметров Microsoft Edge в зависимости от режима настройки киоска. Возможные значения: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.|
|edgeKioskResetAfterIdleTimeInMinutes|Int32|Указывает время в минутах с момента последнего действия пользователя до сброса киоска Microsoft Edge.  Допустимые значения: 0–1440. Значение по умолчанию равно 5. Значение 0 означает отсутствие сброса. Допустимые значения от 0 до 1440|
|cellularBlockDataWhenRoaming|Boolean|Указывает, следует ли запретить использовать мобильные данные в роуминге.|
|cellularBlockVpn|Boolean|Указывает, следует ли запретить использовать VPN по сотовой сети.|
|cellularBlockVpnWhenRoaming|Boolean|Указывает, следует ли запретить использовать VPN по сотовой сети в роуминге.|
|cellularData|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает, следует ли разрешить канал передачи данных на устройстве. Если этот параметр не настроен, канал передачи данных разрешен, и пользователь может отключить его. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|defenderRequireRealTimeMonitoring|Boolean|Указывает, обязательно ли использовать мониторинг в режиме реального времени.|
|defenderRequireBehaviorMonitoring|Boolean|Указывает, обязательно ли использовать наблюдение за поведением.|
|defenderRequireNetworkInspectionSystem|Boolean|Указывает, обязательно ли использовать систему проверки сети.|
|defenderScanDownloads|Boolean|Указывает, следует ли проверять загрузки.|
|defenderScheduleScanEnableLowCpuPriority|Логическое|Если этот параметр включен, во время запланированных проверок будет использоваться низкий приоритет ЦП.|
|defenderDisableCatchupQuickScan|Логическое|Если эта функция заблокирована, дополнительные проверки на наличие запланированных быстрых проверок будут отключены.|
|defenderDisableCatchupFullScan|Логическое|При блокировке дополнительные проверки на наличие запланированных полных проверок будут отключены.|
|defenderScanScriptsLoadedInInternetExplorer|Boolean|Указывает, следует ли проверять сценарии, загружаемые в браузере Internet Explorer.|
|defenderBlockEndUserAccess|Boolean|Указывает, следует ли заблокировать доступ пользователей к Защитнику.|
|defenderSignatureUpdateIntervalInHours|Int32|Интервал обновления сигнатур (в часах). Укажите 0, чтобы не проверять. Допустимые значения: от 0 до 24.|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|Значение для отслеживания действий с файлами. Возможные значения: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Время до удаления вредоносного ПО на карантине (в днях). Допустимые значения: от 0 до 90.|
|defenderScanMaxCpu|Int32|Максимальный процент загрузки ЦП во время проверки. Допустимые значения: от 0 до 100|
|defenderScanArchiveFiles|Boolean|Указывает, следует ли проверять архивные файлы.|
|defenderScanIncomingMail|Boolean|Указывает, следует ли проверять входящую почту.|
|defenderScanRemovableDrivesDuringFullScan|Boolean|Указывает, следует ли сканировать съемные диски во время полной проверки.|
|defenderScanMappedNetworkDrivesDuringFullScan|Boolean|Указывает, следует ли сканировать подключенные сетевые диски во время полной проверки.|
|defenderScanNetworkFiles|Boolean|Указывает, следует ли сканировать файлы, открытые из сетевой папки.|
|defenderRequireCloudProtection|Boolean|Указывает, обязательно ли использовать облачную защиту.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Определяет уровень облачной защиты. Возможные значения: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|defenderCloudExtendedTimeout|Int32|Расширение времени ожидания для сканирования файлов в облаке. Допустимые значения: от 0 до 50.|
|defenderCloudExtendedTimeoutInSeconds|Int32|Расширение времени ожидания для сканирования файлов в облаке. Допустимые значения: от 0 до 50.|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|Позволяет указать, нужно ли спрашивать пользователя перед отправкой образцов. Возможные значения: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderScheduledQuickScanTime|TimeOfDay|Время ежедневной быстрой проверки.|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|Тип проверки системы Защитником. Возможные значения: `userDefined`, `disabled`, `quick`, `full`.|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|День проверки системы Защитником. Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.|
|defenderScheduledScanTime|TimeOfDay|Время проверки системы Защитником.|
|defenderPotentiallyUnwantedAppAction|[defenderPotentiallyUnwantedAppAction](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|Возвращает или задает действие Защитника для выполнения действий с потенциально нежелательными приложениями (PUA), которое включает программное обеспечение с поведением внедрения рекламных программ, объединение программного обеспечения, постоянное запрашивание оплаты или подписки и т. д. Defender оповещений пользователя при загрузке PUA или попытке установить себя. Добавлено в Windows 10 для настольных компьютеров. Возможные значения: `deviceDefault`, `block`, `audit`.|
|defenderPotentiallyUnwantedAppActionSetting|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Возвращает или задает действие Защитника для выполнения действий с потенциально нежелательными приложениями (PUA), которое включает программное обеспечение с поведением внедрения рекламных программ, объединение программного обеспечения, постоянное запрашивание оплаты или подписки и т. д. Defender оповещений пользователя при загрузке PUA или попытке установить себя. Добавлено в Windows 10 для настольных компьютеров. Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md);|Проверяет уровень согласия пользователя в Защитник Windows для отправки данных. Возможные значения: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|defenderBlockOnAccessProtection|Логическое|Разрешает или запрещает использование Защитник Windows on Access Protection.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Возвращает или задает действия Защитника в отношении обнаруженного вредоносного ПО для каждого уровня угрозы.|
|defenderFileExtensionsToExclude|Коллекция String|Расширения файлов, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderFilesAndFoldersToExclude|Коллекция String|Файлы и папки, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderProcessesToExclude|Коллекция String|Процессы, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|lockScreenAllowTimeoutConfiguration|Boolean|Указывает, следует ли отображать настройку, позволяющую определить время до отключения экрана на экране блокировки мобильных устройств с Windows 10. Если для этой политики установлено значение Allow, значение, заданное свойством lockScreenTimeoutInSeconds, игнорируется.|
|lockScreenBlockActionCenterNotifications|Boolean|Указывает, следует ли запретить показ уведомлений из центра уведомлений на экране блокировки.|
|lockScreenBlockCortana|Boolean|Указывает, может ли пользователь взаимодействовать с Кортаной с помощью голоса при заблокированной системе.|
|lockScreenBlockToastNotifications|Boolean|Указывает, следует ли показывать всплывающие уведомления на экране блокировки устройства.|
|lockScreenTimeoutInSeconds|Int32|Установите время (в секундах) от блокировки экрана до его выключения для мобильных устройств с Windows 10. Поддерживаемые значения: от 11 до 1800. Допустимые значения: от 11 до 1800.|
|lockScreenActivateAppsWithVoice|[Включения](../resources/intune-deviceconfig-enablement.md)|Этот параметр политики указывает, могут ли приложения Windows активироваться голосовой связью во время блокировки системы. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|passwordBlockSimple|Boolean|Укажите, разрешены ли такие ПИН-коды или пароли, как "1111" или "1234". Это свойство также контролирует использование графических паролей на компьютерах с Windows 10.|
|passwordExpirationDays|Int32|Срок действия пароля (в днях). Допустимые значения: от 0 до 730.|
|passwordMinimumLength|Int32|Минимальная длина пароля. Допустимые значения: от 4 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые требуются для пароля.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, повторное использование которых необходимо запретить. Допустимые значения: от 0 до 50.|
|passwordRequired|Boolean|Указывает, обязательно ли использовать пароль.|
|passwordRequireWhenResumeFromIdleState|Boolean|Указывает, следует ли запрашивать пароль при выходе из состояния простоя.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек. Допустимые значения: от 0 до 999.|
|passwordMinimumAgeInDays|Int32|Этот параметр безопасности определяет период времени (в днях), в течение которого пароль должен использоваться, прежде чем пользователь сможет изменить его. Допустимые значения от 0 до 998|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Указывает, можно ли использовать идентификатор рекламы. Добавлено в Windows 10 версии 1607. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Boolean|Указывает, следует ли запретить автоматическое принятие примечаний о связывании и конфиденциальности при запуске приложений.|
|privacyDisableLaunchExperience|Логическое|Эта политика предотвращает запуск функции конфиденциальности во время входа новых и обновленных пользователей.|
|privacyBlockInputPersonalization|Boolean|Указывает, следует ли запретить использовать облачные службы распознавания речи для приложений "Кортана", "Диктофон" или Store.|
|privacyBlockPublishUserActivities|Логическое|Блокирует общие возможности и обнаружение недавно использовавшихся ресурсов в переключателях задач и т. д.|
|privacyBlockActivityFeed|Логическое|Блокирует использование облачных служб распознавания речи для приложений Кортаны, Диктовки или Магазина.|
|activateAppsWithVoice|[Включения](../resources/intune-deviceconfig-enablement.md)|Указывает, можно ли активировать приложения Для Windows с помощью голосовой связи. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|startBlockUnpinningAppsFromTaskbar|Boolean|Указывает, следует ли запретить пользователю откреплять приложения с панели задач.|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|Эта политика позволяет свернуть список приложений, полностью удалить этот список или отключить соответствующий переключатель в приложении "Параметры". Возможные значения: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
|startMenuHideChangeAccountSettings|Boolean|Эта политика позволяет скрыть параметр для смены учетной записи на плитке пользователя в меню "Пуск".|
|startMenuHideFrequentlyUsedApps|Boolean|Эта политика позволяет скрыть наиболее часто используемые приложения в меню "Пуск" и отключить соответствующий переключатель в приложении "Параметры".|
|startMenuHideHibernate|Boolean|Эта политика позволяет скрыть параметр кнопки питания для перехода в режим гибернации в меню "Пуск".|
|startMenuHideLock|Boolean|Эта политика позволяет скрыть параметр для блокировки экрана на плитке пользователя в меню "Пуск".|
|startMenuHidePowerButton|Boolean|Эта политика позволяет скрыть кнопку питания в меню "Пуск".|
|startMenuHideRecentJumpLists|Boolean|Эта политика позволяет скрыть списки последних переходов в меню "Пуск" и на панели задач, а также отключить соответствующий переключатель в приложении "Параметры".|
|startMenuHideRecentlyAddedApps|Boolean|Эта политика позволяет скрыть недавно добавленные приложения в меню "Пуск" и отключить соответствующий переключатель в приложении "Параметры".|
|startMenuHideRestartOptions|Boolean|Эта политика позволяет скрыть параметр кнопки питания "Перезагрузить" или "Обновить и перезагрузить" в меню "Пуск".|
|startMenuHideShutDown|Boolean|Эта политика позволяет скрыть параметр кнопки питания "Завершить работу" или "Обновить и завершить работу" в меню "Пуск".|
|startMenuHideSignOut|Boolean|Эта политика позволяет скрыть параметр для выхода из учетной записи на плитке пользователя в меню "Пуск".|
|startMenuHideSleep|Boolean|Эта политика позволяет скрыть параметр кнопки питания для перехода в спящий режим в меню "Пуск".|
|startMenuHideSwitchAccount|Boolean|Эта политика позволяет скрыть параметр для переключения между учетными записями на плитке пользователя в меню "Пуск".|
|startMenuHideUserTile|Boolean|Эта политика позволяет скрыть плитку пользователя в меню "Пуск".|
|startMenuLayoutEdgeAssetsXml|Binary|Этот параметр политики позволяет импортировать ресурсы Edge для использования с политикой startMenuLayoutXml. Макет меню "Пуск" может содержать вспомогательную плитку из приложения Edge для поиска файла локального ресурса Edge. Так как локальный ресурс Edge не существует, вспомогательная плитка Edge будет пустой. Эта политика применяется только при изменении политики startMenuLayoutXml. Значение должно быть в формате массива байтов в кодировке Base64 UTF-8.|
|startMenuLayoutXml|Binary|Позволяет администраторам переопределять стандартный макет меню "Пуск" и блокировать его изменение пользователями. Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета. XML-файл должен быть в формате массива байтов в кодировке UTF8.|
|startMenuMode|[windowsStartMenuModeType](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|Позволяет администраторам определить вид меню "Пуск". Возможные значения: `userDefined`, `fullScreen`, `nonFullScreen`.|
|startMenuPinnedFolderDocuments|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Документы" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderDownloads|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Загрузки" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderFileExplorer|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык проводника в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderHomeGroup|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Домашняя группа" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderMusic|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Музыка" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderNetwork|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Сеть" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPersonalFolder|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык личной папки в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPictures|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Изображения" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderSettings|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Параметры" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderVideos|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Видео" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|settingsBlockSettingsApp|Boolean|Указывает, следует ли заблокировать доступ к приложению "Параметры".|
|settingsBlockSystemPage|Boolean|Указывает, следует ли заблокировать доступ к разделу "Система" в приложении "Параметры".|
|settingsBlockDevicesPage|Boolean|Указывает, следует ли заблокировать доступ к разделу "Устройства" в приложении "Параметры".|
|settingsBlockNetworkInternetPage|Boolean|Указывает, следует ли заблокировать доступ к разделу "Сеть и Интернет" в приложении "Параметры".|
|settingsBlockPersonalizationPage|Boolean|Указывает, следует ли заблокировать доступ к разделу "Персонализация" в приложении "Параметры".|
|settingsBlockAccountsPage|Boolean|Указывает, следует ли заблокировать доступ к разделу "Учетные записи" в приложении "Параметры".|
|settingsBlockTimeLanguagePage|Boolean|Указывает, следует ли заблокировать доступ к разделу "Время и язык" в приложении "Параметры".|
|settingsBlockEaseOfAccessPage|Boolean|Указывает, следует ли заблокировать доступ к разделу "Специальные возможности" в приложении "Параметры".|
|settingsBlockPrivacyPage|Boolean|Указывает, следует ли заблокировать доступ к разделу "Конфиденциальность" в приложении "Параметры".|
|settingsBlockUpdateSecurityPage|Boolean|Указывает, следует ли заблокировать доступ к разделу "Обновление и безопасность" в приложении "Параметры".|
|settingsBlockAppsPage|Boolean|Указывает, следует ли заблокировать доступ к разделу "Приложения" в приложении "Параметры".|
|settingsBlockGamingPage|Boolean|Указывает, следует ли заблокировать доступ к разделу "Игры" в приложении "Параметры".|
|windowsSpotlightBlockConsumerSpecificFeatures|Boolean|Позволяет ИТ-администраторам заблокировать функции, обычно доступные только для потребителей, такие как рекомендации в меню "Пуск", уведомления, связанные с членством в группе, установка приложений после запуска при первом включении компьютера и плитки перенаправления.|
|windowsSpotlightBlocked|Boolean|Позволяет ИТ-администраторам отключить все функции "Windows: интересное".|
|windowsSpotlightBlockOnActionCenter|Boolean|Позволяет запретить Майкрософт показывать информацию о новых возможностях или изменениях после каждой чистой установки операционной системы, обновления или на постоянной основе.|
|windowsSpotlightBlockTailoredExperiences|Boolean|Позволяет заблокировать персонализацию контента на экране "Windows: интересное" на основе данных об использовании устройства.|
|windowsSpotlightBlockThirdPartyNotifications|Boolean|Позволяет заблокировать сторонний контент на экране "Windows: интересное".|
|windowsSpotlightBlockWelcomeExperience|Boolean|Позволяет заблокировать экран приветствия "Windows: интересное".|
|windowsSpotlightBlockWindowsTips|Boolean|Позволяет ИТ-администраторам отключать всплывающие советы по использованию Windows.|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|Указывает тип Spotlight. Возможные значения: `notConfigured`, `disabled`, `enabled`.|
|networkProxyApplySettingsDeviceWide|Boolean|Если этот параметр включен, настройки прокси-сервера применяются ко всем процессам и учетным записям на устройстве. В противном случае они применяются к учетной записи пользователя, зарегистрированной в системе MDM.|
|networkProxyDisableAutoDetect|Boolean|Позволяет отключить автоматическое обнаружение настроек. Если этот параметр включен, система попытается найти путь к сценарию автонастройки прокси-сервера (PAC).|
|networkProxyAutomaticConfigurationUrl|String|Адрес сценария автонастройки прокси-сервера (PAC).|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune-deviceconfig-windows10networkproxyserver.md)|Определяет ручные настройки прокси-сервера.|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.|
|antiTheftModeBlocked|Boolean|Указывает, следует ли запретить пользователю выбирать режим AntiTheft (только для Windows 10 Mobile).|
|bluetoothBlocked|Boolean|Указывает, следует ли запретить использовать Bluetooth.|
|cameraBlocked|Boolean|Определяет, следует ли запретить доступ к камере устройства.|
|connectedDevicesServiceBlocked|Boolean|Указывает, следует ли блокировать службу подключенных устройств, которая позволяет находить другие устройства и подключаться к ним, удаленно обмениваться сообщениями и работать с приложениями, а также выполнять другие действия.|
|certificatesBlockManualRootCertificateInstallation|Boolean|Указывает, следует ли запретить пользователю вручную устанавливать корневой сертификат.|
|copyPasteBlocked|Boolean|Указывает, следует ли запретить пользователю копировать данные.|
|cortanaBlocked|Boolean|Указывает, следует ли запретить использовать Кортану.|
|deviceManagementBlockFactoryResetOnMobile|Boolean|Указывает, следует ли запретить пользователю сбрасывать настройки телефона.|
|deviceManagementBlockManualUnenroll|Boolean|Указывает, следует ли запретить пользователю вручную отменять регистрацию в системе управления устройствами.|
|safeSearchFilter|[safeSearchFilterType](../resources/intune-deviceconfig-safesearchfiltertype.md)|Определяет необходимый уровень фильтрации для безопасного поиска. Возможные значения: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Boolean|Указывает, следует ли блокировать всплывающие окна.|
|edgeBlockSearchSuggestions|Boolean|Указывает, следует ли запретить пользователю использовать предложения поиска в адресной строке.|
|edgeBlockSearchEngineCustomization|Логическое|Указывает, следует ли запретить пользователю добавлять новую поисковую систему или изменять поисковую систему по умолчанию.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Boolean|Указывает, следует ли переключать трафик интрасети с Edge на Internet Explorer. Примечание. Имя этого свойства вводит в заблуждение; Свойство устарело. Вместо этого используйте EdgeSendIntranetTrafficToInternetExplorer.|
|edgeSendIntranetTrafficToInternetExplorer|Логическое|Указывает, следует ли переключать трафик интрасети с Edge на Internet Explorer.|
|edgeRequireSmartScreen|Boolean|Указывает, обязательно ли использовать фильтр Smart Screen.|
|edgeEnterpriseModeSiteListLocation|String|Указывает расположение списка сайтов, запускаемых в корпоративном режиме. Это может быть локальный файл, локальная сеть или http-адрес.|
|edgeFirstRunUrl|String|URL-адрес, открываемый в браузере Edge при первом запуске.|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)|Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для управляемых с помощью системы MDM устройств. Пользователи могут переопределять эту настройку и изменять поисковую систему по умолчанию, если не установлена политика AllowSearchEngineCustomization.|
|edgeHomepageUrls|Коллекция String|Список URL-адресов домашних страниц, показываемых на зарегистрированных в системе MDM устройствах в браузере Edge.|
|edgeBlockAccessToAboutFlags|Boolean|Указывает, следует ли запретить доступ к странице about flags в браузере Edge.|
|smartScreenBlockPromptOverride|Boolean|Указывает, могут ли пользователи игнорировать предупреждения фильтра SmartScreen о потенциально вредоносных веб-сайтах.|
|smartScreenBlockPromptOverrideForFiles|Boolean|Указывает, могут ли пользователи игнорировать предупреждения фильтра SmartScreen о скачивании непроверенных файлов.|
|webRtcBlockLocalhostIpAddress|Boolean|Указывает, отображается ли IP-адрес пользователя localhost при совершении телефонных звонков с помощью WebRTC.|
|internetSharingBlocked|Boolean|Указывает, следует ли запретить использовать Общий Интернет.|
|settingsBlockAddProvisioningPackage|Boolean|Указывает, следует ли запретить пользователю устанавливать пакеты подготовки.|
|settingsBlockRemoveProvisioningPackage|Boolean|Указывает, следует ли запретить агенту конфигурации среды выполнения удалять пакеты подготовки.|
|settingsBlockChangeSystemTime|Boolean|Указывает, следует ли запретить пользователю изменять настройки даты и времени.|
|settingsBlockEditDeviceName|Boolean|Указывает, следует ли запретить пользователю изменять имя устройства.|
|settingsBlockChangeRegion|Boolean|Указывает, следует ли запретить пользователю изменять региональные стандарты.|
|settingsBlockChangeLanguage|Boolean|Указывает, следует ли запретить пользователю изменять параметры языка.|
|settingsBlockChangePowerSleep|Boolean|Указывает, следует ли запретить пользователю изменять параметры питания и спящего режима.|
|locationServicesBlocked|Boolean|Указывает, следует ли запретить использовать службы определения местоположения.|
|microsoftAccountBlocked|Boolean|Указывает, следует ли запретить использовать учетную запись Майкрософт.|
|microsoftAccountBlockSettingsSync|Boolean|Указывает, следует ли запретить синхронизировать настройки учетной записи Майкрософт.|
|nfcBlocked|Boolean|Указывает, следует ли запретить использовать NFC.|
|resetProtectionModeBlocked|Boolean|Указывает, следует ли запретить пользователю сбрасывать режим защиты.|
|screenCaptureBlocked|Boolean|Указывает, следует ли запретить пользователю делать снимки экрана.|
|storageBlockRemovableStorage|Boolean|Указывает, следует ли запретить использовать съемные носители.|
|storageRequireMobileDeviceEncryption|Boolean|Указывает, обязательно ли шифровать данные на мобильном устройстве.|
|usbBlocked|Boolean|Указывает, следует ли запретить пользователю подключать USB-устройства.|
|voiceRecordingBlocked|Boolean|Указывает, следует ли запретить пользователю записывать речь.|
|wiFiBlockAutomaticConnectHotspots|Boolean|Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi. Ни на что не влияет, если Wi-Fi заблокирован.|
|wiFiBlocked|Boolean|Указывает, следует ли запретить использовать Wi-Fi.|
|wiFiBlockManualConfiguration|Boolean|Указывает, следует ли запретить пользователю настраивать Wi-Fi вручную.|
|wiFiScanInterval|Int32|Указывает частоту поиска сетей Wi-Fi. Поддерживаемые значения: 1–500, где 100 — значение по умолчанию, а 500 — низкая частота. Допустимые значения: от 1 до 500.|
|wirelessDisplayBlockProjectionToThisDevice|Boolean|Указывает, могут ли другие устройства находить этот компьютер для проецирования контента.|
|wirelessDisplayBlockUserInputFromReceiver|Boolean|Указывает, следует ли блокировать запросы пользователя с беспроводного дисплея.|
|wirelessDisplayRequirePinForPairing|Boolean|Указывает, обязательно ли использовать ПИН-код для связывания с новыми устройствами.|
|windowsStoreBlocked|Boolean|Указывает, следует ли запретить использовать Microsoft Store.|
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Указывает, можно ли загружать неопубликованные приложения из пакетов AppX с доверенным сертификатом. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|windowsStoreBlockAutoUpdate|Boolean|Указывает, следует ли заблокировать автоматическое обновление приложений из Microsoft Store.|
|developerUnlockSetting|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Указывает, следует ли разрешить разблокировку для разработки. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|sharedUserAppDataAllowed|Boolean|Указывает, следует ли запретить общий доступ к данным для пользователей одного приложения.|
|appsBlockWindowsStoreOriginatedApps|Boolean|Указывает, следует ли отключить запуск всех предустановленных или скачанных приложений из Microsoft Store.|
|windowsStoreEnablePrivateStoreOnly|Boolean|Указывает, следует ли включить только частный магазин.|
|storageRestrictAppDataToSystemVolume|Boolean|Указывает, можно ли хранить данные приложения не на системном диске.|
|storageRestrictAppInstallToSystemVolume|Boolean|Указывает, можно ли устанавливать приложения не на системном диске.|
|gameDvrBlocked|Boolean|Указывает, следует ли блокировать DVR и трансляцию контента.|
|experienceBlockDeviceDiscovery|Boolean|Указывает, следует ли блокировать обнаружение устройств.|
|experienceBlockErrorDialogWhenNoSIM|Boolean|Указывает, следует ли запретить отображение диалогового окна ошибки, если SIM-карта не обнаружена.|
|experienceBlockTaskSwitcher|Boolean|Указывает, следует ли заблокировать переключение задач на устройстве.|
|logonBlockFastUserSwitching|Boolean|Отключает возможность быстрого переключения между учетными записями пользователей, вошедших в систему, без выхода из системы.|
|tenantLockdownRequireNetworkDuringOutOfBoxExperience|Логическое|Указывает, требуется ли устройство для подключения к сети.|
|appManagementMSIAllowUserControlOverInstall|Логическое|Этот параметр политики позволяет пользователям изменять параметры установки, которые обычно доступны только системным администраторам.|
|appManagementMSIAlwaysInstallWithElevatedPrivileges|Логическое|Этот параметр политики позволяет установщику Windows использовать повышенные разрешения при установке любой программы в системе.|
|dataProtectionBlockDirectMemoryAccess|Логическое|Этот параметр политики позволяет блокировать прямой доступ к памяти (DMA) для всех нисходящие порты PCI с горячим подключением, пока пользователь не выполнит вход в Windows.|
|appManagementPackageFamilyNamesToLaunchAfterLogOn|Коллекция String|Список разделенных точкой с запятой имен семейств пакетов для приложений Для Windows. Перечисленные приложения для Windows должны запускаться после входа в систему.|
|uninstallBuiltInApps|Boolean|Указывает, следует ли удалить фиксированный список встроенных приложений Windows.|
|configureTimeZone|String|Указывает часовой пояс, применяемый к устройству. Это стандартное имя Windows для целевого часового пояса.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[Коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства по пользователю. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|privacyAccessControls|[Коллекция windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Указывает список приложений с уровнями управления доступом к категориям данных конфиденциальности и (или) уровням доступа по умолчанию для каждой категории. Эта коллекция может содержать не более 500 элементов.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10GeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
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
  "taskManagerBlockEndTask": true,
  "energySaverOnBatteryThresholdPercentage": 1024,
  "energySaverPluggedInThresholdPercentage": 1024,
  "powerLidCloseActionOnBattery": "String",
  "powerLidCloseActionPluggedIn": "String",
  "powerButtonActionOnBattery": "String",
  "powerButtonActionPluggedIn": "String",
  "powerSleepButtonActionOnBattery": "String",
  "powerSleepButtonActionPluggedIn": "String",
  "powerHybridSleepOnBattery": "String",
  "powerHybridSleepPluggedIn": "String",
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "String (timestamp)",
    "recurrence": "String",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "String",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "String",
  "authenticationPreferredAzureADTenantDomainName": "String",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "String"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "String"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "String",
  "enterpriseCloudPrintOAuthAuthority": "String",
  "enterpriseCloudPrintOAuthClientIdentifier": "String",
  "enterpriseCloudPrintResourceIdentifier": "String",
  "enterpriseCloudPrintDiscoveryMaxLimit": 1024,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "String",
  "experienceDoNotSyncBrowserSettings": "String",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "String"
  ],
  "printerDefaultName": "String",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "findMyFiles": "String",
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "String",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "String",
  "edgeTelemetryForMicrosoft365Analytics": "String",
  "inkWorkspaceAccess": "String",
  "inkWorkspaceAccessState": "String",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "smartScreenAppInstallControl": "String",
  "personalizationDesktopImageUrl": "String",
  "personalizationLockScreenImageUrl": "String",
  "bluetoothAllowedServices": [
    "String"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "String",
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
  "edgeFavoritesListLocation": "String",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "String",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "String",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "String"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "String",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "String",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "String",
  "edgeKioskResetAfterIdleTimeInMinutes": 1024,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "String",
  "defenderRequireRealTimeMonitoring": true,
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderSignatureUpdateIntervalInHours": 1024,
  "defenderMonitorFileActivity": "String",
  "defenderDaysBeforeDeletingQuarantinedMalware": 1024,
  "defenderScanMaxCpu": 1024,
  "defenderScanArchiveFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderRequireCloudProtection": true,
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeout": 1024,
  "defenderCloudExtendedTimeoutInSeconds": 1024,
  "defenderPromptForSampleSubmission": "String",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderScanType": "String",
  "defenderSystemScanSchedule": "String",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderPotentiallyUnwantedAppActionSetting": "String",
  "defenderSubmitSamplesConsentType": "String",
  "defenderBlockOnAccessProtection": true,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "String",
    "moderateSeverity": "String",
    "highSeverity": "String",
    "severeSeverity": "String"
  },
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderProcessesToExclude": [
    "String"
  ],
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 1024,
  "lockScreenActivateAppsWithVoice": "String",
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordMinimumAgeInDays": 1024,
  "privacyAdvertisingId": "String",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "activateAppsWithVoice": "String",
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "String",
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
  "startMenuLayoutEdgeAssetsXml": "binary",
  "startMenuLayoutXml": "binary",
  "startMenuMode": "String",
  "startMenuPinnedFolderDocuments": "String",
  "startMenuPinnedFolderDownloads": "String",
  "startMenuPinnedFolderFileExplorer": "String",
  "startMenuPinnedFolderHomeGroup": "String",
  "startMenuPinnedFolderMusic": "String",
  "startMenuPinnedFolderNetwork": "String",
  "startMenuPinnedFolderPersonalFolder": "String",
  "startMenuPinnedFolderPictures": "String",
  "startMenuPinnedFolderSettings": "String",
  "startMenuPinnedFolderVideos": "String",
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
  "windowsSpotlightConfigureOnLockScreen": "String",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "String",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "String",
    "exceptions": [
      "String"
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
  "safeSearchFilter": "String",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "String",
  "edgeFirstRunUrl": "String",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "String"
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
  "wiFiScanInterval": 1024,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "String",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "String",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "String"
  ],
  "uninstallBuiltInApps": true,
  "configureTimeZone": "String"
}
```




