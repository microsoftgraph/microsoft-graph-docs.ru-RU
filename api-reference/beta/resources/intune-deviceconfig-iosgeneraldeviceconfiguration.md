---
title: Тип ресурса iosGeneralDeviceConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b1a8b37bb728033ea6d2ee67f63d395a69aa0ae
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671355"
---
# <a name="iosgeneraldeviceconfiguration-resource-type"></a>Тип ресурса iosGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|appsVisibilityListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Тип списка, определенного свойством AppsVisibilityList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Boolean|Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|appStoreBlocked|Boolean|Указывает, следует ли запретить использовать App Store. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|appStoreBlockInAppPurchases|Boolean|Указывает, следует ли запретить пользователю совершать покупки из приложения.|
|appStoreBlockUIAppInstallation|Boolean|Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения. Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).|
|appStoreRequirePassword|Boolean|Указывает, требуется ли пароль, когда вы используете приложение App Store.|
|autoFillForceAuthentication|Логическое|Указывает, следует ли принудительно выполнять проверку подлинности пользователя перед автозаполнением паролей и данных кредитной карты в Safari и других приложениях на защищенных устройствах.|
|bluetoothBlockModification|Boolean|Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).|
|cameraBlocked|Boolean|Указывает, следует ли запретить доступ к камере устройства. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|cellularBlockDataRoaming|Boolean|Указывает, следует ли блокировать передачу данных в роуминге.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolean|Указывает, следует ли заблокировать получение фоновых данных в роуминге.|
|cellularBlockPerAppDataModification|Boolean|Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.|
|cellularBlockPersonalHotspot|Boolean|Указывает, следует ли заблокировать личный хот-спот.|
|cellularBlockPlanModification|Логическое|Указывает, следует ли разрешить пользователям изменять параметры плана сотовой связи на защищенном устройстве.|
|cellularBlockVoiceRoaming|Boolean|Указывает, следует ли заблокировать голосовой роуминг.|
|certificatesBlockUntrustedTlsCertificates|Boolean|Указывает, следует ли заблокировать ненадежные сертификаты TLS.|
|classroomAppBlockRemoteScreenObservation|Boolean|Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).|
|classroomAppForceUnpromptedScreenObservation|Boolean|Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.|
|classroomForceAutomaticallyJoinClasses|Логическое|Указывает, следует ли автоматически предоставлять разрешения на запросы преподавателя без запроса учащегося, когда устройство находится в защищенном режиме.|
|classroomForceUnpromptedAppAndDeviceLock|Логическое|Указывает, следует ли разрешить преподавателю блокировать приложения или устройство без запроса учащегося. Только в защищенном режиме.|
|compliantAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType). Эта коллекция может содержать не более 10 000 элементов.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Список, указанный с помощью свойства AppComplianceList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
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
|enterpriseAppBlockTrustModification|Boolean|\[Нерекомендуемая\] настройка этого параметра и установка значения true не влияет на устройство.|
|esimBlockModification|Логическое|Указывает, следует ли разрешить добавление или удаление планов сотовой связи на eSIM защищенного устройства.|
|faceTimeBlocked|Boolean|Указывает, следует ли запретить использовать FaceTime. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|findMyFriendsBlocked|Boolean|Указывает, следует ли блокировать изменения в функции "Найти друзей", когда устройство находится в защищенном режиме.|
|gamingBlockGameCenterFriends|Boolean|Указывает, следует ли запретить пользователю добавлять друзей в Game Center. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|gamingBlockMultiplayer|Boolean|Указывает, следует ли запретить пользователю играть с несколькими игроками. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|gameCenterBlocked|Boolean|Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.|
|hostPairingBlocked|Boolean|Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.|
|iBooksStoreBlocked|Boolean|Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.|
|iBooksStoreBlockErotica|Boolean|Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".|
|iCloudBlockActivityContinuation|Boolean|Указывает, следует ли запретить пользователю продолжать работу, запущенную на устройстве iOS, на другое устройство iOS или macOS.|
|iCloudBlockBackup|Boolean|Указывает, следует ли заблокировать резервное копирование iCloud. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|iCloudBlockDocumentSync|Boolean|Указывает, следует ли блокировать синхронизацию документов iCloud. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|iCloudBlockManagedAppsSync|Boolean|Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.|
|iCloudBlockPhotoLibrary|Boolean|Указывает, следует ли заблокировать медиатеку iCloud.|
|iCloudBlockPhotoStreamSync|Boolean|Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.|
|iCloudBlockSharedPhotoStream|Boolean|Указывает, следует ли заблокировать общий фотопоток.|
|iCloudRequireEncryptedBackup|Boolean|Указывает, обязательно ли шифровать резервные копии iCloud.|
|iTunesBlockExplicitContent|Boolean|Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|iTunesBlockMusicService|Boolean|Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).|
|iTunesBlockRadio|Boolean|Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).|
|keyboardBlockAutoCorrect|Boolean|Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|keyboardBlockDictation|Boolean|Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.|
|keyboardBlockPredictive|Boolean|Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|keyboardBlockShortcuts|Boolean|Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|keyboardBlockSpellCheck|Boolean|Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|kioskModeAllowAssistiveSpeak|Boolean|Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.|
|kioskModeAllowAssistiveTouchSettings|Boolean|Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.|
|kioskModeAllowAutoLock|Boolean|Указывает, следует ли запретить автоблокировку устройства в режиме киоска. Функциональные возможности этого свойства избыточны с использованием ОС по умолчанию и являются устаревшими. Вместо этого используйте KioskModeBlockAutoLock.|
|kioskModeBlockAutoLock|Логическое|Указывает, следует ли блокировать автоматическую блокировку устройства в режиме киоска.|
|kioskModeAllowColorInversionSettings|Boolean|Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.|
|kioskModeAllowRingerSwitch|Boolean|Указывает, можно ли использовать переключатель звонка в режиме киоска. Функциональные возможности этого свойства избыточны с использованием ОС по умолчанию и являются устаревшими. Вместо этого используйте KioskModeBlockRingerSwitch.|
|kioskModeBlockRingerSwitch|Логическое|Указывает, следует ли блокировать использование коммутатора звонка в режиме киоска.|
|kioskModeAllowScreenRotation|Boolean|Указывает, следует ли запретить поворот экрана в режиме киоска. Функциональные возможности этого свойства избыточны с использованием ОС по умолчанию и являются устаревшими. Вместо этого используйте KioskModeBlockScreenRotation.|
|kioskModeBlockScreenRotation|Логическое|Указывает, следует ли блокировать поворот экрана в режиме киоска.|
|kioskModeAllowSleepButton|Boolean|Указывает, можно ли использовать кнопку "Сон" в режиме киоска. Функциональные возможности этого свойства избыточны с использованием ОС по умолчанию и являются устаревшими. Вместо этого используйте KioskModeBlockBlockButton.|
|kioskModeBlockSleepButton|Boolean|Указывает, следует ли блокировать использование кнопки спящего режима в режиме киоска.|
|kioskModeAllowTouchscreen|Boolean|Указывает, можно ли использовать сенсорный экран в режиме киоска. Функциональные возможности этого свойства избыточны с использованием ОС по умолчанию и являются устаревшими. Вместо этого используйте kioskModeBlockTouchscreen.|
|kioskModeBlockTouchscreen|Логическое|Указывает, следует ли блокировать использование сенсорного экрана в режиме киоска.|
|kioskModeEnableVoiceControl|Логическое|Указывает, следует ли включить голосовое управление в режиме киоска.|
|kioskModeAllowVoiceControlModification|Логическое|Указывает, следует ли разрешить пользователю переключать голосовое управление в режиме киоска.|
|kioskModeAllowVoiceOverSettings|Boolean|Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.|
|kioskModeAllowVolumeButtons|Boolean|Указывает, можно ли использовать кнопки громкости в режиме киоска. Функциональные возможности этого свойства избыточны с использованием ОС по умолчанию и являются устаревшими. Вместо этого используйте KioskModeBlockVolumeButtons.|
|kioskModeBlockVolumeButtons|Boolean|Указывает, следует ли блокировать кнопки громкости в режиме терминала.|
|kioskModeAllowZoomSettings|Boolean|Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.|
|kioskModeAppStoreUrl|String|URL-адрес приложения в App Store для использования в режиме киоска. Используйте, если свойство KioskModeManagedAppId не известно.|
|kioskModeBuiltInAppId|String|Идентификатор встроенных приложений для использования в режиме киоска. Используется, если параметры KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.|
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
|mediaContentRatingApps|[ratingAppsType](../resources/intune-deviceconfig-ratingappstype.md)|Параметры оценки содержимого мультимедиа для приложений. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.|
|messagesBlocked|Boolean|Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.|
|notificationsBlockSettingsModification|Boolean|Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).|
|passcodeBlockFingerprintUnlock|Boolean|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passcodeBlockFingerprintModification|Boolean|Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.|
|passcodeBlockModification|Boolean|Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).|
|passcodeBlockSimple|Boolean|Указывает, следует ли заблокировать простые секретные коды.|
|passcodeExpirationDays|Int32|Количество дней до окончания срока действия секретного кода. Допустимые значения: от 1 до 65 535.|
|passcodeMinimumLength|Int32|Минимальная длина секретного кода. Допустимые значения: от 4 до 14.|
|passcodeMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах) до запроса пароля.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passcodeMinimumCharacterSetCount|Int32|Количество наборов символов, которые должен содержать секретный код. Допустимые значения: от 0 до 4.|
|passcodePreviousPasscodeBlockCount|Int32|Количество предыдущих секретных кодов, которые следует блокировать. Допустимые значения: от 1 до 24.|
|passcodeSignInFailureCountBeforeWipe|Int32|Количество неудачных попыток входа до очистки устройства. Допустимые значения от 2 до 11|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Необходимый тип секретного кода. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Boolean|Указывает, обязательно ли использовать секретный код.|
|podcastsBlocked|Boolean|Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).|
|proximityBlockSetupToNewDevice|Boolean|Указывает, следует ли включить запрос на настройку ближайших устройств с защищенным устройством.|
|safariBlockAutofill|Boolean|Указывает, следует ли запретить использовать автозаполнение в Safari. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|safariBlockJavaScript|Boolean|Указывает, следует ли заблокировать JavaScript в Safari.|
|safariBlockPopups|Boolean|Указывает, следует ли блокировать всплывающие окна в Safari.|
|safariBlocked|Boolean|Указывает, следует ли запретить использовать Safari. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Настройки файлов cookie для Safari. Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|Коллекция String|URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.|
|safariPasswordAutoFillDomains|Коллекция String|Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам. Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).|
|safariRequireFraudWarning|Boolean|Указывает, обязательно ли предупреждение о мошенничестве в Safari.|
|screenCaptureBlocked|Boolean|Указывает, следует ли запретить пользователю делать снимки экрана.|
|siriBlocked|Boolean|Указывает, следует ли запретить использовать Siri.|
|siriBlockedWhenLocked|Boolean|Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.|
|siriBlockUserGeneratedContent|Boolean|Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.|
|siriRequireProfanityFilter|Boolean|Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.|
|softwareUpdatesEnforcedDelayInDays|Int32|Задает количество дней, в течение которых будет выполняться отладка обновления программного обеспечения для защищенного устройства. Допустимые значения: от 0 до 90.|
|softwareUpdatesForceDelayed|Логический|Указывает, следует ли откладывать видимость обновлений программного обеспечения пользователями, когда устройство находится в защищенном режиме.|
|spotlightBlockInternetResults|Boolean|Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.|
|voiceDialingBlocked|Boolean|Указывает, следует ли заблокировать голосовой набор.|
|wallpaperBlockModification|Boolean|Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме. Доступно для устройств под управлением iOS и iPadOS версий 14.4 и более ранних версий. Устройства под управлением версии 14.5 и выше должны использовать параметр WiFiConnectToAllowedNetworksOnlyForced.|
|classroomForceRequestPermissionToLeaveClasses|Логическое|Указывает, будет ли учащийся, зарегистрированный в неуправляемом курсе через Classroom, запрашивать разрешение у преподавателя при попытке покинуть курс (iOS 11.3 и более поздних версий).|
|keychainBlockCloudSync|Логическое|Указывает, заблокирована ли синхронизация цепочки ключей iCloud. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|pkiBlockOTAUpdates|Логическое|Указывает, блокируются ли обновления PKI по беспроводной сети. Установка этого ограничения на false не отключает проверки CRL и OCSP (iOS 7.0 и более поздних версий).|
|privacyForceLimitAdTracking|Логическое|Указывает, ограничено ли отслеживание. (iOS 7.0 и более поздних версий).|
|enterpriseBookBlockBackup|Логическое|Указывает, заблокировано ли резервное копирование корпоративных книг.|
|enterpriseBookBlockMetadataSync|Логическое|Указывает, заблокирована ли синхронизация корпоративных заметок и выделений.|
|airPrintBlocked|Логическое|Указывает, заблокирован ли AirPrint (iOS 11.0 и более поздних версий).|
|airPrintBlockCredentialsStorage|Логическое|Указывает, заблокировано ли хранилище имени пользователя и пароля цепочки ключей для Airprint (iOS 11.0 и более поздних версий).|
|airPrintForceTrustedTLS|Логическое|Указывает, требуются ли доверенные сертификаты для связи с печатью по протоколу TLS (iOS 11.0 и более поздних версий).|
|airPrintBlockiBeaconDiscovery|Логическое|Указывает, заблокировано ли обнаружение принтеров AirPrint iBeacon. Это предотвращает ложные маяки Bluetooth AirPrint от фишинга для сетевого трафика (iOS 11.0 и более поздних версий).|
|filesNetworkDriveAccessBlocked|Логическое|Указывает, могут ли устройства получать доступ к файлам или другим ресурсам на сетевом сервере с помощью протокола SMB. Доступно для устройств под управлением iOS и iPadOS версии 13.0 и более поздних версий.|
|filesUsbDriveAccessBlocked|Логическое|Указывает, могут ли разделители с доступом подключаться к файлам и открывать их на USB-накопителе. Доступно для устройств под управлением iOS и iPadOS версии 13.0 и более поздних версий.|
|wifiPowerOnForced|Логическое|Указывает, включена ли Wi-Fi, даже если устройство находится в режиме "в самолете". Доступно для устройств под управлением iOS и iPadOS версии 13.0 и более поздних версий.|
|blockSystemAppRemoval|Логическое|Указывает, блокируется ли удаление системных приложений с устройства на защищенном устройстве (iOS 11.0 и более поздних версий).|
|vpnBlockCreation|Логическое|Указывает, заблокировано ли создание конфигураций VPN (iOS 11.0 и более поздних версий).|
|appRemovalBlocked|Логическое|Указывает, разрешено ли удаление приложений.|
|usbRestrictedModeBlocked|Логическое|Указывает, разрешено ли подключение к USB-аксессуарам во время блокировки устройства (iOS 11.4.1 и более поздних версий).|
|passwordBlockAutoFill|Логическое|Указывает, разрешена ли функция автозаполнения паролей (iOS 12.0 и более поздних версий).|
|passwordBlockProximityRequests|Логическое|Указывает, следует ли блокировать запрос паролей с ближайших устройств (iOS 12.0 и более поздних версий).|
|passwordBlockAirDropSharing|Логическое|Указывает, следует ли блокировать общий доступ к паролям с помощью функции паролей AirDrop iOS 12.0 и более поздних версий.|
|dateAndTimeForceSetAutomatically|Логическое|Указывает, включена ли функция "Настройка даты и времени автоматически" и не может быть отключена пользователем (iOS 12.0 и более поздних версий).|
|contactsAllowManagedToUnmanagedWrite|Логическое|Указывает, могут ли управляемые приложения записывать контакты в неуправляемые учетные записи контактов (iOS 12.0 и более поздние версии).|
|contactsAllowUnmanagedToManagedRead|Логическое|Указывает, могут ли неуправляемые приложения считывать данные из управляемых учетных записей контактов (iOS 12.0 или более поздней версии).|
|cellularBlockPersonalHotspotModification|Логическое|Указывает, следует ли запретить пользователю изменять параметр личного хот-спота (iOS 12.2 или более поздней версии).|
|continuousPathKeyboardBlocked|Логическое|Указывает, следует ли блокировать клавиатуру непрерывного пути при защищенном устройстве (iOS 13 или более поздней версии).|
|findMyDeviceInFindMyAppBlocked|Логическое|Указывает, следует ли блокировать функцию "Найти мое устройство" при защищенном устройстве (iOS 13 или более поздней версии).|
|findMyFriendsInFindMyAppBlocked|Логическое|Указывает, следует ли блокировать поиск друзей при защищенном устройстве (iOS 13 или более поздней версии).|
|iTunesBlocked|Логическое|Указывает, следует ли блокировать приложение iTunes. Требуется защищенное устройство для iOS 13 и более поздних версий.|
|sharedDeviceBlockTemporarySessions|Логическое|Указывает, следует ли блокировать временные сеансы на общих устройствах iPad (iOS 13.4 или более поздней версии).|
|appClipsBlocked|Логическое|Запрещает пользователю добавлять клипы приложений и удаляет все существующие клипы приложений на устройстве.|
|applePersonalizedAdsBlocked|Логическое|Ограничивает персонализированную рекламу Apple, если это так. Доступно в iOS 14 и более поздних версиях.|
|nfcBlocked|Boolean|Отключите NFC, чтобы предотвратить связывание устройств с другими устройствами с поддержкой NFC. Доступно для устройств iOS и iPadOS под управлением 14.2 и более поздних версий.|
|autoUnlockBlocked|Логическое|Блокирует разблокировку устройства с помощью Apple Watch. Доступно для устройств под управлением iOS и iPadOS версии 14.5 и более поздних.|
|unpairedExternalBootToRecoveryAllowed|Логическое|Разрешить пользователям запускать устройства в режим восстановления с непарными устройствами. Доступно для устройств под управлением iOS и iPadOS версии 14.5 и более поздних.|
|onDeviceOnlyDictationForced|Логический|Отключает подключения к серверам Siri, чтобы пользователи не могли использовать Siri для диктовки текста. Доступно для устройств под управлением iOS и iPadOS версии 14.5 и более поздних.|
|wiFiConnectToAllowedNetworksOnlyForced|Логическое|Требовать, чтобы устройства Wi-Fi сети, настраивались с помощью профилей конфигурации. Доступно для устройств под управлением iOS и iPadOS версии 14.5 и более поздних.|
|onDeviceOnlyTranslationForced|Логическое|Если задано значение TRUE, параметр отключает подключения к серверам Siri, чтобы пользователи не могли использовать Siri для перевода текста. Если задано значение FALSE, этот параметр разрешает подключения к серверам Siri, чтобы пользователи могли использовать Siri для перевода текста. Доступно для устройств под управлением iOS и iPadOS версии 15.0 и более поздних версий.|
|managedPasteboardRequired|Логическое|Управление открытым доступом определяет, как пользователи могут совместно использовать данные между неуправляемыми и управляемыми приложениями. При установке значения true применяются ограничения копирования и вставки в зависимости от настройки блокировки просмотра корпоративных документов в неуправляемых приложениях и блокировки просмотра некоркоративных документов в корпоративных <b> приложениях.</b> <b> </b>|
|iCloudPrivateRelayBlocked|Логическое|Частный ретранслятор iCloud — это служба iCloud+, которая запрещает сетям и серверам наблюдение за действиями пользователя в Интернете. Блокируя частный ретранслятор iCloud, Apple не шифрует трафик, исходящий с устройства. Доступно для устройств под управлением iOS 15 и более поздних версий.|
|kioskModeAppType|[iosKioskModeAppType](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|Тип приложения для запуска в режиме киоска. Возможные значения: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.|

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
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeEnableVoiceControl": true,
  "kioskModeAllowVoiceControlModification": true,
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
  "filesNetworkDriveAccessBlocked": true,
  "filesUsbDriveAccessBlocked": true,
  "wifiPowerOnForced": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true,
  "sharedDeviceBlockTemporarySessions": true,
  "appClipsBlocked": true,
  "applePersonalizedAdsBlocked": true,
  "nfcBlocked": true,
  "autoUnlockBlocked": true,
  "unpairedExternalBootToRecoveryAllowed": true,
  "onDeviceOnlyDictationForced": true,
  "wiFiConnectToAllowedNetworksOnlyForced": true,
  "onDeviceOnlyTranslationForced": true,
  "managedPasteboardRequired": true,
  "iCloudPrivateRelayBlocked": true,
  "kioskModeAppType": "String"
}
```




