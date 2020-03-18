---
title: Тип ресурса windows10GeneralConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windows10GeneralConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f68a4fdf2ecfbcc3e2728e652f1da8fee4916c9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786707"
---
# <a name="windows10generalconfiguration-resource-type"></a>Тип ресурса windows10GeneralConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windows10GeneralConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов Windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-list.md)|Коллекция [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Перечисление свойств и связей объектов [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Получение объекта windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-get.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md);|Чтение свойств и связей объекта [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Создание объекта windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-create.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md);|Создание объекта [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Удаление объекта windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-delete.md)|Нет|Удаление объекта [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Обновление объекта windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-update.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Обновление свойств объекта [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|таскманажерблоккендтаск|Логический|Укажите, могут ли пользователи, не являющиеся администраторами, использовать диспетчер задач для завершения задач.|
|енергисаверонбаттерисрешолдперцентаже|Int32|Этот параметр позволяет указать уровень заряда батареи при включенной экономии энергии. При питании от батареи автоматически включается экономия энергии (и ниже) указанного уровня заряда батареи. Допустимый диапазон входных данных (0-100). Допустимые значения: от 0 до 100|
|енергисаверплугжединсрешолдперцентаже|Int32|Этот параметр позволяет указать уровень заряда батареи при включенной экономии энергии. При подключении к сети экономия энергии автоматически включается (и ниже) указанного уровня заряда батареи. Допустимый диапазон входных данных (0-100). Допустимые значения: от 0 до 100|
|поверлидклосеактиононбаттери|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр определяет действие, предпринимаемое Windows, когда пользователь закрывает крышку на мобильном ПК при питании от батареи. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|поверлидклосеактионплугжедин|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр определяет действие, предпринимаемое Windows, когда пользователь закрывает крышку мобильного ПК во время подключения к сети. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|повербуттонактиононбаттери|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр определяет действие, выполняемое Windows, когда пользователь нажимает кнопку питания при питании от аккумулятора. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|повербуттонактионплугжедин|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр определяет действие, выполняемое Windows, когда пользователь нажимает кнопку питания, когда он подключен к сети. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|поверслипбуттонактиононбаттери|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр определяет действие, которое Windows выполняет, когда пользователь нажимает кнопку спящего режима при питании от батареи. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|поверслипбуттонактионплугжедин|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Этот параметр определяет действие, которое Windows выполняет, когда пользователь нажимает кнопку "сон" при подключении к сети. Возможные значения: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|поверхибридслипонбаттери|[Включение](../resources/intune-shared-enablement.md)|Этот параметр позволяет отключить гибридный спящий режим при питании от батарей. Если для этого параметра задано значение Disabled, при переходе системы в спящий режим хиберфиле не создается. Если включить или не настраивать этот параметр политики, пользователи смогут управлять этим параметром. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|поверхибридслипплугжедин|[Включение](../resources/intune-shared-enablement.md)|Этот параметр позволяет отключить гибридный спящий режим при подключении к сети. Если для этого параметра задано значение Disabled, при переходе системы в спящий режим хиберфиле не создается. Если включить или не настраивать этот параметр политики, пользователи смогут управлять этим параметром. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|windows10AppsForceUpdateSchedule|[windows10AppsForceUpdateSchedule](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|Расписание принудительного обновления Windows 10 для приложений.|
|енаблеаутоматикредеплоймент|Логический|Разрешить пользователям с правами администратора удалять все данные и параметры пользователя с помощью сочетания клавиш CTRL + Win + R на экране блокировки устройства, чтобы можно было автоматически повторно настроить и зарегистрировать устройство в управлении.|
|микрософтаккаунтсигнинассистантсеттингс|[сигнинассистантоптионс](../resources/intune-deviceconfig-signinassistantoptions.md)|Управляет службой NT помощника по входу в учетную запись Майкрософт (влидсвк). Возможные значения: `notConfigured`, `disabled`.|
|аусентикатионалловсекондаридевице|Логический|Позволяет устройствам вторичной проверки подлинности работать с Windows.|
|аусентикатионвебсигнин|[Включение](../resources/intune-shared-enablement.md)|Указывает, будет ли включен поставщик учетных данных веб-служб. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|аусентикатионпреферредазуреадтенантдомаиннаме|String|Указывает предпочитаемый домен между доступными доменами в клиенте Azure AD.|
|криптографялловфипсалгорисмполици|Логический|Укажите, следует ли включить или отключить политику федеральной обработки информации (FIPS).|
|дисплайапплиствисгдидпискалингтурнедон|Коллекция String|Список устаревших приложений с включенным масштабированием GDI.|
|дисплайапплиствисгдидпискалингтурнедофф|Коллекция String|Список устаревших приложений, для которых масштабирование GDI отключено.|
|enterpriseCloudPrintDiscoveryEndPoint|String|Конечная точка для обнаружения облачных принтеров.|
|enterpriseCloudPrintOAuthAuthority|String|Конечная точка аутентификации для получения токенов OAuth.|
|enterpriseCloudPrintOAuthClientIdentifier|String|GUID клиентского приложения, которому разрешено получать токены OAuth из системы OAuth.|
|enterpriseCloudPrintResourceIdentifier|String|URI ресурса OAuth для службы печати, настроенный на портале Azure.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Максимальное количество принтеров, запрашиваемых с конечной точки обнаружения. Этот параметр применяется только к мобильным устройствам. Допустимые значения: от 1 до 65 535.|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String|URI ресурса OAuth для службы обнаружения принтеров, настроенный на портале Azure.|
|експериенцедонотсинкбровсерсеттингс|[бровсерсинксеттинг](../resources/intune-deviceconfig-browsersyncsetting.md)|Разрешить или запретить синхронизацию параметров браузера Microsoft Edge. Возможность для ИТ для ИТ, чтобы предотвратить синхронизацию между устройствами, но разрешить переопределение пользователей. Возможные значения: `notConfigured`, `blockedWithUserOverride`, `blocked`.|
|мессагингблокксинк|Логический|Указывает, следует ли блокировать резервное копирование и восстановление текстовых сообщений везде.|
|мессагингблоккммс|Логический|Указывает, следует ли заблокировать функцию отправки и получения MMS на устройстве.|
|мессагингблоккричкоммуникатионсервицес|Логический|Указывает, следует ли заблокировать функцию отправки и получения RCS на устройстве.|
|Свойства printernames|Коллекция String|Автоматическая подготовка принтеров на основе их имен (имена узлов сети).|
|принтердефаултнаме|String|Имя установленного принтера (имя узла сети).|
|принтерблоккаддитион|Логический|Запретить пользователю установку дополнительных принтеров из параметров принтеров.|
|searchBlockDiacritics|Логический|Указывает, можно ли использовать диакритические знаки в поиске.|
|searchDisableAutoLanguageDetection|Логический|Указывает, следует ли использовать автоматическое определение языка при индексировании контента и свойств.|
|searchDisableIndexingEncryptedItems|Логический|Указывает, следует ли запретить индексирование защищенных WIP элементов, чтобы они не отображались в результатах поиска Кортаны или проводника.|
|searchEnableRemoteQueries|Boolean|Указывает, следует ли заблокировать удаленные запросы к индексу этого компьютера.|
|сеарчдисаблеуселокатион|Логический|Указывает, может ли поиск использовать сведения о расположении.|
|сеарчдисаблелокатион|Логический|Указывает, может ли поиск использовать сведения о расположении.|
|searchDisableIndexerBackoff|Логический|Указывает, следует ли отключить функцию отхода индексатора поиска.|
|searchDisableIndexingRemovableDrive|Логический|Указывает, могут ли пользователи добавлять расположения на съемных дисках в библиотеки и для индексирования.|
|searchEnableAutomaticIndexSizeManangement|Логический|Указывает минимальный объем памяти на жестком диске с индексом до остановки индексирования.|
|сеарчблокквебресултс|Логический|Указывает, следует ли запретить Поиск в Интернете.|
|финдмифилес|[Включение](../resources/intune-shared-enablement.md)|Определяет, может ли пользователь настроить поиск в режиме "Мои файлы", который выполняет поиск файлов на дополнительных жестких дисках, а также вне профиля пользователя. "Найти мои файлы" не позволяет пользователям искать файлы и расположения, к которым у них нет доступа. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|секуритиблокказуреаджоинеддевицесаутоенкриптион|Логический|Укажите, следует ли разрешить автоматическое шифрование устройства во время OOBE, когда устройство присоединяется к Azure AD (только для настольных компьютеров).|
|diagnosticsDataSubmissionMode|[диагностикдатасубмиссионмоде](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|Возвращает или задает значение, позволяющее устройству отправлять данные диагностики и телеметрии использования, такие как Watson. Возможные значения: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Логический|Возвращает или задает значение, позволяющее ИТ-администраторам запретить работу приложений и функций с файлами в OneDrive.|
|системтелеметрипроксисервер|String|Получает или задает полное доменное имя или IP-адрес прокси-сервера для переадресации запросов на взаимодействие с пользователем и телеметрию с подключением.|
|edgeTelemetryForMicrosoft365Analytics|[еджетелеметримоде](../resources/intune-deviceconfig-edgetelemetrymode.md)|Указывает, какие типы данных телеметрии (нет, интрасеть, Интернет и т. д.) отправляются в Microsoft 365 Analytics. Возможные значения: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.|
|инкворкспацеакцесс|[инкакцесссеттинг](../resources/intune-deviceconfig-inkaccesssetting.md)|Управляет доступом пользователей к рабочей области для рукописного ввода с рабочего стола и с экрана блокировки. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|инкворкспацеакцессстате|[статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|Управляет доступом пользователей к рабочей области для рукописного ввода с рабочего стола и с экрана блокировки. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|инкворкспацеблокксугжестедаппс|Логический|Укажите, следует ли отображать Рекомендуемые предложения приложения в рабочей области для рукописного ввода.|
|smartScreenEnableAppInstallControl|Логический|Это свойство будет признано устаревшим в июле 2019 и будет заменено свойством Смартскринаппинсталлконтрол. Позволяет ИТ-администраторам разрешать или запрещать установку приложений из мест, отличных от Store.|
|смартскринаппинсталлконтрол|[appInstallControlType](../resources/intune-deviceconfig-appinstallcontroltype.md)|Добавлено в Windows 10 версии 1703. Позволяет ИТ-администраторам разрешать или запрещать установку приложений из мест, отличных от Store. Возможные значения: `notConfigured`, `anywhere`, `storeOnly`, `recommendations`, `preferStore`.|
|personalizationDesktopImageUrl|String|Начинающийся с http или https URL-адрес изображения в формате JPG, JPEG или PNG, которое необходимо скачать и разместить на рабочем столе, или URL-адрес локального изображения в файловой системе, которое нужно разместить на рабочем столе.|
|personalizationLockScreenImageUrl|String|Начинающийся с http или https URL-адрес изображения в формате JPG, JPEG или PNG, которое необходимо скачать и разместить на экране блокировки, или URL-адрес локального изображения в файловой системе, которое нужно разместить на экране блокировки.|
|bluetoothAllowedServices|Коллекция String|Укажите список разрешенных служб и профилей Bluetooth в шестнадцатеричном формате.|
|bluetoothBlockAdvertising|Логический|Указывает, следует ли запретить использовать рекламу по Bluetooth.|
|блуетусблоккпромптедпроксималконнектионс|Логический|Указывает, следует ли запретить пользователям использовать сочетание SWIFT и другие сценарии для близлежащих устройств.|
|bluetoothBlockDiscoverableMode|Логический|Указывает, следует ли запретить использовать режим обнаружения по Bluetooth.|
|bluetoothBlockPrePairing|Логический|Указывает, следует ли заблокировать автоматическое связывание отдельных пакетных периферийных устройств Bluetooth с главным устройством.|
|edgeBlockAutofill|Логический|Указывает, следует ли заблокировать автозаполнение.|
|edgeBlocked|Логический|Указывает, следует ли запретить использовать браузер Edge.|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune-deviceconfig-edgecookiepolicy.md)|Указывает, какие файлы cookie следует блокировать в браузере Edge. Возможные значения: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeBlockDeveloperTools|Логический|Указывает, следует ли заблокировать средства разработчика в браузере Edge.|
|edgeBlockSendingDoNotTrackHeader|Логический|Указывает, следует ли запретить пользователю отправлять заголовок DNT.|
|edgeBlockExtensions|Логический|Указывает, следует ли заблокировать расширения в браузере Edge.|
|edgeBlockInPrivateBrowsing|Boolean|Указывает, следует ли заблокировать просмотр InPrivate в корпоративных сетях в браузере Edge.|
|edgeBlockJavaScript|Логический|Указывает, следует ли запретить использовать JavaScript.|
|edgeBlockPasswordManager|Логический|Указывает, следует ли заблокировать диспетчер паролей.|
|edgeBlockAddressBarDropdown|Логический|Позволяет заблокировать раскрывающийся список адресной строки в Microsoft Edge. Отключите этот параметр, чтобы уменьшить количество сетевых подключений Microsoft Edge к службам Майкрософт.|
|edgeBlockCompatibilityList|Логический|Позволяет заблокировать список совместимости Майкрософт в Microsoft Edge. Этот список помогает Edge правильно отображать сайты с известными проблемами совместимости.|
|edgeClearBrowsingDataOnExit|Логический|Указывает, следует ли удалять данные просмотра при выходе из Microsoft Edge.|
|edgeAllowStartPagesModification|Логический|Указывает, могут ли пользователи изменять начальные страницы в Edge. Используйте свойство EdgeHomepageUrls, чтобы указать начальные страницы по умолчанию, отображаемые при открытии Edge.|
|edgeDisableFirstRunPage|Логический|Позволяет заблокировать веб-страницу Майкрософт, которая открывается при первом запуске Microsoft Edge. Эта политика позволяет предприятиям, зарегистрированным в конфигурациях с нулевым выбросом, блокировать эту страницу.|
|edgeBlockLiveTileDataCollection|Логический|Позволяет запретить Майкрософт собирать информацию о создании живых плиток, когда пользователи закрепляют сайты из Microsoft Edge на начальном экране.|
|edgeSyncFavoritesWithInternetExplorer|Логический|Указывает, следует ли включить синхронизацию избранного между Internet Explorer и Microsoft Edge. Браузеры обмениваются данными о добавлении, удалении и изменении избранных элементов, а также их порядка.|
|еджефаворитеслистлокатион|String|Расположение списка избранного для подготовки. Это может быть локальный файл, локальная сеть или HTTP-адрес.|
|еджеблоккедитфаворитес|Логический|Указывает, следует ли запретить пользователю вносить изменения в папку "Избранное".|
|едженевтабпажеурл|String|Указание страницы, открытой при создании новых вкладок.|
|еджехомебуттонконфигуратион|[еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|Вызывает скрытие кнопки "домой", Загрузка начальной страницы по умолчанию, загрузка новой страницы вкладки или настраиваемый URL-адрес.|
|еджехомебуттонконфигуратионенаблед|Логический|Включите конфигурацию кнопки "домой".|
|еджеопенсвис|[еджеопеноптионс](../resources/intune-deviceconfig-edgeopenoptions.md)|Укажите, какие типы страниц открыты при запуске. Возможные значения: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.|
|еджеблокксиделоадинжекстенсионс|Логический|Указывает, может ли пользователь Загрузка неопубликованных расширения.|
|еджерекуиредекстенсионпаккажефамилинамес|Коллекция String|Укажите список имен семейств пакетов, которые необходимы для расширения браузера и не могут быть отключены пользователем.|
|еджеблоккпринтинг|Логический|Настройка пограничного сервера на разрешение или блокировку печати.|
|еджефаворитесбарвисибилити|[висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Возвращает или задает значение, указывающее, следует ли всегда отображать или скрывать панель избранного на любой странице. Возможные значения: `notConfigured`, `hide`, `show`.|
|еджеблокксавингхистори|Логический|Настройте пограничный сервер, чтобы разрешить сохранение журнала браузера или никогда не сохранять журнал браузера.|
|еджеблоккфуллскринмоде|Логический|Разрешите или запретите переход с пограничным экраном на полноэкранный режим.|
|еджеблокквебконтентонневтабпаже|Логический|Настройте, чтобы загрузить пустую страницу на краю, а не на странице новой вкладки по умолчанию и запретить пользователям изменять ее.|
|еджеблокктабпрелоадинг|Логический|Определяет, будет ли пограничный загружается страница новой вкладки при запуске Windows.|
|еджеблоккпрелаунч|Логический|Решите, будет ли Microsoft Edge предварительно запущен при запуске Windows.|
|еджешовмессажевхенопенингинтернетексплорерситес|[интернетексплорермессажесеттинг](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|Управляет сообщением, отображаемым на границе, перед переключением в Internet Explorer. Возможные значения: `notConfigured`, `disabled`, `enabled`, `keepGoing`.|
|еджепревентцертификатирророверриде|Логический|Разрешить или запретить пользователям переопределять ошибки сертификатов.|
|еджекиоскмодерестриктион|[edgeKioskModeRestrictionType](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|Управляет ограничениями параметров Microsoft EDGE в зависимости от режима настройки киоска. Возможные значения: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.|
|еджекиоскресетафтеридлетимеинминутес|Int32|Задает время (в минутах) от последнего действия пользователя до сброса Microsoft Edge киоска.  Допустимые значения: 0-1440. Значение по умолчанию равно 5. 0 указывает на отсутствие сброса. Допустимые значения — от 0 до 1440|
|cellularBlockDataWhenRoaming|Boolean|Указывает, следует ли запретить использовать мобильные данные в роуминге.|
|cellularBlockVpn|Логический|Указывает, следует ли запретить использовать VPN по сотовой сети.|
|cellularBlockVpnWhenRoaming|Логический|Указывает, следует ли запретить использовать VPN по сотовой сети в роуминге.|
|целлулардата|[конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, следует ли разрешить канал сотовой связи на устройстве. Если этот параметр не задан, канал передачи данных разрешен и пользователь может его отключить. Возможные значения: `blocked`, `required`, `allowed`.|
|defenderBlockEndUserAccess|Логический|Указывает, следует ли заблокировать доступ пользователей к Защитнику.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Время до удаления вредоносного ПО на карантине (в днях). Допустимые значения: от 0 до 90.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Возвращает или задает действия Защитника в отношении обнаруженного вредоносного ПО для каждого уровня угрозы.|
|defenderSystemScanSchedule|[виклисчедуле](../resources/intune-deviceconfig-weeklyschedule.md)|День проверки системы Защитником. Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.|
|defenderFilesAndFoldersToExclude|Коллекция String|Файлы и папки, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderFileExtensionsToExclude|Коллекция String|Расширения файлов, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderScanMaxCpu|Int32|Максимальный процент загрузки ЦП во время проверки. Допустимые значения: от 0 до 100|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|Значение для отслеживания действий с файлами. Возможные значения: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|дефендерпотентиаллюнвантедаппактион|[дефендерпотентиаллюнвантедаппактион](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|Получает или задает действие защитника, которое будет выполняться в потенциально нежелательном приложении (ПУА), которое включает программное обеспечение с поведением AD-Injection, объединением программного обеспечения, постоянным запросом на оплату или подписку и т. д. Пользователь оповещений защитника при загрузке Пуа или попытке его установки. Добавлено в Windows 10 для настольных ПК. Возможные значения: `deviceDefault`, `block`, `audit`.|
|дефендерпотентиаллюнвантедаппактионсеттинг|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Получает или задает действие защитника, которое будет выполняться в потенциально нежелательном приложении (ПУА), которое включает программное обеспечение с поведением AD-Injection, объединением программного обеспечения, постоянным запросом на оплату или подписку и т. д. Пользователь оповещений защитника при загрузке Пуа или попытке его установки. Добавлено в Windows 10 для настольных ПК. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|defenderProcessesToExclude|Коллекция String|Процессы, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|Позволяет указать, нужно ли спрашивать пользователя перед отправкой образцов. Возможные значения: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderRequireBehaviorMonitoring|Логический|Указывает, обязательно ли использовать наблюдение за поведением.|
|defenderRequireCloudProtection|Логический|Указывает, обязательно ли использовать облачную защиту.|
|defenderRequireNetworkInspectionSystem|Логический|Указывает, обязательно ли использовать систему проверки сети.|
|defenderRequireRealTimeMonitoring|Логический|Указывает, обязательно ли использовать мониторинг в режиме реального времени.|
|defenderScanArchiveFiles|Логический|Указывает, следует ли проверять архивные файлы.|
|defenderScanDownloads|Логический|Указывает, следует ли проверять загрузки.|
|дефендерсчедулесканенаблеловкпуприорити|Логический|Если этот параметр включен, во время запланированных проверок будет использоваться недостаточный приоритет ЦП.|
|дефендердисаблекатчупкуиккскан|Логический|При блокировании будет отключено дополнительное сканирование для запланированных быстрых проверок.|
|дефендердисаблекатчупфуллскан|Логический|При блокировании будет отключено дополнительное сканирование для запланированных полных проверок.|
|defenderScanNetworkFiles|Логический|Указывает, следует ли сканировать файлы, открытые из сетевой папки.|
|defenderScanIncomingMail|Логический|Указывает, следует ли проверять входящую почту.|
|defenderScanMappedNetworkDrivesDuringFullScan|Логический|Указывает, следует ли сканировать подключенные сетевые диски во время полной проверки.|
|defenderScanRemovableDrivesDuringFullScan|Логический|Указывает, следует ли сканировать съемные диски во время полной проверки.|
|defenderScanScriptsLoadedInInternetExplorer|Boolean|Указывает, следует ли проверять сценарии, загружаемые в браузере Internet Explorer.|
|defenderSignatureUpdateIntervalInHours|Int32|Интервал обновления сигнатур (в часах). Укажите 0, чтобы не проверять. Допустимые значения: от 0 до 24.|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|Тип проверки системы Защитником. Возможные значения: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledScanTime|TimeOfDay|Время проверки системы Защитником.|
|defenderScheduledQuickScanTime|TimeOfDay|Время ежедневной быстрой проверки.|
|defenderCloudBlockLevel|[дефендерклаудблокклевелтипе](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Определяет уровень облачной защиты. Возможные значения: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|дефендерклаудекстендедтимеаут|Int32|Расширение времени ожидания для сканирования файлов в облаке. Допустимые значения: от 0 до 50.|
|дефендерклаудекстендедтимеаутинсекондс|Int32|Расширение времени ожидания для сканирования файлов в облаке. Допустимые значения: от 0 до 50.|
|дефендерблокконакцесспротектион|Логический|Разрешает или запрещает защитник Windows для функций защиты доступа.|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md);|Проверка уровня согласия пользователя в Защитнике Windows для отправки данных. Возможные значения: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|lockScreenAllowTimeoutConfiguration|Логический|Указывает, следует ли отображать настройку, позволяющую определить время до отключения экрана на экране блокировки мобильных устройств с Windows 10. Если для этой политики установлено значение Allow, значение, заданное свойством lockScreenTimeoutInSeconds, игнорируется.|
|lockScreenBlockActionCenterNotifications|Логический|Указывает, следует ли запретить показ уведомлений из центра уведомлений на экране блокировки.|
|lockScreenBlockCortana|Логический|Указывает, может ли пользователь взаимодействовать с Кортаной с помощью голоса при заблокированной системе.|
|lockScreenBlockToastNotifications|Логический|Указывает, следует ли показывать всплывающие уведомления на экране блокировки устройства.|
|lockScreenTimeoutInSeconds|Int32|Установите время (в секундах) от блокировки экрана до его выключения для мобильных устройств с Windows 10. Поддерживаемые значения: от 11 до 1800. Допустимые значения: от 11 до 1800.|
|локкскринактиватеаппсвисвоице|[Включение](../resources/intune-shared-enablement.md)|Этот параметр политики определяет, могут ли приложения Windows активироваться по голосовым данным, пока система заблокирована. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|passwordBlockSimple|Логический|Укажите, разрешены ли такие ПИН-коды или пароли, как "1111" или "1234". Это свойство также контролирует использование графических паролей на компьютерах с Windows 10.|
|passwordExpirationDays|Int32|Срок действия пароля (в днях). Допустимые значения: от 0 до 730.|
|passwordMinimumLength|Int32|Минимальная длина пароля. Допустимые значения: от 4 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые требуются для пароля.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, повторное использование которых необходимо запретить. Допустимые значения: от 0 до 50.|
|passwordRequired|Логический|Указывает, обязательно ли использовать пароль.|
|passwordRequireWhenResumeFromIdleState|Boolean|Указывает, следует ли запрашивать пароль при выходе из состояния простоя.|
|passwordRequiredType|[рекуиредпассвордтипе](../resources/intune-deviceconfig-requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек. Допустимые значения: от 0 до 999.|
|пассвордминимумажеиндайс|Int32|Этот параметр безопасности определяет период времени (в днях), в течение которого необходимо использовать пароль, прежде чем пользователь сможет его изменить. Допустимые значения — от 0 до 998|
|privacyAdvertisingId|[статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|Указывает, можно ли использовать идентификатор рекламы. Добавлено в Windows 10 версии 1607. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Логический|Указывает, следует ли запретить автоматическое принятие примечаний о связывании и конфиденциальности при запуске приложений.|
|привацидисаблелаунчекспериенце|Логический|Эта политика запрещает запуск службы конфиденциальности при входе пользователя для новых и обновленных пользователей.|
|privacyBlockInputPersonalization|Логический|Указывает, следует ли запретить использовать облачные службы распознавания речи для приложений "Кортана", "Диктофон" или Store.|
|привациблоккпублишусерактивитиес|Логический|Блокирует общий доступ/обнаружение недавно использовавшихся ресурсов в переключателе задач и т. д.|
|привациблоккактивитифид|Логический|Блокирует использование облачных голосовых служб для Кортаны, диктовки или хранения приложений.|
|активатеаппсвисвоице|[Включение](../resources/intune-shared-enablement.md)|Указывает, можно ли активировать приложения Windows с помощью голосовых вызовов. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|startBlockUnpinningAppsFromTaskbar|Логический|Указывает, следует ли запретить пользователю откреплять приложения с панели задач.|
|startMenuAppListVisibility|[виндовсстартменуапплиствисибилититипе](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|Эта политика позволяет свернуть список приложений, полностью удалить этот список или отключить соответствующий переключатель в приложении "Параметры". Возможные значения: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
|startMenuHideChangeAccountSettings|Логический|Эта политика позволяет скрыть параметр для смены учетной записи на плитке пользователя в меню "Пуск".|
|startMenuHideFrequentlyUsedApps|Логический|Эта политика позволяет скрыть наиболее часто используемые приложения в меню "Пуск" и отключить соответствующий переключатель в приложении "Параметры".|
|startMenuHideHibernate|Логический|Эта политика позволяет скрыть параметр кнопки питания для перехода в режим гибернации в меню "Пуск".|
|startMenuHideLock|Логический|Эта политика позволяет скрыть параметр для блокировки экрана на плитке пользователя в меню "Пуск".|
|startMenuHidePowerButton|Логический|Эта политика позволяет скрыть кнопку питания в меню "Пуск".|
|startMenuHideRecentJumpLists|Логический|Эта политика позволяет скрыть списки последних переходов в меню "Пуск" и на панели задач, а также отключить соответствующий переключатель в приложении "Параметры".|
|startMenuHideRecentlyAddedApps|Логический|Эта политика позволяет скрыть недавно добавленные приложения в меню "Пуск" и отключить соответствующий переключатель в приложении "Параметры".|
|startMenuHideRestartOptions|Логический|Эта политика позволяет скрыть параметр кнопки питания "Перезагрузить" или "Обновить и перезагрузить" в меню "Пуск".|
|startMenuHideShutDown|Логический|Эта политика позволяет скрыть параметр кнопки питания "Завершить работу" или "Обновить и завершить работу" в меню "Пуск".|
|startMenuHideSignOut|Логический|Эта политика позволяет скрыть параметр для выхода из учетной записи на плитке пользователя в меню "Пуск".|
|startMenuHideSleep|Логический|Эта политика позволяет скрыть параметр кнопки питания для перехода в спящий режим в меню "Пуск".|
|startMenuHideSwitchAccount|Логический|Эта политика позволяет скрыть параметр для переключения между учетными записями на плитке пользователя в меню "Пуск".|
|startMenuHideUserTile|Boolean|Эта политика позволяет скрыть плитку пользователя в меню "Пуск".|
|startMenuLayoutEdgeAssetsXml|Binary|Этот параметр политики позволяет импортировать ресурсы Edge для использования с политикой startMenuLayoutXml. Макет меню "Пуск" может содержать вспомогательную плитку из приложения Edge для поиска файла локального ресурса Edge. Так как локальный ресурс Edge не существует, вспомогательная плитка Edge будет пустой. Эта политика применяется только при изменении политики startMenuLayoutXml. Значение должно быть в формате массива байтов в кодировке Base64 UTF-8.|
|startMenuLayoutXml|Binary|Позволяет администраторам переопределять стандартный макет меню "Пуск" и блокировать его изменение пользователями. Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета. XML-файл должен быть в формате массива байтов в кодировке UTF8.|
|startMenuMode|[виндовсстартменумодетипе](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|Позволяет администраторам определить вид меню "Пуск". Возможные значения: `userDefined`, `fullScreen`, `nonFullScreen`.|
|startMenuPinnedFolderDocuments|[висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Документы" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderDownloads|[висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Загрузки" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderFileExplorer|[висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык проводника в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderHomeGroup|[висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Домашняя группа" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderMusic|[висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Музыка" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderNetwork|[висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Сеть" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPersonalFolder|[висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык личной папки в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPictures|[висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Изображения" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderSettings|[висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Параметры" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderVideos|[висибилитисеттинг](../resources/intune-deviceconfig-visibilitysetting.md)|Определяет, виден ли ярлык папки "Видео" в меню "Пуск". Возможные значения: `notConfigured`, `hide`, `show`.|
|settingsBlockSettingsApp|Логический|Указывает, следует ли заблокировать доступ к приложению "Параметры".|
|settingsBlockSystemPage|Логический|Указывает, следует ли заблокировать доступ к разделу "Система" в приложении "Параметры".|
|settingsBlockDevicesPage|Логический|Указывает, следует ли заблокировать доступ к разделу "Устройства" в приложении "Параметры".|
|settingsBlockNetworkInternetPage|Логический|Указывает, следует ли заблокировать доступ к разделу "Сеть и Интернет" в приложении "Параметры".|
|settingsBlockPersonalizationPage|Логический|Указывает, следует ли заблокировать доступ к разделу "Персонализация" в приложении "Параметры".|
|settingsBlockAccountsPage|Логический|Указывает, следует ли заблокировать доступ к разделу "Учетные записи" в приложении "Параметры".|
|settingsBlockTimeLanguagePage|Логический|Указывает, следует ли заблокировать доступ к разделу "Время и язык" в приложении "Параметры".|
|settingsBlockEaseOfAccessPage|Логический|Указывает, следует ли заблокировать доступ к разделу "Специальные возможности" в приложении "Параметры".|
|settingsBlockPrivacyPage|Логический|Указывает, следует ли заблокировать доступ к разделу "Конфиденциальность" в приложении "Параметры".|
|settingsBlockUpdateSecurityPage|Логический|Указывает, следует ли заблокировать доступ к разделу "Обновление и безопасность" в приложении "Параметры".|
|settingsBlockAppsPage|Логический|Указывает, следует ли заблокировать доступ к разделу "Приложения" в приложении "Параметры".|
|settingsBlockGamingPage|Логический|Указывает, следует ли заблокировать доступ к разделу "Игры" в приложении "Параметры".|
|windowsSpotlightBlockConsumerSpecificFeatures|Логический|Позволяет ИТ-администраторам заблокировать функции, обычно доступные только для потребителей, такие как рекомендации в меню "Пуск", уведомления, связанные с членством в группе, установка приложений после запуска при первом включении компьютера и плитки перенаправления.|
|windowsSpotlightBlocked|Логический|Позволяет ИТ-администраторам отключить все функции "Windows: интересное".|
|windowsSpotlightBlockOnActionCenter|Логический|Позволяет запретить Майкрософт показывать информацию о новых возможностях или изменениях после каждой чистой установки операционной системы, обновления или на постоянной основе.|
|windowsSpotlightBlockTailoredExperiences|Логический|Позволяет заблокировать персонализацию контента на экране "Windows: интересное" на основе данных об использовании устройства.|
|windowsSpotlightBlockThirdPartyNotifications|Логический|Позволяет заблокировать сторонний контент на экране "Windows: интересное".|
|windowsSpotlightBlockWelcomeExperience|Логический|Позволяет заблокировать экран приветствия "Windows: интересное".|
|windowsSpotlightBlockWindowsTips|Логический|Позволяет ИТ-администраторам отключать всплывающие советы по использованию Windows.|
|windowsSpotlightConfigureOnLockScreen|[виндовсспотлигхтенаблементсеттингс](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|Указывает тип прожектора. Возможные значения: `notConfigured`, `disabled`, `enabled`.|
|networkProxyApplySettingsDeviceWide|Логический|Если этот параметр включен, настройки прокси-сервера применяются ко всем процессам и учетным записям на устройстве. В противном случае они применяются к учетной записи пользователя, зарегистрированной в системе MDM.|
|networkProxyDisableAutoDetect|Логический|Позволяет отключить автоматическое обнаружение настроек. Если этот параметр включен, система попытается найти путь к сценарию автонастройки прокси-сервера (PAC).|
|networkProxyAutomaticConfigurationUrl|String|Адрес сценария автонастройки прокси-сервера (PAC).|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune-deviceconfig-windows10networkproxyserver.md)|Определяет ручные настройки прокси-сервера.|
|accountsBlockAddingNonMicrosoftAccountEmail|Логический|Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.|
|antiTheftModeBlocked|Boolean|Указывает, следует ли запретить пользователю выбирать режим AntiTheft (только для Windows 10 Mobile).|
|bluetoothBlocked|Логический|Указывает, следует ли запретить использовать Bluetooth.|
|cameraBlocked|Логический|Определяет, следует ли запретить доступ к камере устройства.|
|connectedDevicesServiceBlocked|Логический|Указывает, следует ли блокировать службу подключенных устройств, которая позволяет находить другие устройства и подключаться к ним, удаленно обмениваться сообщениями и работать с приложениями, а также выполнять другие действия.|
|certificatesBlockManualRootCertificateInstallation|Логический|Указывает, следует ли запретить пользователю вручную устанавливать корневой сертификат.|
|copyPasteBlocked|Логический|Указывает, следует ли запретить пользователю копировать данные.|
|cortanaBlocked|Логический|Указывает, следует ли запретить использовать Кортану.|
|deviceManagementBlockFactoryResetOnMobile|Логический|Указывает, следует ли запретить пользователю сбрасывать настройки телефона.|
|deviceManagementBlockManualUnenroll|Логический|Указывает, следует ли запретить пользователю вручную отменять регистрацию в системе управления устройствами.|
|safeSearchFilter|[сафесеарчфилтертипе](../resources/intune-deviceconfig-safesearchfiltertype.md)|Определяет необходимый уровень фильтрации для безопасного поиска. Возможные значения: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Логический|Указывает, следует ли блокировать всплывающие окна.|
|edgeBlockSearchSuggestions|Логический|Указывает, следует ли запретить пользователю использовать варианты поиска в адресной строке.|
|еджеблокксеарченгинекустомизатион|Логический|Указывает, следует ли запретить пользователю добавлять новую поисковую систему или изменять поисковую систему по умолчанию.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Логический|Указывает, следует ли переключить трафик интрасети от края к Internet Explorer. Note: имя этого свойства является недостоверным; свойство устарело, вместо него используйте Еджесендинтранеттраффиктоинтернетексплорер.|
|еджесендинтранеттраффиктоинтернетексплорер|Логический|Указывает, следует ли переключить трафик интрасети от края к Internet Explorer.|
|edgeRequireSmartScreen|Логический|Указывает, обязательно ли использовать фильтр Smart Screen.|
|edgeEnterpriseModeSiteListLocation|String|Указывает расположение списка сайтов, запускаемых в корпоративном режиме. Это может быть локальный файл, локальная сеть или http-адрес.|
|edgeFirstRunUrl|String|URL-адрес, открываемый в браузере Edge при первом запуске.|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)|Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для управляемых с помощью системы MDM устройств. Пользователи могут переопределять эту настройку и изменять поисковую систему по умолчанию, если не установлена политика AllowSearchEngineCustomization.|
|edgeHomepageUrls|Коллекция String|Список URL-адресов домашних страниц, показываемых на зарегистрированных в системе MDM устройствах в браузере Edge.|
|edgeBlockAccessToAboutFlags|Логический|Указывает, следует ли запретить доступ к странице about flags в браузере Edge.|
|smartScreenBlockPromptOverride|Логический|Указывает, могут ли пользователи игнорировать предупреждения фильтра SmartScreen о потенциально вредоносных веб-сайтах.|
|smartScreenBlockPromptOverrideForFiles|Логический|Указывает, могут ли пользователи игнорировать предупреждения фильтра SmartScreen о скачивании непроверенных файлов.|
|webRtcBlockLocalhostIpAddress|Логический|Указывает, отображается ли IP-адрес пользователя localhost при совершении телефонных звонков с помощью WebRTC.|
|internetSharingBlocked|Логический|Указывает, следует ли запретить использовать Общий Интернет.|
|settingsBlockAddProvisioningPackage|Логический|Указывает, следует ли запретить пользователю устанавливать пакеты подготовки.|
|settingsBlockRemoveProvisioningPackage|Логический|Указывает, следует ли запретить агенту конфигурации среды выполнения удалять пакеты подготовки.|
|settingsBlockChangeSystemTime|Логический|Указывает, следует ли запретить пользователю изменять настройки даты и времени.|
|settingsBlockEditDeviceName|Логический|Указывает, следует ли запретить пользователю изменять имя устройства.|
|settingsBlockChangeRegion|Логический|Указывает, следует ли запретить пользователю изменять региональные стандарты.|
|settingsBlockChangeLanguage|Логический|Указывает, следует ли запретить пользователю изменять параметры языка.|
|settingsBlockChangePowerSleep|Boolean|Указывает, следует ли запретить пользователю изменять параметры питания и спящего режима.|
|locationServicesBlocked|Логический|Указывает, следует ли запретить использовать службы определения местоположения.|
|microsoftAccountBlocked|Логический|Указывает, следует ли запретить использовать учетную запись Майкрософт.|
|microsoftAccountBlockSettingsSync|Логический|Указывает, следует ли запретить синхронизировать настройки учетной записи Майкрософт.|
|nfcBlocked|Логический|Указывает, следует ли запретить использовать NFC.|
|resetProtectionModeBlocked|Логический|Указывает, следует ли запретить пользователю сбрасывать режим защиты.|
|screenCaptureBlocked|Логический|Указывает, следует ли запретить пользователю делать снимки экрана.|
|storageBlockRemovableStorage|Логический|Указывает, следует ли запретить использовать съемные носители.|
|storageRequireMobileDeviceEncryption|Логический|Указывает, обязательно ли шифровать данные на мобильном устройстве.|
|usbBlocked|Логический|Указывает, следует ли запретить пользователю подключать USB-устройства.|
|voiceRecordingBlocked|Логический|Указывает, следует ли запретить пользователю записывать речь.|
|wiFiBlockAutomaticConnectHotspots|Логический|Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi. Ни на что не влияет, если Wi-Fi заблокирован.|
|wiFiBlocked|Логический|Указывает, следует ли запретить использовать Wi-Fi.|
|wiFiBlockManualConfiguration|Логический|Указывает, следует ли запретить пользователю настраивать Wi-Fi вручную.|
|wiFiScanInterval|Int32|Указывает частоту поиска сетей Wi-Fi. Поддерживаемые значения: 1–500, где 100 — значение по умолчанию, а 500 — низкая частота. Допустимые значения: от 1 до 500.|
|wirelessDisplayBlockProjectionToThisDevice|Логический|Указывает, могут ли другие устройства находить этот компьютер для проецирования контента.|
|wirelessDisplayBlockUserInputFromReceiver|Логический|Указывает, следует ли блокировать запросы пользователя с беспроводного дисплея.|
|wirelessDisplayRequirePinForPairing|Логический|Указывает, обязательно ли использовать ПИН-код для связывания с новыми устройствами.|
|windowsStoreBlocked|Логический|Указывает, следует ли запретить использовать Microsoft Store.|
|appsAllowTrustedAppsSideloading|[статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|Указывает, можно ли загружать неопубликованные приложения из пакетов AppX с доверенным сертификатом. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|windowsStoreBlockAutoUpdate|Логический|Указывает, следует ли заблокировать автоматическое обновление приложений из Microsoft Store.|
|developerUnlockSetting|[статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|Указывает, следует ли разрешить разблокировку для разработки. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|sharedUserAppDataAllowed|Логический|Указывает, следует ли запретить общий доступ к данным для пользователей одного приложения.|
|appsBlockWindowsStoreOriginatedApps|Логический|Указывает, следует ли отключить запуск всех предустановленных или скачанных приложений из Microsoft Store.|
|windowsStoreEnablePrivateStoreOnly|Логический|Указывает, следует ли включить только частный магазин.|
|storageRestrictAppDataToSystemVolume|Логический|Указывает, можно ли хранить данные приложения не на системном диске.|
|storageRestrictAppInstallToSystemVolume|Логический|Указывает, можно ли устанавливать приложения не на системном диске.|
|gameDvrBlocked|Логический|Указывает, следует ли блокировать DVR и трансляцию контента.|
|experienceBlockDeviceDiscovery|Логический|Указывает, следует ли блокировать обнаружение устройств.|
|experienceBlockErrorDialogWhenNoSIM|Логический|Указывает, следует ли запретить отображение диалогового окна ошибки, если SIM-карта не обнаружена.|
|experienceBlockTaskSwitcher|Логический|Указывает, следует ли заблокировать переключение задач на устройстве.|
|logonBlockFastUserSwitching|Boolean|Отключает возможность быстрого переключения между учетными записями пользователей, вошедших в систему, без выхода из системы.|
|tenantLockdownRequireNetworkDuringOutOfBoxExperience|Логический|Указывает, требуется ли устройство для подключения к сети.|
|аппманажементмсиалловусерконтроловеринсталл|Логический|Этот параметр политики позволяет пользователям изменять параметры установки, которые обычно доступны только системным администраторам.|
|аппманажементмсиалвайсинсталлвиселеватедпривилежес|Логический|Этот параметр политики направляет установщик Windows использовать повышенные разрешения при установке любой программы в систему.|
|датапротектионблоккдиректмеморякцесс|Логический|Этот параметр политики позволяет заблокировать прямой доступ к памяти (DMA) для всех подключенных портов PCI, подключенных к горячему подключению, пока пользователь не войдет в систему Windows.|
|аппманажементпаккажефамилинаместолаунчафтерлогон|Коллекция String|Список имен семейств пакетов для приложений Windows, разделенных точкой с запятой. Перечисленные приложения Windows будут запущены после входа в систему.|
|uninstallBuiltInApps|Boolean|Указывает, следует ли удалить фиксированный список встроенных приложений Windows.|
|конфигуретимезоне|String|Указывает часовой пояс, применяемый к устройству. Это стандартное имя Windows для целевого часового пояса.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|привациакцессконтролс|Коллекция [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Указывает список приложений со своими уровнями управления доступом для категорий данных о конфиденциальности, а также уровни доступа по умолчанию для каждой категории.|

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
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 1024,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "String",
    "moderateSeverity": "String",
    "highSeverity": "String",
    "severeSeverity": "String"
  },
  "defenderSystemScanSchedule": "String",
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderScanMaxCpu": 1024,
  "defenderMonitorFileActivity": "String",
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderPotentiallyUnwantedAppActionSetting": "String",
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPromptForSampleSubmission": "String",
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
  "defenderSignatureUpdateIntervalInHours": 1024,
  "defenderScanType": "String",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeout": 1024,
  "defenderCloudExtendedTimeoutInSeconds": 1024,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "String",
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



