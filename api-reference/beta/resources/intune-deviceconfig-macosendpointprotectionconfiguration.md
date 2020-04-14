---
title: Тип ресурса Макосендпоинтпротектионконфигуратион
description: Профиль конфигурации Endpoint Protection MacOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bebe34f85974bfe67d89ed372f70aded53deac5a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402132"
---
# <a name="macosendpointprotectionconfiguration-resource-type"></a>Тип ресурса Макосендпоинтпротектионконфигуратион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль конфигурации Endpoint Protection MacOS.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Макосендпоинтпротектионконфигуратионс](../api/intune-deviceconfig-macosendpointprotectionconfiguration-list.md)|Коллекция [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Список свойств и связей объектов [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|
|[Получение Макосендпоинтпротектионконфигуратион](../api/intune-deviceconfig-macosendpointprotectionconfiguration-get.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md);|Чтение свойств и связей объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|
|[Создание Макосендпоинтпротектионконфигуратион](../api/intune-deviceconfig-macosendpointprotectionconfiguration-create.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md);|Создание нового объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|
|[Удаление Макосендпоинтпротектионконфигуратион](../api/intune-deviceconfig-macosendpointprotectionconfiguration-delete.md)|Нет|Удаляет объект [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).|
|[Обновление Макосендпоинтпротектионконфигуратион](../api/intune-deviceconfig-macosendpointprotectionconfiguration-update.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md);|Обновление свойств объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|

## <a name="properties"></a>Свойства
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
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|гатекипералловедаппсаурце|[макосгатекипераппсаурцес](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS. Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.|
|гатекиперблокковерриде|Логическое|Если задано значение true, переопределение пользователя для привратника будет отключено.|
|firewallEnabled|Логическое|Указывает, следует ли включить брандмауэр.|
|firewallBlockAllIncoming|Логическое|Соответствует параметру "блокировать все входящие подключения".|
|firewallEnableStealthMode|Логическое|Соответствует параметру "включить скрытый режим".|
|фиреваллаппликатионс|Коллекция [макосфиреваллаппликатион](../resources/intune-deviceconfig-macosfirewallapplication.md)|Список приложений с параметрами брандмауэра. Параметры брандмауэра для приложений, не включенных в этот список, определяются пользователем. Эта коллекция может содержать не более 500 элементов.|
|филеваултенаблед|Логическое|Указывает, следует ли включить Филеваулт.|
|филеваултселектедрековерикэйтипес|[macOSFileVaultRecoveryKeyTypes](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|Обязательно если включен Филеваулт, определяет типы ключа восстановления, которые необходимо использовать. . Возможные значения: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.|
|филеваултинститутионалрековерикэйцертификате|Binary|Обязательно, если выбранные типы ключей восстановления включают Институтионалрековерикэй. Файл сертификата в кодировке DER, который использовался для установки ключа восстановления в учреждений.|
|филеваултинститутионалрековерикэйцертификатефиленаме|String|Имя файла сертификата ключа восстановления для сотрудников, который будет отображаться в пользовательском интерфейсе. (*. der).|
|филеваултперсоналрековерикэйхелпмессаже|String|Обязательно, если выбранные типы ключей восстановления включают Персоналрековерикэй. Короткое сообщение, в котором показано, как получить свой ключ восстановления личных настроек.|
|филеваулталловдеферралунтилсигнаут|Boolean|Необязательно. Если задано значение true, пользователь может отложить включение Филеваулт, пока не выйдете из системы.|
|филеваултнумберофтимесусерканигноре|Int32|Необязательный. При использовании параметра "отложить" это максимальное число раз, когда пользователь может игнорировать приглашения на включение Филеваулт, чтобы пользователь мог выполнить вход. Если задано значение-1, всегда будет выдаваться запрос на включение Филеваулт, пока Филеваулт не будет включен, хотя разрешить пользователю обходить включение Филеваулт. Если задать для этого параметра значение 0, эта функция будет отключена.|
|филеваултдисаблепромптатсигнаут|Boolean|Необязательно. При использовании параметра отсрочки, если задано значение true, пользователю не предлагается включить Филеваулт при входе.|
|филеваултперсоналрековерикэйротатионинмонсс|Int32|Необязательный. Если выбранные типы ключей восстановления включают Персоналрековерикэй, частота вращения этого ключа в месяцах.|
|филеваулсидеперсоналрековерикэй|Boolean|Необязательно. Скрытый персональный ключ восстановления не отображается на экране пользователя во время шифрования Филеваулт, что снижает риск его завершения в неправильной руки.|
|адванцедсреатпротектионреалтиме|[Включение](../resources/intune-shared-enablement.md)|Определяет, следует ли включить защиту в режиме реального времени для функции Advanced Threat Protection для защитника Майкрософт в macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|адванцедсреатпротектионклаудделиверед|[Включение](../resources/intune-shared-enablement.md)|Определяет, следует ли включить защиту от облачной защиты для Advanced Threat Protection в защитнике Майкрософт для macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|адванцедсреатпротектионаутоматиксамплесубмиссион|[Включение](../resources/intune-shared-enablement.md)|Определяет, следует ли включать автоматическую отправку образца файлов для Advanced Threat Protection в защитнике Майкрософт в macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|адванцедсреатпротектиондиагностикдатаколлектион|[Включение](../resources/intune-shared-enablement.md)|Определяет, следует ли включить сбор данных диагностики и использования для Advanced Threat Protection для защитника Майкрософт в macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|адванцедсреатпротектионексклудедфолдерс|Коллекция String|Список путей к папкам, которые необходимо исключить из антивирусной проверки для Advanced Threat protection защитника Майкрософт в macOS.|
|адванцедсреатпротектионексклудедфилес|Коллекция String|Список путей к файлам, которые необходимо исключить из антивирусной проверки для Advanced Threat Protection в macOS.|
|адванцедсреатпротектионексклудедекстенсионс|Коллекция String|Список расширений файлов, которые необходимо исключить из антивирусного сканирования для Advanced Threat Protection в macOS.|
|адванцедсреатпротектионексклудедпроцессес|Коллекция String|Список имен процессов, которые необходимо исключить из антивирусной проверки для Advanced Threat Protection в macOS.|

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



