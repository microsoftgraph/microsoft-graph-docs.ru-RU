---
title: Тип ресурса aospDeviceOwnerPkcsCertificateProfile
description: Профиль сертификата PKCS владельца устройства AOSP
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fef9518d136af0bb0ced39e84abbbb7804da5e24
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669142"
---
# <a name="aospdeviceownerpkcscertificateprofile-resource-type"></a>Тип ресурса aospDeviceOwnerPkcsCertificateProfile

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль сертификата PKCS владельца устройства AOSP


Наследует от [aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление aospDeviceOwnerPkcsCertificateProfiles](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-list.md)|[Коллекция aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)|Список свойств и связей объектов [aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) .|
|[Получение aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-get.md)|[aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)|Чтение свойств и связей объекта [aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) .|
|[Создание aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-create.md)|[aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)|Создайте объект [aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) .|
|[Удаление aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-delete.md)|Нет|Удаляет [aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md).|
|[Обновление aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-update.md)|[aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)|Обновление свойств объекта [aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) .|

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
|renewalThresholdPercentage|Int32|Пороговое значение продления сертификата в процентах. Допустимые значения от 1 до 99, унаследованные от [aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md)|
|subjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Формат имени субъекта сертификата. Эта коллекция может содержать не более 500 элементов. Наследуется от [aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md). Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|certificateValidityPeriodValue|Int32|Значение срока действия сертификата. Наследуется от [aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md)|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|Масштабирование для срока действия сертификата. Наследуется от [aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md). Возможные значения: `days`, `months`, `years`.|
|extendedKeyUsages|[Коллекция extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)|Параметры расширенного использования ключа (EKU). Эта коллекция может содержать не более 500 элементов. Наследуется от [aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md)|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune-shared-subjectalternativenametype.md)|Альтернативный тип имени субъекта сертификата. Эта коллекция может содержать не более 500 элементов. Наследуется от [aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md). Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.|
|certificationAuthority|String|Центр сертификации PKCS|
|certificationAuthorityName|String|Имя центра сертификации PKCS|
|certificationAuthorityType|[deviceManagementCertificationAuthority](../resources/intune-deviceconfig-devicemanagementcertificationauthority.md)|Тип центра сертификации. Возможные значения: `notConfigured`, `microsoft`, `digiCert`.|
|certificateTemplateName|String|Имя шаблона сертификата PKCS|
|subjectAlternativeNameFormatString|String|Настраиваемая строка, определяющее атрибут AAD.|
|subjectNameFormatString|String|Пользовательский формат для использования с SubjectNameFormat = Custom. Пример: CN={{EmailAddress}},E={{EmailAddress}},OU=Корпоративные пользователи,O=Contoso Corporation,L=Redmond,ST=WA,C=US|
|certificateStore|[certificateStore](../resources/intune-shared-certificatestore.md)|Сертификат целевого хранилища. Возможные значения: `user`, `machine`.|
|customSubjectAlternativeNames|[Коллекция customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)|Настраиваемые параметры альтернативного имени субъекта. Эта коллекция может содержать не более 500 элементов.|

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
|rootCertificate|[aospDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-aospdeviceownertrustedrootcertificate.md)|Доверенный корневой сертификат. Наследуется от [aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md)|
|managedDeviceCertificateStates|[Коллекция managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Состояние сертификата для устройств. Эта коллекция может содержать не более 2147483647 элементов.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aospDeviceOwnerPkcsCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerPkcsCertificateProfile",
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
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ],
  "subjectAlternativeNameType": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificationAuthorityType": "String",
  "certificateTemplateName": "String",
  "subjectAlternativeNameFormatString": "String",
  "subjectNameFormatString": "String",
  "certificateStore": "String",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "String",
      "name": "String"
    }
  ]
}
```




