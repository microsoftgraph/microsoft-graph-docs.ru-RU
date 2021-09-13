---
title: Создание macOSEndpointProtectionConfiguration
description: Создание нового объекта macOSEndpointProtectionConfiguration.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 98fda3953f99731700e74ce37da9efaf9d854a32
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59138885"
---
# <a name="create-macosendpointprotectionconfiguration"></a>Создание macOSEndpointProtectionConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
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
В теле запроса устройте представление JSON для объекта macOSEndpointProtectionConfiguration.

В следующей таблице показаны свойства, необходимые при создании macOSEndpointProtectionConfiguration.

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
|gatekeeperBlockOverride|Логический|Если задана истина, переопределения пользователя для Gatekeeper будут отключены.|
|firewallEnabled|Логическое|Следует ли включить брандмауэр или нет.|
|брандмауэрBlockAllIncoming|Логическое|Соответствует параметру "Блокировка всех входящих подключений".|
|firewallEnableStealthMode|Логический|Соответствует режиму "Включить режим стелс".|
|брандмауэрАпплиляции|[коллекция macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)|Список приложений с настройками брандмауэра. Параметры брандмауэра для приложений, не входящего в этот список, определяются пользователем. Эта коллекция может содержать не более 500 элементов.|
|fileVaultEnabled|Логическое|Следует ли включить FileVault или нет.|
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



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2786

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
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
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "enabled",
  "advancedThreatProtectionCloudDelivered": "enabled",
  "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
  "advancedThreatProtectionDiagnosticDataCollection": "enabled",
  "advancedThreatProtectionExcludedFolders": [
    "Advanced Threat Protection Excluded Folders value"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "Advanced Threat Protection Excluded Files value"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "Advanced Threat Protection Excluded Extensions value"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "Advanced Threat Protection Excluded Processes value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2958

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
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
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "enabled",
  "advancedThreatProtectionCloudDelivered": "enabled",
  "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
  "advancedThreatProtectionDiagnosticDataCollection": "enabled",
  "advancedThreatProtectionExcludedFolders": [
    "Advanced Threat Protection Excluded Folders value"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "Advanced Threat Protection Excluded Files value"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "Advanced Threat Protection Excluded Extensions value"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "Advanced Threat Protection Excluded Processes value"
  ]
}
```



