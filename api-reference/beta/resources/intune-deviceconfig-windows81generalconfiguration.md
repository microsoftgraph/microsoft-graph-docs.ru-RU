---
title: Тип ресурса windows81GeneralConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windows81GeneralConfiguration.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ed40025a392b66b8bff0421259a111139315771
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59145983"
---
# <a name="windows81generalconfiguration-resource-type"></a>Тип ресурса windows81GeneralConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windows81GeneralConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-list.md)|Коллекция [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|Перечисление свойств и связей объектов [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).|
|[Получение объекта windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-get.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|Чтение свойств и связей объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).|
|[Создание объекта windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-create.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|Создание объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).|
|[Удаление объекта windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-delete.md)|Нет|Удаление объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).|
|[Обновление объекта windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-update.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|Обновление свойств объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция объектов string|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.|
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
|cellularBlockDataRoaming|Boolean|Указывает, следует ли блокировать передачу данных в роуминге.|
|diagnosticsBlockDataSubmission|Boolean|Указывает, следует ли заблокировать отправку диагностических данных.|
|passwordBlockPicturePasswordAndPin|Boolean|Указывает, следует ли запретить использование графического пароля и ПИН-кода.|
|passwordExpirationDays|Int32|Срок действия пароля (в днях).|
|passwordMinimumLength|Int32|Минимальная длина пароля.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые требуются для пароля.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, повторное использование которых следует запретить. Допустимые значения: от 0 до 24.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек.|
|storageRequireDeviceEncryption|Boolean|Указывает, обязательно ли шифрование данных на мобильном устройстве.|
|minimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|Минимальная классификация обновлений, устанавливаемая автоматически. Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.|
|updatesMinimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|Минимальная классификация обновлений, устанавливаемая автоматически. Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.|
|updatesRequireAutomaticUpdates|Boolean|Указывает, обязательно ли автоматическое обновление.|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|Настройки контроля учетных записей. Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.|
|workFoldersUrl|String|URL-адрес рабочей папки.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows81GeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
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
  "browserEnterpriseModeSiteListLocation": "String",
  "browserInternetSecurityLevel": "String",
  "browserIntranetSecurityLevel": "String",
  "browserLoggingReportLocation": "String",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "String",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "String",
  "updatesMinimumAutoInstallClassification": "String",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "String",
  "workFoldersUrl": "String"
}
```



