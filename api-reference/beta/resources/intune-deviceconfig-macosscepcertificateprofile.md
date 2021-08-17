---
title: тип ресурса macOSScepCertificateProfile
description: Профиль сертификата SCEP ОС Mac OS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cfb6300b8f787e4157ede1c0d2bc4b649867838b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58248125"
---
# <a name="macosscepcertificateprofile-resource-type"></a>тип ресурса macOSScepCertificateProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль сертификата SCEP ОС Mac OS.


Наследует [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список macOSScepCertificateProfiles](../api/intune-deviceconfig-macosscepcertificateprofile-list.md)|[коллекция macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)|Список свойств и связей [объектов macOSScepCertificateProfile.](../resources/intune-deviceconfig-macosscepcertificateprofile.md)|
|[Get macOSScepCertificateProfile](../api/intune-deviceconfig-macosscepcertificateprofile-get.md)|[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)|Чтение свойств и связей [объекта macOSScepCertificateProfile.](../resources/intune-deviceconfig-macosscepcertificateprofile.md)|
|[Создание macOSScepCertificateProfile](../api/intune-deviceconfig-macosscepcertificateprofile-create.md)|[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)|Создайте [новый объект macOSScepCertificateProfile.](../resources/intune-deviceconfig-macosscepcertificateprofile.md)|
|[Удаление macOSScepCertificateProfile](../api/intune-deviceconfig-macosscepcertificateprofile-delete.md)|Нет|Удаляет [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).|
|[Обновление macOSScepCertificateProfile](../api/intune-deviceconfig-macosscepcertificateprofile-update.md)|[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)|Обновление свойств объекта [macOSScepCertificateProfile.](../resources/intune-deviceconfig-macosscepcertificateprofile.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логический|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|renewalThresholdPercentage|Int32|Процент порогового значения обновления сертификата. Унаследованный от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|
|subjectNameFormat|[appleSubjectNameFormat](../resources/intune-deviceconfig-applesubjectnameformat.md)|Формат имени субъекта сертификата. Наследуется [от macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md). Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune-shared-subjectalternativenametype.md)|Тип альтернативного имени субъекта сертификата. Наследуется [от macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md). Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.|
|certificateValidityPeriodValue|Int32|Значение для срока действия сертификата. Унаследованный от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|Масштаб для срока действия сертификата. Наследуется [от macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md). Возможные значения: `days`, `months`, `years`.|
|scepServerUrls|Коллекция String|URL-адрес сервера SCEP Server (s).|
|subjectNameFormatString|String|Настраиваемый формат для использования с SubjectNameFormat = Custom. Пример: CN={{EmailAddress},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US|
|keyUsage|[keyUsages](../resources/intune-shared-keyusages.md)|Использование ключей SCEP. Возможные значения: `keyEncipherment`, `digitalSignature`.|
|keySize|[keySize](../resources/intune-shared-keysize.md)|Размер ключа SCEP. Возможные значения: `size1024`, `size2048`, `size4096`.|
|hashAlgorithm|[hashAlgorithms](../resources/intune-shared-hashalgorithms.md)|Алгоритм хаширования SCEP. Возможные значения: `sha1`, `sha2`.|
|extendedKeyUsages|[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)|Параметры расширенного использования ключей (EKU). Эта коллекция может содержать не более 500 элементов.|
|subjectAlternativeNameFormatString|String|Настраиваемая строка, определяемая атрибутом AAD.|
|certificateStore|[certificateStore](../resources/intune-shared-certificatestore.md)|Сертификат целевого магазина. Возможные значения: `user`, `machine`.|
|customSubjectAlternativeNames|[коллекция customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)|Настраиваемые альтернативные имена субъектов Параметры. Эта коллекция может содержать не более 500 элементов.|
|allowAllAppsAccess|Логический|Параметр AllowAllAppsAccess|

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
|rootCertificate|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Надежный корневой сертификат.|
|managedDeviceCertificateStates|[коллекция managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Состояние сертификата для устройств|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSScepCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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
  "renewalThresholdPercentage": 1024,
  "subjectNameFormat": "String",
  "subjectAlternativeNameType": "String",
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "scepServerUrls": [
    "String"
  ],
  "subjectNameFormatString": "String",
  "keyUsage": "String",
  "keySize": "String",
  "hashAlgorithm": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ],
  "subjectAlternativeNameFormatString": "String",
  "certificateStore": "String",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "String",
      "name": "String"
    }
  ],
  "allowAllAppsAccess": true
}
```




