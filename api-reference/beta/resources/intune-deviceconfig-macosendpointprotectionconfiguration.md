---
title: Тип ресурса macOSEndpointProtectionConfiguration
description: Профиль конфигурации защиты конечных точек MacOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 213a4173104e159330cce48a8fffefd107b8546c
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666986"
---
# <a name="macosendpointprotectionconfiguration-resource-type"></a>Тип ресурса macOSEndpointProtectionConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль конфигурации защиты конечных точек MacOS.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-list.md)|[Коллекция macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Список свойств и связей объектов [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|
|[Получение объекта macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-get.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md);|Чтение свойств и связей объекта [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|
|[Создание объекта macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-create.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md);|Создайте объект [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|
|[Удаление объекта macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-delete.md)|Нет|Удаляет объект [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).|
|[Обновление объекта macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-update.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md);|Обновление свойств объекта [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|

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
|gatekeeperAllowedAppSource|[macOSGatekeeperAppSources](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|Параметр "Система и конфиденциальность", который определяет, из каких расположений скачивания приложения можно запускать на устройстве macOS. Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.|
|gatekeeperBlockOverride|Логическое|Если задано значение true, переопределение пользователя для Gatekeeper будет отключено.|
|firewallEnabled|Логическое|Следует ли включить брандмауэр.|
|firewallBlockAllIncoming|Логическое|Соответствует параметру "Блокировать все входящие подключения".|
|FirewallEnableStealthMode|Логическое|Соответствует параметру "Включить скрытый режим".|
|firewallApplications|[Коллекция macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)|Список приложений с параметрами брандмауэра. Параметры брандмауэра для приложений, не включаемые в этот список, определяются пользователем. Эта коллекция может содержать не более 500 элементов.|
|fileVaultEnabled|Логическое|Указывает, следует ли включить FileVault.|
|FileVaultSelectedRecoveryKeyTypes|[macOSFileVaultRecoveryKeyTypes](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|Требуется, если fileVault включен, определяет типы ключа восстановления для использования. . Возможные значения: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.|
|fileVaultInstitutionalRecoveryKeyCertificate|Binary|Обязательный, если выбранные типы ключей восстановления включают Вмеализированный ключ восстановления. Файл сертификата в кодировке DER, используемый для задания неустроимого ключа восстановления.|
|fileVaultInstitutionalRecoveryKeyCertificateFileName|String|Имя файла сертификата ключа восстановления, который будет отображаться в пользовательском интерфейсе. (*.der).|
|fileVaultPersonalRecoveryKeyHelpMessage|String|Обязательный, если выбранные типы ключей восстановления включают PersonalRecoveryKey. Пользователю отображается короткое сообщение, в котором объясняется, как получить личный ключ восстановления.|
|fileVaultAllowDeferralUntilSignOut|Boolean|Необязательное свойство. Если задано значение true, пользователь может отложить включение FileVault, пока не выйдите из системы.|
|fileVaultNumberOfTimesUserCanIgnore|Int32|Необязательный. При использовании параметра Defer это максимальное число раз, когда пользователь может игнорировать запросы на включение FileVault, прежде чем для входа пользователя потребуется FileVault. Если задано значение -1, всегда будет предложено включить FileVault до включения FileVault, хотя это позволит пользователю обойти включение FileVault. Установка значения 0 отключит эту функцию.|
|FileVaultDisablePromptAtSignOut|Boolean|Необязательное свойство. При использовании параметра "Отложить", если задано значение true, пользователю не предлагается включить FileVault при выходе из системы.|
|fileVaultPersonalRecoveryKeyRotationInMonths|Int32|Необязательный. Если выбранные типы ключей восстановления включают PersonalRecoveryKey, частота смены ключа в месяцах.|
|FileVaultHidePersonalRecoveryKey|Boolean|Необязательное свойство. Скрытый личный ключ восстановления не отображается на экране пользователя во время шифрования FileVault, что снижает риск того, что он будет находиться в неправильных руках.|
|advancedThreatProtectionRealTime|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, следует ли включить защиту в режиме реального времени для Расширенной защиты от угроз в Microsoft Defender в macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionCloudDelivered|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, следует ли включить облачную защиту для Advanced Threat Protection в Microsoft Defender в macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionAutomaticSampleSubmission|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, следует ли включить автоматическую отправку примеров файлов для Расширенной защиты от угроз в Microsoft Defender в macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionDiagnosticDataCollection|[Включения](../resources/intune-deviceconfig-enablement.md)|Определяет, следует ли включить сбор диагностических данных и данных об использовании для Расширенной защиты от угроз в Microsoft Defender в macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionExcludedFolders|Коллекция строк|Список путей к папкам, исключаемых из антивирусной проверки для Advanced Threat Protection в Microsoft Defender в macOS.|
|advancedThreatProtectionExcludedFiles|Коллекция объектов string|Список путей к файлам, исключаемых из антивирусной проверки для Advanced Threat Protection в Microsoft Defender в macOS.|
|advancedThreatProtectionExcludedExtensions|Коллекция объектов string|Список расширений файлов, которые необходимо исключить из антивирусной проверки для Расширенной защиты от угроз в Microsoft Defender в macOS.|
|advancedThreatProtectionExcludedProcesses|Коллекция String|Список имен процессов, исключаемых из антивирусной проверки для Расширенной защиты от угроз в Microsoft Defender в macOS.|

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
  "@odata.type": "microsoft.graph.macOSEndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
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
  "gatekeeperAllowedAppSource": "String",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "String",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "String",
  "fileVaultInstitutionalRecoveryKeyCertificate": "binary",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "String",
  "fileVaultPersonalRecoveryKeyHelpMessage": "String",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 1024,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 1024,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "String",
  "advancedThreatProtectionCloudDelivered": "String",
  "advancedThreatProtectionAutomaticSampleSubmission": "String",
  "advancedThreatProtectionDiagnosticDataCollection": "String",
  "advancedThreatProtectionExcludedFolders": [
    "String"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "String"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "String"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "String"
  ]
}
```




