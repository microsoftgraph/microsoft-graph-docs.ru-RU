---
title: Create iosGeneralDeviceConfiguration
description: Создание объекта iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42896574ce799467bb3f4591b719bd41139e1582
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439058"
---
# <a name="create-iosgeneraldeviceconfiguration"></a>Create iosGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).

## <a name="prerequisites"></a>Необходимые разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта iosGeneralDeviceConfiguration в формате JSON.

Ниже показаны свойства, которые необходимо указывать при создании объекта iosGeneralDeviceConfiguration.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Логическое|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|accountBlockModification|Логическое|Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.|
|activationLockAllowWhenSupervised|Логическое|Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.|
|airDropBlocked|Логическое|Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.|
|airDropForceUnmanagedDropTarget|Логическое|Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).|
|airPlayForcePairingPasswordForOutgoingRequests|Логическое|Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.|
|appleWatchBlockPairing|Логическое|Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|appleWatchForceWristDetection|Логическое|Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).|
|appleNewsBlocked|Логическое|Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|appsSingleAppModeList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы. Только в защищенном режиме. iOS 7.0 и более поздних версий. Эта коллекция может содержать не более 500 элементов.|
|appsVisibilityList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий). Эта коллекция может содержать не более 10 000 элементов.|
|appsVisibilityListType|[апплисттипе](../resources/intune-deviceconfig-applisttype.md)|Тип списка, определенного свойством AppsVisibilityList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Логическое|Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|appStoreBlocked|Boolean|Указывает, следует ли запретить использовать App Store. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|appStoreBlockInAppPurchases|Логическое|Указывает, следует ли запретить пользователю совершать покупки из приложения.|
|appStoreBlockUIAppInstallation|Логическое|Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения. Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).|
|appStoreRequirePassword|Логическое|Указывает, требуется ли пароль, когда вы используете приложение App Store.|
|аутофиллфорцеаусентикатион|Логическое|Указывает, следует ли принудительно выполнять проверку подлинности пользователей перед автозаполнением паролей и сведений о кредитных картах в Safari и других приложениях на контролируемых устройствах.|
|bluetoothBlockModification|Логическое|Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).|
|cameraBlocked|Логическое|Указывает, следует ли запретить доступ к камере устройства. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|cellularBlockDataRoaming|Логическое|Указывает, следует ли блокировать передачу данных в роуминге.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Логическое|Указывает, следует ли заблокировать получение фоновых данных в роуминге.|
|cellularBlockPerAppDataModification|Логическое|Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.|
|cellularBlockPersonalHotspot|Логическое|Указывает, следует ли заблокировать личный хот-спот.|
|целлуларблоккпланмодификатион|Логическое|Указывает, следует ли запретить пользователям изменять параметры плана сотовой связи на защищенном устройстве.|
|cellularBlockVoiceRoaming|Логическое|Указывает, следует ли заблокировать голосовой роуминг.|
|certificatesBlockUntrustedTlsCertificates|Логическое|Указывает, следует ли заблокировать ненадежные сертификаты TLS.|
|classroomAppBlockRemoteScreenObservation|Логическое|Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).|
|classroomAppForceUnpromptedScreenObservation|Логическое|Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.|
|классрумфорцеаутоматикаллижоинклассес|Логическое|Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося, когда устройство находится в защищенном режиме.|
|классрумфорцеунпромптедаппанддевицелокк|Логическое|Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся. Только в защищенном режиме.|
|compliantAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType). Эта коллекция может содержать не более 10 000 элементов.|
|compliantAppListType|[апплисттипе](../resources/intune-deviceconfig-applisttype.md)|Список, указанный с помощью свойства AppComplianceList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|configurationProfileBlockChanges|Логическое|Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.|
|definitionLookupBlocked|Логическое|Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|deviceBlockEnableRestrictions|Логическое|Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.|
|deviceBlockEraseContentAndSettings|Логическое|Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.|
|deviceBlockNameModification|Логическое|Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|diagnosticDataBlockSubmission|Логическое|Указывает, следует ли заблокировать отправку диагностических данных.|
|diagnosticDataBlockSubmissionModification|Логическое|Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).|
|documentsBlockManagedDocumentsInUnmanagedApps|Логическое|Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.|
|documentsBlockUnmanagedDocumentsInManagedApps|Логическое|Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.|
|emailInDomainSuffixes|Коллекция String|Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.|
|enterpriseAppBlockTrust|Boolean|Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.|
|enterpriseAppBlockTrustModification|Boolean|\[Нерекомендуемая\] Настройка этого параметра и установка для этого параметра значения "true" не оказывает никакого действия на устройстве.|
|есимблоккмодификатион|Логическое|Указывает, следует ли разрешить добавление или удаление планов сотовой связи на eSIM контролируемого устройства.|
|faceTimeBlocked|Логическое|Указывает, следует ли запретить использовать FaceTime. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|findMyFriendsBlocked|Логическое|Указывает, следует ли заблокировать изменения для поиска друзей, когда устройство находится в защищенном режиме.|
|gamingBlockGameCenterFriends|Логическое|Указывает, следует ли запретить пользователю добавлять друзей в Game Center. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|gamingBlockMultiplayer|Логическое|Указывает, следует ли запретить пользователю играть с несколькими игроками. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|gameCenterBlocked|Логическое|Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.|
|hostPairingBlocked|Логическое|Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.|
|iBooksStoreBlocked|Логическое|Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.|
|iBooksStoreBlockErotica|Логическое|Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".|
|iCloudBlockActivityContinuation|Логическое|Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.|
|iCloudBlockBackup|Логическое|Указывает, следует ли заблокировать резервное копирование iCloud. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|iCloudBlockDocumentSync|Логическое|Указывает, следует ли заблокировать синхронизацию документов iCloud. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|iCloudBlockManagedAppsSync|Логическое|Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.|
|iCloudBlockPhotoLibrary|Логическое|Указывает, следует ли заблокировать медиатеку iCloud.|
|iCloudBlockPhotoStreamSync|Логическое|Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.|
|iCloudBlockSharedPhotoStream|Логическое|Указывает, следует ли заблокировать общий фотопоток.|
|iCloudRequireEncryptedBackup|Логическое|Указывает, обязательно ли шифровать резервные копии iCloud.|
|iTunesBlockExplicitContent|Логическое|Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|iTunesBlockMusicService|Логическое|Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).|
|iTunesBlockRadio|Логическое|Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).|
|keyboardBlockAutoCorrect|Логическое|Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|keyboardBlockDictation|Логическое|Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.|
|keyboardBlockPredictive|Логическое|Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|keyboardBlockShortcuts|Логическое|Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|keyboardBlockSpellCheck|Логическое|Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|kioskModeAllowAssistiveSpeak|Логическое|Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.|
|kioskModeAllowAssistiveTouchSettings|Логическое|Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.|
|kioskModeAllowAutoLock|Логическое|Указывает, следует ли запретить автоблокировку устройства в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблоккаутолокк.|
|киоскмодеблоккаутолокк|Логическое|Указывает, следует ли блокировать автоматическую блокировку устройств в режиме киоска.|
|kioskModeAllowColorInversionSettings|Логическое|Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.|
|kioskModeAllowRingerSwitch|Boolean|Указывает, можно ли использовать переключатель звонка в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблоккринжерсвитч.|
|киоскмодеблоккринжерсвитч|Логическое|Указывает, следует ли запретить использование переключателя звонка в режиме киоска.|
|kioskModeAllowScreenRotation|Логическое|Указывает, следует ли запретить поворот экрана в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблоккскринротатион.|
|киоскмодеблоккскринротатион|Логическое|Указывает, следует ли блокировать поворот экрана в режиме киоска.|
|kioskModeAllowSleepButton|Логическое|Указывает, можно ли использовать кнопку "Сон" в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблоккслипбуттон.|
|kioskModeBlockSleepButton|Логическое|Указывает, следует ли запретить использование кнопки "сон" в режиме киоска.|
|kioskModeAllowTouchscreen|Логическое|Указывает, можно ли использовать сенсорный экран в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблокктаучскрин.|
|киоскмодеблокктаучскрин|Логическое|Указывает, следует ли запретить использование сенсорного экрана в режиме киоска.|
|киоскмодинаблевоицеконтрол|Логическое|Указывает, следует ли включить управление голосовым режимом в режиме киоска.|
|киоскмодеалловвоицеконтролмодификатион|Логическое|Указывает, следует ли запретить пользователю переключать управление голосовым режимом в режиме киоска.|
|kioskModeAllowVoiceOverSettings|Логическое|Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.|
|kioskModeAllowVolumeButtons|Логическое|Указывает, можно ли использовать кнопки громкости в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблоккволумебуттонс.|
|kioskModeBlockVolumeButtons|Логическое|Указывает, следует ли блокировать кнопки громкости в режиме терминала.|
|kioskModeAllowZoomSettings|Логическое|Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.|
|kioskModeAppStoreUrl|String|URL-адрес приложения в App Store для использования в режиме киоска. Используйте, если свойство KioskModeManagedAppId не известно.|
|киоскмодебуилтинаппид|String|Идентификатор встроенных приложений для использования в режиме киоска. Используется, когда KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.|
|kioskModeRequireAssistiveTouch|Логическое|Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.|
|kioskModeRequireColorInversion|Логическое|Указывает, обязательно ли использовать инверсию цвета в режиме киоска.|
|kioskModeRequireMonoAudio|Логическое|Указывает, обязательно ли использовать монозвук в режиме киоска.|
|kioskModeRequireVoiceOver|Логическое|Указывает, обязательно ли использовать VoiceOver в режиме киоска.|
|kioskModeRequireZoom|Логическое|Указывает, обязательно ли использовать масштабирование в режиме киоска.|
|kioskModeManagedAppId|String|Идентификатор управляемого приложения для использования в режиме киоска. Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.|
|lockScreenBlockControlCenter|Логическое|Указывает, следует ли запретить использовать центр управления на заблокированном экране.|
|lockScreenBlockNotificationView|Логическое|Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.|
|lockScreenBlockPassbook|Логическое|Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.|
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
|mediaContentRatingApps|[ратингаппстипе](../resources/intune-deviceconfig-ratingappstype.md)|Параметры оценки контента мультимедиа для приложений. Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.|
|messagesBlocked|Логическое|Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.|
|notificationsBlockSettingsModification|Логическое|Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).|
|passcodeBlockFingerprintUnlock|Логическое|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passcodeBlockFingerprintModification|Логическое|Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.|
|passcodeBlockModification|Логическое|Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).|
|passcodeBlockSimple|Логическое|Указывает, следует ли заблокировать простые секретные коды.|
|passcodeExpirationDays|Int32|Количество дней до окончания срока действия секретного кода. Допустимые значения: от 1 до 65 535.|
|passcodeMinimumLength|Int32|Минимальная длина секретного кода. Допустимые значения: от 4 до 14.|
|passcodeMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах) до запроса пароля.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passcodeMinimumCharacterSetCount|Int32|Количество наборов символов, которые должен содержать секретный код. Допустимые значения: от 0 до 4.|
|passcodePreviousPasscodeBlockCount|Int32|Количество предыдущих секретных кодов, которые следует блокировать. Допустимые значения: от 1 до 24.|
|passcodeSignInFailureCountBeforeWipe|Int32|Количество неудачных попыток входа до очистки устройства. Допустимые значения: от 4 до 11.|
|passcodeRequiredType|[рекуиредпассвордтипе](../resources/intune-deviceconfig-requiredpasswordtype.md)|Необходимый тип секретного кода. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Логическое|Указывает, обязательно ли использовать секретный код.|
|podcastsBlocked|Логическое|Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).|
|проксимитиблокксетуптоневдевице|Логическое|Указывает, следует ли включить запрос на установку находящихся рядом устройств с защищенным устройством.|
|safariBlockAutofill|Логическое|Указывает, следует ли запретить использовать автозаполнение в Safari. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|safariBlockJavaScript|Логическое|Указывает, следует ли заблокировать JavaScript в Safari.|
|safariBlockPopups|Логическое|Указывает, следует ли блокировать всплывающие окна в Safari.|
|safariBlocked|Boolean|Указывает, следует ли запретить использовать Safari. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Настройки файлов cookie для Safari. Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|Коллекция String|URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.|
|safariPasswordAutoFillDomains|Коллекция String|Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам. Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).|
|safariRequireFraudWarning|Логическое|Указывает, обязательно ли предупреждение о мошенничестве в Safari.|
|screenCaptureBlocked|Логическое|Указывает, следует ли запретить пользователю делать снимки экрана.|
|siriBlocked|Логическое|Указывает, следует ли запретить использовать Siri.|
|siriBlockedWhenLocked|Логическое|Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.|
|siriBlockUserGeneratedContent|Логическое|Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.|
|siriRequireProfanityFilter|Логическое|Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.|
|софтвареупдатесенфорцедделайиндайс|Int32|Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства. Допустимые значения: от 0 до 90.|
|софтвареупдатесфорцеделайед|Логическое|Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.|
|spotlightBlockInternetResults|Логическое|Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.|
|voiceDialingBlocked|Логическое|Указывает, следует ли заблокировать голосовой набор.|
|wallpaperBlockModification|Логическое|Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.|
|классрумфорцерекуестпермиссионтолеавеклассес|Логическое|Указывает, является ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса (iOS 11,3 и более поздних версий).|
|кэйчаинблоккклаудсинк|Логическое|Указывает, заблокирована ли синхронизация ключей iCloud для iCloud. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|пкиблоккотаупдатес|Логическое|Указывает, блокируются ли обновления PKI беспроводной сети. Если задать для этого ограничения значение false, проверки CRL и OCSP (iOS 7,0 и более поздних версий) не отключаются.|
|привацифорцелимитадтраккинг|Логическое|Указывает, ограничено ли отслеживание AD. (iOS 7,0 и более поздних версий).|
|ентерприсебукблоккбаккуп|Логическое|Указывает, блокируется ли резервное копирование корпоративной книги.|
|ентерприсебукблоккметадатасинк|Логическое|Указывает, блокируется ли синхронизация заметок и выделений корпоративных книг.|
|airPrintBlocked|Логическое|Указывает, заблокировано ли Аирпринт (iOS 11,0 и более поздних версий).|
|аирпринтблокккредентиалсстораже|Логическое|Указывает, заблокировано ли хранение цепочки ключей имени пользователя и пароля для Аирпринт (iOS 11,0 и более поздних версий).|
|airPrintForceTrustedTLS|Логическое|Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (iOS 11,0 и более поздних версий).|
|airPrintBlockiBeaconDiscovery|Логическое|Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт. Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (iOS 11,0 и более поздних версий).|
|филеснетворкдривеакцессблоккед|Логическое|Указывает, могут ли устройства получать доступ к файлам или другим ресурсам на сетевом сервере с помощью протокола SMB. Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.|
|филесусбдривеакцессблоккед|Логическое|Указывает, могут ли севицес с Access подключаться к файлам и открывать их на USB-диске. Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.|
|вифиповеронфорцед|Логическое|Указывает, остается ли Wi-Fi On, даже если устройство находится в режиме "в самолете". Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.|
|блокксистемаппремовал|Логическое|Указывает, заблокировано ли удаление системных приложений с устройства на контролируемом устройстве (iOS 11,0 и более поздних версий).|
|впнблокккреатион|Логическое|Указывает, блокируется ли создание конфигураций VPN (iOS 11,0 и более поздних версий).|
|аппремовалблоккед|Логическое|Указывает, разрешено ли удаление приложений.|
|усбрестриктедмодеблоккед|Логическое|Указывает, разрешена ли подключаться к стандарту USB, пока устройство заблокировано (iOS 11.4.1 и более поздних версий).|
|пассвордблоккаутофилл|Логическое|Указывает, разрешена ли функция автозаполнения паролей (iOS 12,0 и более поздних версий).|
|пассвордблоккпроксимитирекуестс|Логическое|Указывает, следует ли запретить запрашивать пароли с близлежащих устройств (iOS 12,0 и более поздних версий).|
|пассвордблоккаирдропшаринг|Логическое|Указывает, следует ли заблокировать общий доступ к паролям с помощью AirDrop паролей iOS 12,0 и более поздних версий.|
|датеандтимефорцесетаутоматикалли|Логическое|Указывает, включена ли функция даты и времени "автоматически задано" и не может быть отключена пользователем (iOS 12,0 и более поздних версий).|
|контактсалловманажедтаунманажедврите|Логическое|Указывает, могут ли управляемые приложения записывать контакты в неуправляемые учетные записи контактов (iOS 12,0 и более поздних версий).|
|контактсалловунманажедтоманажедреад|Логическое|Указывает, могут ли неуправляемые приложения читать из управляемых учетных записей контактов (iOS 12,0 или более поздней версии).|
|целлуларблоккперсоналхотспотмодификатион|Логическое|Указывает, следует ли запретить пользователю изменять параметр личных гиперобъектов (iOS 12,2 или более поздней версии).|
|континуауспаскэйбоардблоккед|Логическое|Указывает, следует ли заблокировать клавиатуру непрерывного пути, когда устройство защищено (iOS 13 или более поздней версии).|
|финдмидевицеинфиндмяппблоккед|Логическое|Указывает, следует ли заблокировать Поиск устройства, когда устройство защищено (iOS 13 или более поздней версии).|
|финдмифриендсинфиндмяппблоккед|Логическое|Указывает, следует ли заблокировать "найти друзей", когда устройство защищено (iOS 13 или более поздней версии).|
|итунесблоккед|Логическое|Указывает, следует ли заблокировать приложение iTunes. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|киоскмодеапптипе|[иоскиоскмодеапптипе](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|Тип приложения, которое будет запускаться в режиме киоска. Возможные значения: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10518

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
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
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
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
    "Email In Domain Suffixes value"
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
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
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
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10690

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
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
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
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
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
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
    "Email In Domain Suffixes value"
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
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
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
  "kioskModeAppType": "appStoreApp"
}
```



