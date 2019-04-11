---
title: Create windows10GeneralConfiguration
description: Создание объекта windows10GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f392f98c987e4d1ea8cc92b198a46ff53f0e2fd5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792848"
---
# <a name="create-windows10generalconfiguration"></a>Create windows10GeneralConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).

## <a name="prerequisites"></a>Необходимые разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

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
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта windows10GeneralConfiguration в формате JSON.

Ниже показаны свойства, которые необходимо указывать при создании объекта windows10GeneralConfiguration.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Таскманажерблоккендтаск|Boolean|Укажите, могут ли пользователи, не являющиеся администраторами, использовать диспетчер задач для завершения задач.|
|windows10AppsForceUpdateSchedule|[windows10AppsForceUpdateSchedule](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|Расписание принудительного обновления Windows 10 для приложений.|
|Енаблеаутоматикредеплоймент|Boolean|Разрешить пользователям с правами администратора удалять все данные и параметры пользователя с помощью СОЧЕТАНИЯ клавиш CTRL + Win + R на экране блокировки устройства, чтобы можно было автоматически повторно настроить и зарегистрировать устройство в управлении.|
|Микрософтаккаунтсигнинассистантсеттингс|[Сигнинассистантоптионс](../resources/intune-deviceconfig-signinassistantoptions.md)|Управляет службой NT помощника по входу в учетную запись Майкрософт (влидсвк). Возможные значения: `notConfigured`, `disabled`.|
|Аусентикатионалловсекондаридевице|Boolean|Позволяет устройствам вторичной проверки подлинности работать с Windows.|
|Аусентикатионвебсигнин|[Включение](../resources/intune-shared-enablement.md)|Указывает, будет ли включен поставщик учетных данных веб-служб. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Аусентикатионпреферредазуреадтенантдомаиннаме|String|Указывает предпочитаемый домен между доступными доменами в клиенте Azure AD.|
|Криптографялловфипсалгорисмполици|Boolean|Укажите, следует ли включить или отключить политику федеральной обработки информации (FIPS).|
|Дисплайапплиствисгдидпискалингтурнедон|Коллекция String|Список устаревших приложений с включенным масштабированием GDI.|
|Дисплайапплиствисгдидпискалингтурнедофф|Коллекция String|Список устаревших приложений, для которых масштабирование GDI отключено.|
|enterpriseCloudPrintDiscoveryEndPoint|String|Конечная точка для обнаружения облачных принтеров.|
|enterpriseCloudPrintOAuthAuthority|String|Конечная точка аутентификации для получения токенов OAuth.|
|enterpriseCloudPrintOAuthClientIdentifier|String|GUID клиентского приложения, которому разрешено получать токены OAuth из системы OAuth.|
|enterpriseCloudPrintResourceIdentifier|String|URI ресурса OAuth для службы печати, настроенный на портале Azure.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Максимальное количество принтеров, запрашиваемых с конечной точки обнаружения. Этот параметр применяется только к мобильным устройствам. Допустимые значения: от 1 до 65 535.|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String|URI ресурса OAuth для службы обнаружения принтеров, настроенный на портале Azure.|
|Експериенцедонотсинкбровсерсеттингс|[Бровсерсинксеттинг](../resources/intune-deviceconfig-browsersyncsetting.md)|Разрешить или запретить синхронизацию параметров браузера Microsoft Edge. Возможность для ИТ для ИТ, чтобы предотвратить синхронизацию между устройствами, но разрешить переопределение пользователей. Возможные значения: `notConfigured`, `blockedWithUserOverride`, `blocked`.|
|Мессагингблокксинк|Boolean|Указывает, следует ли блокировать резервное копирование и восстановление текстовых сообщений везде.|
|Мессагингблоккммс|Boolean|Указывает, следует ли заблокировать функцию отправки и получения MMS на устройстве.|
|Мессагингблоккричкоммуникатионсервицес|Boolean|Указывает, следует ли заблокировать функцию отправки и получения RCS на устройстве.|
|Свойства printernames|Коллекция String|Автоматическая подготовка принтеров на основе их имен (имена узлов сети).|
|Принтердефаултнаме|String|Имя установленного принтера (имя узла сети).|
|Принтерблоккаддитион|Boolean|Запретить пользователю установку дополнительных принтеров из параметров принтеров.|
|searchBlockDiacritics|Boolean|Указывает, можно ли использовать диакритические знаки в поиске.|
|searchDisableAutoLanguageDetection|Boolean|Указывает, следует ли использовать автоматическое определение языка при индексировании контента и свойств.|
|searchDisableIndexingEncryptedItems|Boolean|Указывает, следует ли запретить индексирование защищенных WIP элементов, чтобы они не отображались в результатах поиска Кортаны или проводника.|
|searchEnableRemoteQueries|Boolean|Указывает, следует ли заблокировать удаленные запросы к индексу этого компьютера.|
|Сеарчдисаблеуселокатион|Boolean|Указывает, может ли поиск использовать сведения о расположении.|
|Сеарчдисаблелокатион|Boolean|Указывает, может ли поиск использовать сведения о расположении.|
|searchDisableIndexerBackoff|Boolean|Указывает, следует ли отключить функцию отхода индексатора поиска.|
|searchDisableIndexingRemovableDrive|Boolean|Указывает, могут ли пользователи добавлять расположения на съемных дисках в библиотеки и для индексирования.|
|searchEnableAutomaticIndexSizeManangement|Boolean|Указывает минимальный объем памяти на жестком диске с индексом до остановки индексирования.|
|Сеарчблокквебресултс|Boolean|Указывает, следует ли запретить Поиск в Интернете.|
|Секуритиблокказуреаджоинеддевицесаутоенкриптион|Boolean|Укажите, следует ли разрешить автоматическое шифрование устройства во время OOBE, когда устройство присоединяется к Azure AD (только для настольных компьютеров).|
|diagnosticsDataSubmissionMode|[Диагностикдатасубмиссионмоде](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|Возвращает или задает значение, позволяющее устройству отправлять данные диагностики и телеметрии использования, такие как Watson. Возможные значения: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Boolean|Возвращает или задает значение, позволяющее ИТ-администраторам запретить работу приложений и функций с файлами в OneDrive.|
|Системтелеметрипроксисервер|String|Получает или задает полное доменное имя или IP-адрес прокси-сервера для переадресации запросов на взаимодействие с пользователем и телеМетрию с подключением.|
|edgeTelemetryForMicrosoft365Analytics|[Еджетелеметримоде](../resources/intune-deviceconfig-edgetelemetrymode.md)|Указывает, какие типы данных телеметрии (нет, интрасеть, Интернет и т. д.) отправляются в Microsoft 365 Analytics. Возможные значения: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.|
|Инкворкспацеакцесс|[Инкакцесссеттинг](../resources/intune-deviceconfig-inkaccesssetting.md)|Управляет доступом пользователей к рабочей области для рукописного ввода с рабочего стола и с экрана блокировки. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|Инкворкспацеакцессстате|[Статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|Управляет доступом пользователей к рабочей области для рукописного ввода с рабочего стола и с экрана блокировки. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|Инкворкспацеблокксугжестедаппс|Boolean|Укажите, следует ли отображать Рекомендуемые предложения приложения в рабочей области для рукописного ввода.|
|smartScreenEnableAppInstallControl|Boolean|Позволяет ИТ-администраторам разрешать или запрещать установку приложений из мест, отличных от Store.|
|personalizationDesktopImageUrl|String|Начинающийся с http или https URL-адрес изображения в формате JPG, JPEG или PNG, которое необходимо скачать и разместить на рабочем столе, или URL-адрес локального изображения в файловой системе, которое нужно разместить на рабочем столе.|
|personalizationLockScreenImageUrl|String|Начинающийся с http или https URL-адрес изображения в формате JPG, JPEG или PNG, которое необходимо скачать и разместить на экране блокировки, или URL-адрес локального изображения в файловой системе, которое нужно разместить на экране блокировки.|
|bluetoothAllowedServices|Коллекция String|Укажите список разрешенных служб и профилей Bluetooth в шестнадцатеричном формате.|
|bluetoothBlockAdvertising|Boolean|Указывает, следует ли запретить использовать рекламу по Bluetooth.|
|Блуетусблоккпромптедпроксималконнектионс|Boolean|Указывает, следует ли запретить пользователям использовать сочетание SWIFT и другие сценарии для близлежащих устройств.|
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
|Еджефаворитеслистлокатион|String|Расположение списка избранного для подготовки. Это может быть локальный файл, локальная сеть или HTTP-адрес.|
|Еджеблоккедитфаворитес|Boolean|Указывает, следует ли запретить пользователю вносить изменения в папку "Избранное".|
|Едженевтабпажеурл|String|Указание страницы, открытой при создании новых вкладок.|
|Еджехомебуттонконфигуратион|[Еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|Вызывает скрытие кнопки "домой", Загрузка начальной страницы по умолчанию, загрузка новой страницы вкладки или настраиваемый URL-адрес.|
|Еджехомебуттонконфигуратионенаблед|Boolean|Включите конфигурацию кнопки "домой".|
|Еджеопенсвис|[Еджеопеноптионс](../resources/intune-deviceconfig-edgeopenoptions.md)|Укажите, какие типы страниц открыты при запуске. Возможные значения: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.|
|Еджеблокксиделоадинжекстенсионс|Boolean|Указывает, может ли пользователь Загрузка неопубликованных расширения.|
|Еджерекуиредекстенсионпаккажефамилинамес|Коллекция String|Укажите список имен семейств пакетов, которые необходимы для расширения браузера и не могут быть отключены пользователем.|
|Еджеблоккпринтинг|Boolean|Настройка поГраничного сервера на разрешение или блокировку печати.|
|Еджефаворитесбарвисибилити|[Висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Возвращает или задает значение, указывающее, следует ли всегда отображать или скрывать панель избранного на любой странице. Возможные значения: `notConfigured`, `hide`, `show`.|
|Еджеблокксавингхистори|Boolean|Настройте поГраничный сервер, чтобы разрешить сохранение журнала браузера или никогда не сохранять журнал браузера.|
|Еджеблоккфуллскринмоде|Boolean|РазРешите или запретите переход с поГраничным экраном на полноэкранный режим.|
|Еджеблокквебконтентонневтабпаже|Boolean|Настройте, чтобы загрузить пустую страницу на краю, а не на странице новой вкладки по умолчанию и запретить пользователям изменять ее.|
|Еджеблокктабпрелоадинг|Boolean|Определяет, будет ли поГраничный загружается страница новой вкладки при запуске Windows.|
|Еджеблоккпрелаунч|Boolean|Решите, будет ли Microsoft Edge предварительно запущен при запуске Windows.|
|Еджешовмессажевхенопенингинтернетексплорерситес|[Интернетексплорермессажесеттинг](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|Управляет сообщением, отображаемым на границе, перед переключением в Internet Explorer. Возможные значения: `notConfigured`, `disabled`, `enabled`, `keepGoing`.|
|Еджепревентцертификатирророверриде|Boolean|Разрешить или запретить пользователям переопределять ошибки сертификатов.|
|Еджекиоскмодерестриктион|[edgeKioskModeRestrictionType](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|Управляет ограничениями параметров Microsoft EDGE в зависимости от режима настройки киоска. Возможные значения: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.|
|Еджекиоскресетафтеридлетимеинминутес|Int32|Задает время (в минутах) от последнего действия пользователя до сброса Microsoft Edge киоска.  Допустимые значения: 0-1440. Значение по умолчанию равно 5. 0 указывает на отсутствие сброса. Допустимые значения — от 0 до 1440|
|cellularBlockDataWhenRoaming|Boolean|Указывает, следует ли запретить использовать мобильные данные в роуминге.|
|cellularBlockVpn|Boolean|Указывает, следует ли запретить использовать VPN по сотовой сети.|
|cellularBlockVpnWhenRoaming|Boolean|Указывает, следует ли запретить использовать VPN по сотовой сети в роуминге.|
|Целлулардата|[Конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, следует ли разрешить канал сотовой связи на устройстве. Если этот параметр не задан, канал передачи данных разрешен и пользователь может его отключить. Возможные значения: `blocked`, `required`, `allowed`.|
|defenderBlockEndUserAccess|Boolean|Указывает, следует ли заблокировать доступ пользователей к Защитнику.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Время до удаления вредоносного ПО на карантине (в днях). Допустимые значения: от 0 до 90.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Возвращает или задает действия Защитника в отношении обнаруженного вредоносного ПО для каждого уровня угрозы.|
|defenderSystemScanSchedule|[Виклисчедуле](../resources/intune-deviceconfig-weeklyschedule.md)|День проверки системы Защитником. Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|defenderFilesAndFoldersToExclude|Коллекция String|Файлы и папки, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderFileExtensionsToExclude|Коллекция String|Расширения файлов, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderScanMaxCpu|Int32|Максимальный процент загрузки ЦП во время проверки. Допустимые значения: от 0 до 100|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|Значение для отслеживания действий с файлами. Возможные значения: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|Дефендерпотентиаллюнвантедаппактион|[Дефендерпотентиаллюнвантедаппактион](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|Получает или задает действие защитника, которое будет выполняться в потенциально неЖелательном приложении (ПУА), которое включает программное обеспечение с поведением AD-Injection, объединением программного обеспечения, постоянным запросом на оплату или подписку и т. д. Пользователь оповещений защитника при загрузке Пуа или попытке его установки. Добавлено в Windows 10 для настольных ПК. Возможные значения: `deviceDefault`, `block`, `audit`.|
|Дефендерпотентиаллюнвантедаппактионсеттинг|[Дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Получает или задает действие защитника, которое будет выполняться в потенциально неЖелательном приложении (ПУА), которое включает программное обеспечение с поведением AD-Injection, объединением программного обеспечения, постоянным запросом на оплату или подписку и т. д. Пользователь оповещений защитника при загрузке Пуа или попытке его установки. Добавлено в Windows 10 для настольных ПК. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|defenderProcessesToExclude|Коллекция String|Процессы, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|Позволяет указать, нужно ли спрашивать пользователя перед отправкой образцов. Возможные значения: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderRequireBehaviorMonitoring|Boolean|Указывает, обязательно ли использовать наблюдение за поведением.|
|defenderRequireCloudProtection|Boolean|Указывает, обязательно ли использовать облачную защиту.|
|defenderRequireNetworkInspectionSystem|Boolean|Указывает, обязательно ли использовать систему проверки сети.|
|defenderRequireRealTimeMonitoring|Boolean|Указывает, обязательно ли использовать мониторинг в режиме реального времени.|
|defenderScanArchiveFiles|Boolean|Указывает, следует ли проверять архивные файлы.|
|defenderScanDownloads|Boolean|Указывает, следует ли проверять загрузки.|
|Дефендерсчедулесканенаблеловкпуприорити|Boolean|Если этот параметр включен, во время запланированных проверок будет использоваться недостаточный приоритет ЦП.|
|Дефендердисаблекатчупкуиккскан|Boolean|При блокировании будет отключено дополнительное сканирование для запланированных быстрых проверок.|
|Дефендердисаблекатчупфуллскан|Boolean|При блокировании будет отключено дополнительное сканирование для запланированных полных проверок.|
|defenderScanNetworkFiles|Boolean|Указывает, следует ли сканировать файлы, открытые из сетевой папки.|
|defenderScanIncomingMail|Boolean|Указывает, следует ли проверять входящую почту.|
|defenderScanMappedNetworkDrivesDuringFullScan|Boolean|Указывает, следует ли сканировать подключенные сетевые диски во время полной проверки.|
|defenderScanRemovableDrivesDuringFullScan|Boolean|Указывает, следует ли сканировать съемные диски во время полной проверки.|
|defenderScanScriptsLoadedInInternetExplorer|Boolean|Указывает, следует ли проверять сценарии, загружаемые в браузере Internet Explorer.|
|defenderSignatureUpdateIntervalInHours|Int32|Интервал обновления сигнатур (в часах). Укажите 0, чтобы не проверять. Допустимые значения: от 0 до 24.|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|Тип проверки системы Защитником. Возможные значения: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledScanTime|TimeOfDay|Время проверки системы Защитником.|
|defenderScheduledQuickScanTime|TimeOfDay|Время ежедневной быстрой проверки.|
|defenderCloudBlockLevel|[Дефендерклаудблокклевелтипе](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Определяет уровень облачной защиты. Возможные значения: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|Дефендерклаудекстендедтимеаут|Int32|Расширение времени ожидания для сканирования файлов в облаке. Допустимые значения: от 0 до 50.|
|Дефендерклаудекстендедтимеаутинсекондс|Int32|Расширение времени ожидания для сканирования файлов в облаке. Допустимые значения: от 0 до 50.|
|Дефендерблокконакцесспротектион|Boolean|Разрешает или запрещает защитник Windows для функций защиты доступа.|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|Проверка уровня согласия пользователя в Защитнике Windows для отправки данных. Возможные значения: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|lockScreenAllowTimeoutConfiguration|Boolean|Указывает, следует ли отображать настройку, позволяющую определить время до отключения экрана на экране блокировки мобильных устройств с Windows 10. Если для этой политики установлено значение Allow, значение, заданное свойством lockScreenTimeoutInSeconds, игнорируется.|
|lockScreenBlockActionCenterNotifications|Boolean|Указывает, следует ли запретить показ уведомлений из центра уведомлений на экране блокировки.|
|lockScreenBlockCortana|Boolean|Указывает, может ли пользователь взаимодействовать с Кортаной с помощью голоса при заблокированной системе.|
|lockScreenBlockToastNotifications|Boolean|Указывает, следует ли показывать всплывающие уведомления на экране блокировки устройства.|
|lockScreenTimeoutInSeconds|Int32|Установите время (в секундах) от блокировки экрана до его выключения для мобильных устройств с Windows 10. Поддерживаемые значения: от 11 до 1800. Допустимые значения: от 11 до 1800.|
|passwordBlockSimple|Boolean|Укажите, разрешены ли такие ПИН-коды или пароли, как "1111" или "1234". Это свойство также контролирует использование графических паролей на компьютерах с Windows 10.|
|passwordExpirationDays|Int32|Срок действия пароля (в днях). Допустимые значения: от 0 до 730.|
|passwordMinimumLength|Int32|Минимальная длина пароля. Допустимые значения: от 4 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые требуются для пароля.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, повторное использование которых необходимо запретить. Допустимые значения: от 0 до 50.|
|passwordRequired|Boolean|Указывает, обязательно ли использовать пароль.|
|passwordRequireWhenResumeFromIdleState|Boolean|Указывает, следует ли запрашивать пароль при выходе из состояния простоя.|
|passwordRequiredType|[Рекуиредпассвордтипе](../resources/intune-deviceconfig-requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек. Допустимые значения: от 0 до 999.|
|Пассвордминимумажеиндайс|Int32|Этот параметр безопасности определяет период времени (в днях), в течение которого необходимо использовать пароль, прежде чем пользователь сможет его изменить. Допустимые значения — от 0 до 998|
|privacyAdvertisingId|[Статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|Указывает, можно ли использовать идентификатор рекламы. Добавлено в Windows 10 версии 1607. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Boolean|Указывает, следует ли запретить автоматическое принятие примечаний о связывании и конфиденциальности при запуске приложений.|
|Привацидисаблелаунчекспериенце|Boolean|Эта политика запрещает запуск службы конфиденциальности при входе пользователя для новых и обновленных пользователей.|
|privacyBlockInputPersonalization|Boolean|Указывает, следует ли запретить использовать облачные службы распознавания речи для приложений "Кортана", "Диктофон" или Store.|
|Привациблоккпублишусерактивитиес|Boolean|Блокирует общий доступ/обнаружение недавно использовавшихся ресурсов в переключателе задач и т. д.|
|Привациблоккактивитифид|Boolean|Блокирует использование облачных голосовых служб для Кортаны, диктовки или хранения приложений.|
|startBlockUnpinningAppsFromTaskbar|Boolean|Указывает, следует ли запретить пользователю откреплять приложения с панели задач.|
|startMenuAppListVisibility|[Виндовсстартменуапплиствисибилититипе](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|Эта политика позволяет свернуть список приложений, полностью удалить этот список или отключить соответствующий переключатель в приложении "Параметры". Возможные значения: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
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
|startMenuMode|[Виндовсстартменумодетипе](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|Позволяет администраторам определить вид меню "Пуск". Возможные значения: `userDefined`, `fullScreen`, `nonFullScreen`.|
|startMenuPinnedFolderDocuments|[Висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Документы" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderDownloads|[Висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Загрузки" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderFileExplorer|[Висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык проводника в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderHomeGroup|[Висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Домашняя группа" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderMusic|[Висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Музыка" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderNetwork|[Висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Сеть" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPersonalFolder|[Висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык личной папки в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPictures|[Висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Изображения" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderSettings|[Висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Параметры" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderVideos|[Висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Видео" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
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
|windowsSpotlightConfigureOnLockScreen|[Виндовсспотлигхтенаблементсеттингс](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|Указывает тип прожектора. Возможные значения: `notConfigured`, `disabled`, `enabled`.|
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
|safeSearchFilter|[Сафесеарчфилтертипе](../resources/intune-deviceconfig-safesearchfiltertype.md)|Определяет необходимый уровень фильтрации для безопасного поиска. Возможные значения: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Boolean|Указывает, следует ли блокировать всплывающие окна.|
|edgeBlockSearchSuggestions|Boolean|Указывает, следует ли запретить пользователю использовать варианты поиска в адресной строке.|
|Еджеблокксеарченгинекустомизатион|Boolean|Указывает, следует ли запретить пользователю добавлять новую поисковую систему или изменять поисковую систему по умолчанию.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Boolean|Указывает, следует ли переключить трафик интрасети от края к Internet Explorer. Note: имя этого свойства является недостоверным; свойство устарело, вместо него используйте Еджесендинтранеттраффиктоинтернетексплорер.|
|Еджесендинтранеттраффиктоинтернетексплорер|Boolean|Указывает, следует ли переключить трафик интрасети от края к Internet Explorer.|
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
|appsAllowTrustedAppsSideloading|[Статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|Указывает, можно ли загружать неопубликованные приложения из пакетов AppX с доверенным сертификатом. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|windowsStoreBlockAutoUpdate|Boolean|Указывает, следует ли заблокировать автоматическое обновление приложений из Microsoft Store.|
|developerUnlockSetting|[Статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|Указывает, следует ли разрешить разблокировку для разработки. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
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
|tenantLockdownRequireNetworkDuringOutOfBoxExperience|Boolean|Указывает, требуется ли устройство для подключения к сети.|
|Аппманажементмсиалловусерконтроловеринсталл|Boolean|Этот параметр политики позволяет пользователям изменять параметры установки, которые обычно доступны только системным администраторам.|
|Аппманажементмсиалвайсинсталлвиселеватедпривилежес|Boolean|Этот параметр политики направляет установщик Windows использовать повышенные разрешения при установке любой программы в систему.|
|Датапротектионблоккдиректмеморякцесс|Boolean|Этот параметр политики позволяет заблокировать прямой доступ к памяти (DMA) для всех подключенных портов PCI, подключенных к горячему подключению, пока пользователь не войдет в систему Windows.|
|Аппманажементпаккажефамилинаместолаунчафтерлогон|Коллекция String|Список имен семейств пакетов для приложений Windows, разделенных точкой с запятой. Перечисленные приложения Windows будут запущены после входа в систему.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 13518

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "taskManagerBlockEndTask": true,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
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
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
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
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
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
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
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
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
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
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
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
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
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
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
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
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 13690

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "taskManagerBlockEndTask": true,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
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
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
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
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
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
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
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
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
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
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
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
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
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
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
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
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ]
}
```





