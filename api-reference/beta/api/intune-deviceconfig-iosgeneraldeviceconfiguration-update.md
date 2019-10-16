---
title: Обновление объекта iosGeneralDeviceConfiguration
description: Обновление свойств объекта iosGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 72f0312cf219a28dc06747cc095a52b65b1caeea
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533814"
---
# <a name="update-iosgeneraldeviceconfiguration"></a>Обновление объекта iosGeneralDeviceConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).

## <a name="prerequisites"></a>Необходимые компоненты
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в формате JSON.

В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).

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
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
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
|appsVisibilityListType|[апплисттипе](../resources/intune-deviceconfig-applisttype.md)|Тип списка, определенного свойством AppsVisibilityList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Логический|Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|appStoreBlocked|Boolean|Указывает, следует ли запретить использовать App Store. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|appStoreBlockInAppPurchases|Логический|Указывает, следует ли запретить пользователю совершать покупки из приложения.|
|appStoreBlockUIAppInstallation|Логический|Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения. Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).|
|appStoreRequirePassword|Логический|Указывает, требуется ли пароль, когда вы используете приложение App Store.|
|аутофиллфорцеаусентикатион|Логический|Указывает, следует ли принудительно выполнять проверку подлинности пользователей перед автозаполнением паролей и сведений о кредитных картах в Safari и других приложениях на контролируемых устройствах.|
|bluetoothBlockModification|Логический|Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).|
|cameraBlocked|Логический|Указывает, следует ли запретить доступ к камере устройства. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|cellularBlockDataRoaming|Логический|Указывает, следует ли блокировать передачу данных в роуминге.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Логический|Указывает, следует ли заблокировать получение фоновых данных в роуминге.|
|cellularBlockPerAppDataModification|Логический|Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.|
|cellularBlockPersonalHotspot|Логический|Указывает, следует ли заблокировать личный хот-спот.|
|целлуларблоккпланмодификатион|Логический|Указывает, следует ли запретить пользователям изменять параметры плана сотовой связи на защищенном устройстве.|
|cellularBlockVoiceRoaming|Логический|Указывает, следует ли заблокировать голосовой роуминг.|
|certificatesBlockUntrustedTlsCertificates|Логический|Указывает, следует ли заблокировать ненадежные сертификаты TLS.|
|classroomAppBlockRemoteScreenObservation|Логический|Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).|
|classroomAppForceUnpromptedScreenObservation|Логический|Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.|
|классрумфорцеаутоматикаллижоинклассес|Логический|Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося, когда устройство находится в защищенном режиме.|
|классрумфорцеунпромптедаппанддевицелокк|Логический|Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся. Только в защищенном режиме.|
|compliantAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType). Эта коллекция может содержать не более 10 000 элементов.|
|compliantAppListType|[апплисттипе](../resources/intune-deviceconfig-applisttype.md)|Список, указанный с помощью свойства AppComplianceList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
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
|enterpriseAppBlockTrustModification|Boolean|Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.|
|есимблоккмодификатион|Логический|Указывает, следует ли разрешить добавление или удаление планов сотовой связи на eSIM контролируемого устройства.|
|faceTimeBlocked|Логический|Указывает, следует ли запретить использовать FaceTime. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|findMyFriendsBlocked|Логический|Указывает, следует ли заблокировать изменения для поиска друзей, когда устройство находится в защищенном режиме.|
|gamingBlockGameCenterFriends|Логический|Указывает, следует ли запретить пользователю добавлять друзей в Game Center. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|gamingBlockMultiplayer|Логический|Указывает, следует ли запретить пользователю играть с несколькими игроками. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|gameCenterBlocked|Логический|Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.|
|hostPairingBlocked|Логический|Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.|
|iBooksStoreBlocked|Логический|Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.|
|iBooksStoreBlockErotica|Логический|Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".|
|iCloudBlockActivityContinuation|Логический|Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.|
|iCloudBlockBackup|Логический|Указывает, следует ли заблокировать резервное копирование iCloud. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|iCloudBlockDocumentSync|Логический|Указывает, следует ли заблокировать синхронизацию документов iCloud. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|iCloudBlockManagedAppsSync|Логический|Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.|
|iCloudBlockPhotoLibrary|Логический|Указывает, следует ли заблокировать медиатеку iCloud.|
|iCloudBlockPhotoStreamSync|Логический|Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.|
|iCloudBlockSharedPhotoStream|Логический|Указывает, следует ли заблокировать общий фотопоток.|
|iCloudRequireEncryptedBackup|Логический|Указывает, обязательно ли шифровать резервные копии iCloud.|
|iTunesBlockExplicitContent|Логический|Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|iTunesBlockMusicService|Логический|Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).|
|iTunesBlockRadio|Логический|Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).|
|keyboardBlockAutoCorrect|Логический|Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|keyboardBlockDictation|Логический|Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.|
|keyboardBlockPredictive|Логический|Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|keyboardBlockShortcuts|Логический|Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).|
|keyboardBlockSpellCheck|Логический|Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).|
|kioskModeAllowAssistiveSpeak|Логический|Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.|
|kioskModeAllowAssistiveTouchSettings|Логический|Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.|
|kioskModeAllowAutoLock|Логический|Указывает, следует ли запретить автоблокировку устройства в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблоккаутолокк.|
|киоскмодеблоккаутолокк|Логический|Указывает, следует ли блокировать автоматическую блокировку устройств в режиме киоска.|
|kioskModeAllowColorInversionSettings|Логический|Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.|
|kioskModeAllowRingerSwitch|Boolean|Указывает, можно ли использовать переключатель звонка в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблоккринжерсвитч.|
|киоскмодеблоккринжерсвитч|Логический|Указывает, следует ли запретить использование переключателя звонка в режиме киоска.|
|kioskModeAllowScreenRotation|Логический|Указывает, следует ли запретить поворот экрана в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблоккскринротатион.|
|киоскмодеблоккскринротатион|Логический|Указывает, следует ли блокировать поворот экрана в режиме киоска.|
|kioskModeAllowSleepButton|Логический|Указывает, можно ли использовать кнопку "Сон" в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблоккслипбуттон.|
|kioskModeBlockSleepButton|Логический|Указывает, следует ли запретить использование кнопки "сон" в режиме киоска.|
|kioskModeAllowTouchscreen|Логический|Указывает, можно ли использовать сенсорный экран в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблокктаучскрин.|
|киоскмодеблокктаучскрин|Логический|Указывает, следует ли запретить использование сенсорного экрана в режиме киоска.|
|киоскмодинаблевоицеконтрол|Логический|Указывает, следует ли включить управление голосовым режимом в режиме киоска.|
|киоскмодеалловвоицеконтролмодификатион|Логический|Указывает, следует ли запретить пользователю переключать управление голосовым режимом в режиме киоска.|
|kioskModeAllowVoiceOverSettings|Логический|Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.|
|kioskModeAllowVolumeButtons|Логический|Указывает, можно ли использовать кнопки громкости в режиме киоска. Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей. Вместо этого используйте Киоскмодеблоккволумебуттонс.|
|kioskModeBlockVolumeButtons|Логический|Указывает, следует ли блокировать кнопки громкости в режиме терминала.|
|kioskModeAllowZoomSettings|Логический|Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.|
|kioskModeAppStoreUrl|String|URL-адрес приложения в App Store для использования в режиме киоска. Используйте, если свойство KioskModeManagedAppId не известно.|
|киоскмодебуилтинаппид|String|Идентификатор встроенных приложений для использования в режиме киоска. Используется, когда KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.|
|kioskModeRequireAssistiveTouch|Логический|Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.|
|kioskModeRequireColorInversion|Логический|Указывает, обязательно ли использовать инверсию цвета в режиме киоска.|
|kioskModeRequireMonoAudio|Логический|Указывает, обязательно ли использовать монозвук в режиме киоска.|
|kioskModeRequireVoiceOver|Логический|Указывает, обязательно ли использовать VoiceOver в режиме киоска.|
|kioskModeRequireZoom|Логический|Указывает, обязательно ли использовать масштабирование в режиме киоска.|
|kioskModeManagedAppId|String|Идентификатор управляемого приложения для использования в режиме киоска. Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.|
|lockScreenBlockControlCenter|Логический|Указывает, следует ли запретить использовать центр управления на заблокированном экране.|
|lockScreenBlockNotificationView|Логический|Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.|
|lockScreenBlockPassbook|Логический|Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.|
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
|messagesBlocked|Логический|Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.|
|notificationsBlockSettingsModification|Логический|Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).|
|passcodeBlockFingerprintUnlock|Логический|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passcodeBlockFingerprintModification|Логический|Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.|
|passcodeBlockModification|Логический|Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).|
|passcodeBlockSimple|Логический|Указывает, следует ли заблокировать простые секретные коды.|
|passcodeExpirationDays|Int32|Количество дней до окончания срока действия секретного кода. Допустимые значения: от 1 до 65 535.|
|passcodeMinimumLength|Int32|Минимальная длина секретного кода. Допустимые значения: от 4 до 14.|
|passcodeMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах) до запроса пароля.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passcodeMinimumCharacterSetCount|Int32|Количество наборов символов, которые должен содержать секретный код. Допустимые значения: от 0 до 4.|
|passcodePreviousPasscodeBlockCount|Int32|Количество предыдущих секретных кодов, которые следует блокировать. Допустимые значения: от 1 до 24.|
|passcodeSignInFailureCountBeforeWipe|Int32|Количество неудачных попыток входа до очистки устройства. Допустимые значения: от 4 до 11.|
|passcodeRequiredType|[рекуиредпассвордтипе](../resources/intune-deviceconfig-requiredpasswordtype.md)|Необходимый тип секретного кода. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Логический|Указывает, обязательно ли использовать секретный код.|
|podcastsBlocked|Логический|Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).|
|проксимитиблокксетуптоневдевице|Логический|Указывает, следует ли включить запрос на установку находящихся рядом устройств с защищенным устройством.|
|safariBlockAutofill|Логический|Указывает, следует ли запретить использовать автозаполнение в Safari. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|safariBlockJavaScript|Логический|Указывает, следует ли заблокировать JavaScript в Safari.|
|safariBlockPopups|Логический|Указывает, следует ли блокировать всплывающие окна в Safari.|
|safariBlocked|Boolean|Указывает, следует ли запретить использовать Safari. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Настройки файлов cookie для Safari. Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|Коллекция String|URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.|
|safariPasswordAutoFillDomains|Коллекция String|Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам. Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).|
|safariRequireFraudWarning|Логический|Указывает, обязательно ли предупреждение о мошенничестве в Safari.|
|screenCaptureBlocked|Логический|Указывает, следует ли запретить пользователю делать снимки экрана.|
|siriBlocked|Логический|Указывает, следует ли запретить использовать Siri.|
|siriBlockedWhenLocked|Логический|Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.|
|siriBlockUserGeneratedContent|Логический|Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.|
|siriRequireProfanityFilter|Логический|Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.|
|софтвареупдатесенфорцедделайиндайс|Int32|Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства. Допустимые значения: от 0 до 90.|
|софтвареупдатесфорцеделайед|Логический|Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.|
|spotlightBlockInternetResults|Логический|Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.|
|voiceDialingBlocked|Логический|Указывает, следует ли заблокировать голосовой набор.|
|wallpaperBlockModification|Логический|Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.|
|классрумфорцерекуестпермиссионтолеавеклассес|Логический|Указывает, является ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса (iOS 11,3 и более поздних версий).|
|кэйчаинблоккклаудсинк|Логический|Указывает, заблокирована ли синхронизация ключей iCloud для iCloud. Для iOS 13 и более поздних версий требуется контролируемое устройство.|
|пкиблоккотаупдатес|Логический|Указывает, блокируются ли обновления PKI беспроводной сети. Если задать для этого ограничения значение false, проверки CRL и OCSP (iOS 7,0 и более поздних версий) не отключаются.|
|привацифорцелимитадтраккинг|Логический|Указывает, ограничено ли отслеживание AD. (iOS 7,0 и более поздних версий).|
|ентерприсебукблоккбаккуп|Логический|Указывает, блокируется ли резервное копирование корпоративной книги.|
|ентерприсебукблоккметадатасинк|Логический|Указывает, блокируется ли синхронизация заметок и выделений корпоративных книг.|
|airPrintBlocked|Логический|Указывает, заблокировано ли Аирпринт (iOS 11,0 и более поздних версий).|
|аирпринтблокккредентиалсстораже|Логический|Указывает, заблокировано ли хранение цепочки ключей имени пользователя и пароля для Аирпринт (iOS 11,0 и более поздних версий).|
|airPrintForceTrustedTLS|Логический|Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (iOS 11,0 и более поздних версий).|
|airPrintBlockiBeaconDiscovery|Логический|Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт. Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (iOS 11,0 и более поздних версий).|
|филеснетворкдривеакцессблоккед|Логический|Указывает, могут ли устройства получать доступ к файлам или другим ресурсам на сетевом сервере с помощью протокола SMB. Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.|
|филесусбдривеакцессблоккед|Логический|Указывает, могут ли севицес с Access подключаться к файлам и открывать их на USB-диске. Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.|
|вифиповеронфорцед|Логический|Указывает, остается ли Wi-Fi On, даже если устройство находится в режиме "в самолете". Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.|
|блокксистемаппремовал|Логический|Указывает, заблокировано ли удаление системных приложений с устройства на контролируемом устройстве (iOS 11,0 и более поздних версий).|
|впнблокккреатион|Логический|Указывает, блокируется ли создание конфигураций VPN (iOS 11,0 и более поздних версий).|
|аппремовалблоккед|Логический|Указывает, разрешено ли удаление приложений.|
|усбрестриктедмодеблоккед|Логический|Указывает, разрешена ли подключаться к стандарту USB, пока устройство заблокировано (iOS 11.4.1 и более поздних версий).|
|пассвордблоккаутофилл|Логический|Указывает, разрешена ли функция автозаполнения паролей (iOS 12,0 и более поздних версий).|
|пассвордблоккпроксимитирекуестс|Логический|Указывает, следует ли запретить запрашивать пароли с близлежащих устройств (iOS 12,0 и более поздних версий).|
|пассвордблоккаирдропшаринг|Логический|Указывает, следует ли заблокировать общий доступ к паролям с помощью AirDrop паролей iOS 12,0 и более поздних версий.|
|датеандтимефорцесетаутоматикалли|Логический|Указывает, включена ли функция даты и времени "автоматически задано" и не может быть отключена пользователем (iOS 12,0 и более поздних версий).|
|контактсалловманажедтаунманажедврите|Логический|Указывает, могут ли управляемые приложения записывать контакты в неуправляемые учетные записи контактов (iOS 12,0 и более поздних версий).|
|контактсалловунманажедтоманажедреад|Логический|Указывает, могут ли неуправляемые приложения читать из управляемых учетных записей контактов (iOS 12,0 или более поздней версии).|
|целлуларблоккперсоналхотспотмодификатион|Логический|Указывает, следует ли запретить пользователю изменять параметр личных гиперобъектов (iOS 12,2 или более поздней версии).|
|сиридисаблесерверлоггинг|Логический|Указывает, отключено ли ведение журнала Siri на стороне сервера (iOS 12,2 или более поздней версии).|
|континуауспаскэйбоардблоккед|Логический|Указывает, следует ли заблокировать клавиатуру непрерывного пути, когда устройство защищено (iOS 13 или более поздней версии).|
|финдмидевицеинфиндмяппблоккед|Логический|Указывает, следует ли заблокировать Поиск устройства, когда устройство защищено (iOS 13 или более поздней версии).|
|финдмифриендсинфиндмяппблоккед|Логический|Указывает, следует ли заблокировать "найти друзей", когда устройство защищено (iOS 13 или более поздней версии).|
|итунесблоккед|Логический|Указывает, следует ли заблокировать приложение iTunes. Для iOS 13 и более поздних версий требуется контролируемое устройство.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 10517

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
  "siriDisableServerLogging": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10689

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
  "siriDisableServerLogging": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true
}
```






