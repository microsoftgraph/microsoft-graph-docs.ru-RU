---
title: Update windows81GeneralConfiguration
description: Обновление свойств объекта windows81GeneralConfiguration.
ms.openlocfilehash: 1469d204349694f453eb7571d90aa7a1ab427387
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080231"
---
# <a name="update-windows81generalconfiguration"></a>Update windows81GeneralConfiguration

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Обновление свойств объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в формате JSON.

В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия. Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью. Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|описание|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|accountsBlockAddingNonMicrosoftAccountEmail|Логический|Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.|
|applyOnlyToWindows81|Boolean|Указывает, применяется ли эта политика только к Windows 8.1. Это свойство доступно только для чтения.|
|browserBlockAutofill|Boolean|Указывает, следует ли заблокировать автозаполнение.|
|browserBlockAutomaticDetectionOfIntranetSites|Boolean|Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.|
|browserBlockEnterpriseModeAccess|Boolean|Указывает, следует ли заблокировать доступ к корпоративному режиму.|
|browserBlockJavaScript|Boolean|Указывает, следует ли запретить использование JavaScript.|
|browserBlockPlugins|Boolean|Указывает, следует ли заблокировать подключаемые модули.|
|browserBlockPopups|Boolean|Указывает, следует ли блокировать всплывающие окна.|
|browserBlockSendingDoNotTrackHeader|Boolean|Указывает, следует ли запретить пользователю отправлять заголовок DNT.|
|browserBlockSingleWordEntryOnIntranetSites|Boolean|Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.|
|browserRequireSmartScreen|Boolean|Указывает, обязательно ли использовать фильтр Smart Screen.|
|browserEnterpriseModeSiteListLocation|String|Расположение списка сайтов, запускаемых в корпоративном режиме. Это может быть локальный файл, локальная сеть или HTTP-адрес.|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|Уровень интернет-безопасности. Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|Уровень безопасности интрасети. Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|browserLoggingReportLocation|String|Расположение хранения отчетов.|
|browserRequireHighSecurityForRestrictedSites|Boolean|Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.|
|browserRequireFirewall|Boolean|Указывает, обязательно ли использовать брандмауэр.|
|browserRequireFraudWarning|Boolean|Указывает, обязательно ли предупреждение о мошенничестве.|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|Уровень безопасности надежных сайтов. Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|cellularBlockDataRoaming|Логический|Указывает, следует ли блокировать передачу данных в роуминге.|
|diagnosticsBlockDataSubmission|Boolean|Указывает, следует ли блокировать отправку диагностических данных.|
|passwordBlockPicturePasswordAndPin|Boolean|Указывает, следует ли запретить использование графического пароля и ПИН-кода.|
|passwordExpirationDays|Int32|Срок действия пароля (в днях).|
|passwordMinimumLength|Int32|Минимальная длина пароля.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые требуются для пароля.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, повторное использование которых следует запретить. Допустимые значения: от 0 до 24|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек.|
|storageRequireDeviceEncryption|Boolean|Указывает, обязательно ли шифрование данных на мобильном устройстве.|
|minimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|Как минимум обновление классификации для автоматической установки. Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.|
|updatesMinimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|Как минимум обновление классификации для автоматической установки. Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.|
|updatesRequireAutomaticUpdates|Boolean|Указывает, обязательно ли автоматическое обновление.|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|Настройки контроля учетных записей. Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.|
|workFoldersUrl|String|URL-адрес рабочей папки.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в тексте ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1920

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2096

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```





