---
title: тип ресурса macOSEndpointProtectionConfiguration
description: Профиль конфигурации защиты конечной точки MacOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c5ad98d6f208b8e676e335046cc5a66da967de08
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054543"
---
# <a name="macosendpointprotectionconfiguration-resource-type"></a>тип ресурса macOSEndpointProtectionConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль конфигурации защиты конечной точки MacOS.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список macOSEndpointProtectionConfigurations](../api/intune-deviceconfig-macosendpointprotectionconfiguration-list.md)|[коллекция macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Список свойств и связей объектов [macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|
|[Получить macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-get.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Чтение свойств и связей [объекта macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|
|[Создание macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-create.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Создание нового [объекта macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|
|[Удаление macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-delete.md)|Нет|Удаляет [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).|
|[Обновление macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-update.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Обновление свойств объекта [macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|

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
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|gatekeeperAllowedAppSource|[macOSGatekeeperAppSources](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|Параметр System и Privacy, который определяет, какие приложения для скачивания можно запускать на macOS-устройстве. Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.|
|gatekeeperBlockOverride|Логическое|Если задана истина, переопределения пользователя для Gatekeeper будут отключены.|
|firewallEnabled|Логическое|Следует ли включить брандмауэр или нет.|
|брандмауэрBlockAllIncoming|Логический|Соответствует параметру "Блокировка всех входящих подключений".|
|firewallEnableStealthMode|Логическое|Соответствует режиму "Включить режим стелс".|
|брандмауэрАпплиляции|[коллекция macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)|Список приложений с настройками брандмауэра. Параметры брандмауэра для приложений, не входящего в этот список, определяются пользователем. Эта коллекция может содержать не более 500 элементов.|
|fileVaultEnabled|Логический|Следует ли включить FileVault или нет.|
|fileVaultSelectedRecoveryKeyTypes|[macOSFileVaultRecoveryKeyTypes](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|Требуется, если включен FileVault, определяет тип(ы) ключа восстановления для использования. . Возможные значения: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.|
|fileVaultInstitutionalRecoveryKeyCertificate|В двоичном формате|Необходимый, если выбранный тип ключа восстановления (s) включает InstitutionalRecoveryKey. Кодированный файл сертификата DER, используемый для задавания институционального ключа восстановления.|
|fileVaultInstitutionalRecoveryKeyCertificateFileName|String|Имя файла сертификата ключа восстановления, отображаемого в пользовательском интерфейсе. (*.der).|
|fileVaultPersonalRecoveryKeyHelpMessage|String|Необходимый, если выбранный тип ключа восстановления (s) включает PersonalRecoveryKey. Короткое сообщение, отображаемая пользователю, которое объясняет, как он может получить свой личный ключ восстановления.|
|fileVaultAllowDeferralUntilSignOut|Boolean|Необязательный параметр. Если установлена истина, пользователь может отложить включение FileVault до тех пор, пока они не выпишутся.|
|fileVaultNumberOfTimesUserCanIgnore|Int32|Необязательный. При использовании параметра Defer это максимальное количество раз, когда пользователь может игнорировать подсказки, чтобы включить FileVault, прежде чем fileVault потребуется для пользователя, чтобы войти. Если установлено до -1, всегда будет предложено включить FileVault до включения FileVault, хотя это позволит пользователю обойти включение FileVault. Настройка этого параметра до 0 отключит функцию.|
|fileVaultDisablePromptAtSignOut|Boolean|Необязательный параметр. При использовании параметра Defer, если задается true, пользователю не предложено включить FileVault при входе.|
|fileVaultPersonalRecoveryKeyRotationInMonths|Int32|Необязательный. Если выбранный тип ключа восстановления (s) включает PersonalRecoveryKey, частота вращения этого ключа в месяцах.|
|fileVaultHidePersonalRecoveryKey|Boolean|Необязательный параметр. Скрытый личный ключ восстановления не появляется на экране пользователя во время шифрования FileVault, что снижает риск его оказаться в неправильных руках.|
|advancedThreatProtectionRealTime|[включить](../resources/intune-shared-enablement.md)|Определяет, следует ли включить защиту в режиме реального времени для microsoft Defender Advanced Threat Protection на macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionCloudDelivered|[включить](../resources/intune-shared-enablement.md)|Определяет, следует ли включить облачную защиту для microsoft Defender Advanced Threat Protection на macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionAutomaticSampleSubmission|[включить](../resources/intune-shared-enablement.md)|Определяет, следует ли включить автоматическую отправку образца файла для microsoft Defender Advanced Threat Protection на macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionDiagnosticDataCollection|[включить](../resources/intune-shared-enablement.md)|Определяет, следует ли включить сбор данных диагностики и использования для microsoft Defender Advanced Threat Protection на macOS. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionExcludedFolders|Коллекция объектов string|Список путей к папкам, исключающих антивирусное сканирование для microsoft Defender Advanced Threat Protection на macOS.|
|advancedThreatProtectionExcludedFiles|Коллекция объектов string|Список путей к файлам, которые необходимо исключить из антивирусного сканирования для microsoft Defender Advanced Threat Protection на macOS.|
|advancedThreatProtectionExcludedExtensions|Коллекция объектов string|Список расширений файлов, которые необходимо исключить из антивирусного сканирования для Microsoft Defender Advanced Threat Protection на macOS.|
|advancedThreatProtectionExcludedProcesses|Коллекция объектов string|Список имен процессов, которые необходимо исключить из антивирусного сканирования для microsoft Defender Advanced Threat Protection на macOS.|

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



