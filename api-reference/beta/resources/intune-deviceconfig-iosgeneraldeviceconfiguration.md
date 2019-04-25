---
title: Тип ресурса iosGeneralDeviceConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом iosGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dba0349ddfe7b0e4fd71193bbea7dd35dcf0a04
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564213"
---
# <a name="iosgeneraldeviceconfiguration-resource-type"></a>Тип ресурса iosGeneralDeviceConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом iosGeneralDeviceConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов IosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-list.md)|Коллекция [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|Перечисление свойств и связей объектов [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).|
|[Получение объекта iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-get.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md);|Чтение свойств и связей объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).|
|[Создание объекта iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-create.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md);|Создание объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).|
|[Удаление объекта iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-delete.md)|Нет|Удаление объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).|
|[Обновление объекта iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-update.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|accountBlockModification|Boolean|Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.|
|activationLockAllowWhenSupervised|Boolean|Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.|
|airDropBlocked|Boolean|Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.|
|airDropForceUnmanagedDropTarget|Boolean|Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).|
|airPlayForcePairingPasswordForOutgoingRequests|Boolean|Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.|
|appleWatchBlockPairing|Boolean|Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|appleWatchForceWristDetection|Boolean|Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).|
|appleNewsBlocked|Boolean|Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|appsSingleAppModeList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы. Только в защищенном режиме. iOS 7.0 и более поздних версий. Эта коллекция может содержать не более 500 элементов.|
|appsVisibilityList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий). Эта коллекция может содержать не более 10 000 элементов.|
|appsVisibilityListType|[Апплисттипе](../resources/intune-deviceconfig-applisttype.md)|Тип списка, определенного свойством AppsVisibilityList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Boolean|Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|appStoreBlocked|Boolean|Указывает, следует ли запретить использовать App Store.|
|appStoreBlockInAppPurchases|Boolean|Указывает, следует ли запретить пользователю совершать покупки из приложения.|
|appStoreBlockUIAppInstallation|Boolean|Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения. Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).|
|appStoreRequirePassword|Boolean|Указывает, требуется ли пароль, когда вы используете приложение App Store.|
|Аутофиллфорцеаусентикатион|Boolean|Указывает, следует ли принудительно выполнять проверку подлинности пользователей перед автозаполнением паролей и сведений о кредитных картах в Safari и других приложениях на контролируемых устройствах.|
|bluetoothBlockModification|Boolean|Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).|
|cameraBlocked|Boolean|Указывает, следует ли запретить доступ к камере устройства.|
|cellularBlockDataRoaming|Boolean|Указывает, следует ли блокировать передачу данных в роуминге.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolean|Указывает, следует ли заблокировать получение фоновых данных в роуминге.|
|cellularBlockPerAppDataModification|Boolean|Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.|
|cellularBlockPersonalHotspot|Boolean|Указывает, следует ли заблокировать личный хот-спот.|
|Целлуларблоккпланмодификатион|Boolean|Указывает, следует ли запретить пользователям изменять параметры плана сотовой связи на защищенном устройстве.|
|cellularBlockVoiceRoaming|Boolean|Указывает, следует ли заблокировать голосовой роуминг.|
|certificatesBlockUntrustedTlsCertificates|Boolean|Указывает, следует ли заблокировать ненадежные сертификаты TLS.|
|classroomAppBlockRemoteScreenObservation|Boolean|Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).|
|classroomAppForceUnpromptedScreenObservation|Boolean|Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.|
|Классрумфорцеаутоматикаллижоинклассес|Boolean|Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося, когда устройство находится в защищенном режиме.|
|Классрумфорцеунпромптедаппанддевицелокк|Boolean|Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся. Только в защищенном режиме.|
|compliantAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType). Эта коллекция может содержать не более 10 000 элементов.|
|compliantAppListType|[Апплисттипе](../resources/intune-deviceconfig-applisttype.md)|Список, указанный с помощью свойства AppComplianceList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|configurationProfileBlockChanges|Boolean|Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.|
|definitionLookupBlocked|Boolean|Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|deviceBlockEnableRestrictions|Boolean|Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.|
|deviceBlockEraseContentAndSettings|Boolean|Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.|
|deviceBlockNameModification|Boolean|Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|diagnosticDataBlockSubmission|Boolean|Указывает, следует ли заблокировать отправку диагностических данных.|
|diagnosticDataBlockSubmissionModification|Boolean|Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).|
|documentsBlockManagedDocumentsInUnmanagedApps|Boolean|Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.|
|documentsBlockUnmanagedDocumentsInManagedApps|Boolean|Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.|
|emailInDomainSuffixes|Коллекция String|Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.|
|enterpriseAppBlockTrust|Boolean|Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.|
|enterpriseAppBlockTrustModification|Boolean|Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.|
|Есимблоккмодификатион|Boolean|Указывает, следует ли разрешить добавление или удаление планов сотовой связи на eSIM контролируемого устройства.|
|faceTimeBlocked|Boolean|Указывает, следует ли запретить использовать FaceTime.|
|findMyFriendsBlocked|Boolean|Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в защищенном режиме.|
|gamingBlockGameCenterFriends|Boolean|Указывает, следует ли запретить пользователю добавлять друзей в Game Center.|
|gamingBlockMultiplayer|Boolean|Указывает, следует ли запретить пользователю играть с несколькими игроками.|
|gameCenterBlocked|Boolean|Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.|
|hostPairingBlocked|Boolean|Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.|
|iBooksStoreBlocked|Boolean|Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.|
|iBooksStoreBlockErotica|Boolean|Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".|
|iCloudBlockActivityContinuation|Boolean|Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.|
|iCloudBlockBackup|Boolean|Указывает, следует ли заблокировать резервное копирование iCloud.|
|iCloudBlockDocumentSync|Boolean|Указывает, следует ли заблокировать синхронизацию документов iCloud.|
|iCloudBlockManagedAppsSync|Boolean|Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.|
|iCloudBlockPhotoLibrary|Boolean|Указывает, следует ли заблокировать медиатеку iCloud.|
|iCloudBlockPhotoStreamSync|Boolean|Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.|
|iCloudBlockSharedPhotoStream|Boolean|Указывает, следует ли заблокировать общий фотопоток.|
|iCloudRequireEncryptedBackup|Boolean|Указывает, обязательно ли шифровать резервные копии iCloud.|
|iTunesBlockExplicitContent|Boolean|Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.|
|iTunesBlockMusicService|Boolean|Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).|
|iTunesBlockRadio|Boolean|Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).|
|keyboardBlockAutoCorrect|Boolean|Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|keyboardBlockDictation|Boolean|Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.|
|keyboardBlockPredictive|Boolean|Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|keyboardBlockShortcuts|Boolean|Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|keyboardBlockSpellCheck|Boolean|Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|kioskModeAllowAssistiveSpeak|Boolean|Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.|
|kioskModeAllowAssistiveTouchSettings|Boolean|Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.|
|kioskModeAllowAutoLock|Boolean|Указывает, следует ли запретить автоблокировку устройства в режиме киоска.|
|kioskModeAllowColorInversionSettings|Boolean|Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.|
|kioskModeAllowRingerSwitch|Boolean|Указывает, можно ли использовать переключатель звонка в режиме киоска.|
|kioskModeAllowScreenRotation|Boolean|Указывает, следует ли запретить поворот экрана в режиме киоска.|
|kioskModeAllowSleepButton|Boolean|Указывает, можно ли использовать кнопку "Сон" в режиме киоска.|
|kioskModeAllowTouchscreen|Boolean|Указывает, можно ли использовать сенсорный экран в режиме киоска.|
|kioskModeAllowVoiceOverSettings|Boolean|Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.|
|kioskModeAllowVolumeButtons|Boolean|Указывает, можно ли использовать кнопки громкости в режиме киоска.|
|kioskModeBlockVolumeButtons|Boolean|Указывает, следует ли блокировать кнопки громкости в режиме терминала.|
|kioskModeAllowZoomSettings|Boolean|Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.|
|kioskModeAppStoreUrl|String|URL-адрес приложения в App Store для использования в режиме киоска. Используйте, если свойство KioskModeManagedAppId не известно.|
|Киоскмодебуилтинаппид|String|Идентификатор встроенных приложений для использования в режиме киоска. Используется, когда KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.|
|kioskModeRequireAssistiveTouch|Boolean|Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.|
|kioskModeRequireColorInversion|Boolean|Указывает, обязательно ли использовать инверсию цвета в режиме киоска.|
|kioskModeRequireMonoAudio|Boolean|Указывает, обязательно ли использовать монозвук в режиме киоска.|
|kioskModeRequireVoiceOver|Boolean|Указывает, обязательно ли использовать VoiceOver в режиме киоска.|
|kioskModeRequireZoom|Boolean|Указывает, обязательно ли использовать масштабирование в режиме киоска.|
|kioskModeManagedAppId|String|Идентификатор управляемого приложения для использования в режиме киоска. Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.|
|lockScreenBlockControlCenter|Boolean|Указывает, следует ли запретить использовать центр управления на заблокированном экране.|
|lockScreenBlockNotificationView|Boolean|Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.|
|lockScreenBlockPassbook|Boolean|Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.|
|lockScreenBlockTodayView|Boolean|Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.|
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
|mediaContentRatingApps|[Ратингаппстипе](../resources/intune-deviceconfig-ratingappstype.md)|Параметры оценки контента мультимедиа для приложений. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.|
|messagesBlocked|Boolean|Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.|
|notificationsBlockSettingsModification|Boolean|Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).|
|passcodeBlockFingerprintUnlock|Boolean|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passcodeBlockFingerprintModification|Boolean|Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.|
|passcodeBlockModification|Boolean|Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).|
|passcodeBlockSimple|Логический|Указывает, следует ли заблокировать простые секретные коды.|
|passcodeExpirationDays|Int32|Количество дней до окончания срока действия секретного кода. Допустимые значения: от 1 до 65 535.|
|passcodeMinimumLength|Int32|Минимальная длина секретного кода. Допустимые значения: от 4 до 14.|
|passcodeMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах) до запроса пароля.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passcodeMinimumCharacterSetCount|Int32|Количество наборов символов, которые должен содержать секретный код. Допустимые значения: от 0 до 4.|
|passcodePreviousPasscodeBlockCount|Int32|Количество предыдущих секретных кодов, которые следует блокировать. Допустимые значения: от 1 до 24.|
|passcodeSignInFailureCountBeforeWipe|Int32|Количество неудачных попыток входа до очистки устройства. Допустимые значения: от 4 до 11.|
|passcodeRequiredType|[Рекуиредпассвордтипе](../resources/intune-deviceconfig-requiredpasswordtype.md)|Необходимый тип секретного кода. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Boolean|Указывает, обязательно ли использовать секретный код.|
|podcastsBlocked|Boolean|Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).|
|Проксимитиблокксетуптоневдевице|Boolean|Указывает, следует ли включить запрос на установку находящихся рядом устройств с защищенным устройством.|
|safariBlockAutofill|Boolean|Указывает, следует ли запретить использовать автозаполнение в Safari.|
|safariBlockJavaScript|Boolean|Указывает, следует ли заблокировать JavaScript в Safari.|
|safariBlockPopups|Boolean|Указывает, следует ли блокировать всплывающие окна в Safari.|
|safariBlocked|Boolean|Указывает, следует ли запретить использовать Safari.|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Настройки файлов cookie для Safari. Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|Коллекция String|URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.|
|safariPasswordAutoFillDomains|Коллекция String|Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам. Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).|
|safariRequireFraudWarning|Boolean|Указывает, обязательно ли предупреждение о мошенничестве в Safari.|
|screenCaptureBlocked|Boolean|Указывает, следует ли запретить пользователю делать снимки экрана.|
|siriBlocked|Boolean|Указывает, следует ли запретить использовать Siri.|
|siriBlockedWhenLocked|Boolean|Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.|
|siriBlockUserGeneratedContent|Boolean|Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.|
|siriRequireProfanityFilter|Boolean|Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.|
|Софтвареупдатесенфорцедделайиндайс|Int32|Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства. Допустимые значения: от 0 до 90.|
|Софтвареупдатесфорцеделайед|Boolean|Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.|
|spotlightBlockInternetResults|Boolean|Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.|
|voiceDialingBlocked|Boolean|Указывает, следует ли заблокировать голосовой набор.|
|wallpaperBlockModification|Boolean|Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.|
|Классрумфорцерекуестпермиссионтолеавеклассес|Boolean|Указывает, является ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса (iOS 11,3 и более поздних версий).|
|Кэйчаинблоккклаудсинк|Boolean|Указывает, заблокирована ли синхронизация ключей iCloud для iCloud.|
|Пкиблоккотаупдатес|Boolean|Указывает, блокируются ли обновления PKI беспроводной сети. Если задать для этого ограничения значение false, проверки CRL и OCSP (iOS 7,0 и более поздних версий) не отключаются.|
|Привацифорцелимитадтраккинг|Boolean|Указывает, ограничено ли отслеживание AD. (iOS 7,0 и более поздних версий).|
|Ентерприсебукблоккбаккуп|Boolean|Указывает, блокируется ли резервное копирование корпоративной книги.|
|Ентерприсебукблоккметадатасинк|Boolean|Указывает, блокируется ли синхронизация заметок и выделений корпоративных книг.|
|airPrintBlocked|Boolean|Указывает, заблокировано ли Аирпринт (iOS 11,0 и более поздних версий).|
|Аирпринтблокккредентиалсстораже|Boolean|Указывает, заблокировано ли хранение цепочки ключей имени пользователя и пароля для Аирпринт (iOS 11,0 и более поздних версий).|
|airPrintForceTrustedTLS|Boolean|Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (iOS 11,0 и более поздних версий).|
|airPrintBlockiBeaconDiscovery|Boolean|Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт. Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (iOS 11,0 и более поздних версий).|
|Блокксистемаппремовал|Boolean|Указывает, заблокировано ли удаление системных приложений с устройства на контролируемом устройстве (iOS 11,0 и более поздних версий).|
|Впнблокккреатион|Boolean|Указывает, блокируется ли создание конфигураций VPN (iOS 11,0 и более поздних версий).|
|Аппремовалблоккед|Boolean|Указывает, разрешено ли удаление приложений.|
|Усбрестриктедмодеблоккед|Boolean|Указывает, разрешена ли подключаться к стандарту USB, пока устройство заблокировано (iOS 11.4.1 и более поздних версий).|
|Пассвордблоккаутофилл|Boolean|Указывает, разрешена ли функция автоЗаполнения паролей (iOS 12,0 и более поздних версий).|
|Пассвордблоккпроксимитирекуестс|Boolean|Указывает, следует ли запретить запрашивать пароли с близлежащих устройств (iOS 12,0 и более поздних версий).|
|Пассвордблоккаирдропшаринг|Boolean|Указывает, следует ли заблокировать общий доступ к паролям с помощью AirDrop паролей iOS 12,0 и более поздних версий.|
|Датеандтимефорцесетаутоматикалли|Boolean|Указывает, включена ли функция даты и времени "автоматически задано" и не может быть отключена пользователем (iOS 12,0 и более поздних версий).|
|Контактсалловманажедтаунманажедврите|Boolean|Указывает, могут ли управляемые приложения записывать контакты в неуправляемые учетные записи контактов (iOS 12,0 и более поздних версий).|
|Контактсалловунманажедтоманажедреад|Boolean|Указывает, могут ли неуправляемые приложения читать из управляемых учетных записей контактов (iOS 12,0 или более поздней версии).|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|

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
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "esimBlockModification": true,
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
  "proximityBlockSetupToNewDevice": true,
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
  "softwareUpdatesEnforcedDelayInDays": 1024,
  "softwareUpdatesForceDelayed": true,
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





