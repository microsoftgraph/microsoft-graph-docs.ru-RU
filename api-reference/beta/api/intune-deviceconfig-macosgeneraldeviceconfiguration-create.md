---
title: Create macOSGeneralDeviceConfiguration
description: Создание объекта macOSGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 773e694fe3d4ce03fc599d9d7992aba1cdcda548
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448776"
---
# <a name="create-macosgeneraldeviceconfiguration"></a>Create macOSGeneralDeviceConfiguration

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).

## <a name="prerequisites"></a>Необходимые разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

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
В тексте запроса добавьте представление объекта macOSGeneralDeviceConfiguration в формате JSON.

В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта macOSGeneralDeviceConfiguration.

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
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|compliantAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType). Эта коллекция может содержать не более 10 000 элементов.|
|compliantAppListType|[апплисттипе](../resources/intune-deviceconfig-applisttype.md)|Список, включенный в CompliantAppsList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|emailInDomainSuffixes|Коллекция String|Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.|
|passwordBlockSimple|Boolean|Блокировка простых паролей.|
|passwordExpirationDays|Int32|Количество дней до окончания срока действия пароля.|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые должен содержать пароль. Допустимые значения: от 0 до 4.|
|passwordMinimumLength|Int32|Минимальная длина паролей.|
|passwordMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Период бездействия (в минутах), по истечении которого будет гаснуть экран.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, которые требуется блокировать.|
|passwordRequiredType|[рекуиредпассвордтипе](../resources/intune-deviceconfig-requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordRequired|Логический|Определяет, нужно ли запрашивать ввод пароля.|
|кэйчаинблоккклаудсинк|Логический|Указывает, заблокирована ли синхронизация ключей iCloud для iCloud (macOS 10,12 и более поздних версий).|
|airPrintBlocked|Логический|Указывает, заблокировано ли Аирпринт (macOS 10,12 и более поздних версий).|
|airPrintForceTrustedTLS|Логический|Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (macOS 10,13 и более поздних версий).|
|airPrintBlockiBeaconDiscovery|Логический|Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт. Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (macOS 10,3 и более поздних версий).|
|safariBlockAutofill|Логический|Указывает, следует ли запретить использовать автозаполнение в Safari.|
|cameraBlocked|Логический|Указывает, следует ли запретить доступ к камере устройства.|
|iTunesBlockMusicService|Логический|Указывает, следует ли заблокировать музыкальную службу и вернуть приложение "Музыка" в классический режим.|
|spotlightBlockInternetResults|Boolean|Указывает, следует ли запретить получение результатов из поиска в Интернете.|
|keyboardBlockDictation|Логический|Указывает, следует ли запретить пользователю использовать диктовку.|
|definitionLookupBlocked|Логический|Указывает, следует ли заблокировать Поиск определений.|
|апплеватчблоккаутаунлокк|Логический|Указывает, следует ли запретить пользователям разблокирование своего Mac-адреса с контрольной записью Apple.|
|итунесблоккфилешаринг|Логический|Указывает, следует ли запретить передачу файлов с помощью iTunes.|
|iCloudBlockDocumentSync|Логический|Указывает, следует ли заблокировать синхронизацию документов iCloud.|
|иклаудблоккмаил|Логический|Указывает, следует ли запретить синхронизацию почты для iCloud.|
|иклаудблоккаддрессбук|Логический|Указывает, следует ли запретить синхронизацию контактов с iCloud.|
|иклаудблокккалендар|Логический|Указывает, следует ли запретить синхронизацию календарей в iCloud.|
|иклаудблоккреминдерс|Логический|Указывает, следует ли запретить синхронизацию напоминаний для iCloud.|
|иклаудблоккбукмаркс|Логический|Указывает, следует ли блокировать синхронизацию закладок в iCloud.|
|иклаудблоккнотес|Логический|Указывает, следует ли запретить синхронизацию заметок в iCloud.|
|airDropBlocked|Логический|Указывает, следует ли запретить AirDrop.|
|пассвордблоккмодификатион|Логический|Указывает, следует ли запретить изменение секретного кода.|
|passwordBlockFingerprintUnlock|Логический|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|пассвордблоккаутофилл|Логический|Указывает, следует ли заблокировать функцию автозаполнения паролей.|
|пассвордблоккпроксимитирекуестс|Логический|Указывает, следует ли запретить запрашивать пароли с ближайших устройств.|
|пассвордблоккаирдропшаринг|Логический|Указывает, следует ли заблокировать общий доступ к паролям с помощью функции паролей AirDrop.|
|софтвареупдатесенфорцедделайиндайс|Int32|Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства. Допустимые значения: от 0 до 90.|
|софтвареупдатесфорцеделайед|Логический|Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.|
|контенткачингблоккед|Логический|Указывает, следует ли запретить кэширование контента.|
|iCloudBlockPhotoLibrary|Логический|Указывает, следует ли заблокировать медиатеку iCloud.|
|screenCaptureBlocked|Boolean|Указывает, следует ли запретить пользователю делать снимки экрана.|
|classroomAppBlockRemoteScreenObservation|Логический|Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "аудитория". Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.|
|classroomAppForceUnpromptedScreenObservation|Логический|Указывает, следует ли автоматически предоставлять разрешение преподавателю управляемого курса в приложении аудитории для просмотра экрана учащегося без выдачи запросов. Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.|
|классрумфорцеаутоматикаллижоинклассес|Логический|Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося. Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.|
|классрумфорцерекуестпермиссионтолеавеклассес|Логический|Указывает, должен ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса. Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.|
|классрумфорцеунпромптедаппанддевицелокк|Логический|Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся. Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.|
|iCloudBlockActivityContinuation|Boolean|Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве MacOS, на другом устройстве iOS или MacOS (MacOS 10,15 или более поздней версии).|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3146

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3318

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
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
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true
}
```





