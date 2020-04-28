---
title: Тип ресурса windows81SCEPCertificateProfile
description: Профиль сертификата SCEP для Windows 8.1 и SCEP
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 072e0b5e4e85254956087c6de8ff8f6a04786553
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467818"
---
# <a name="windows81scepcertificateprofile-resource-type"></a>Тип ресурса windows81SCEPCertificateProfile

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль сертификата SCEP для Windows 8.1 и SCEP


Наследуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows81SCEPCertificateProfiles](../api/intune-deviceconfig-windows81scepcertificateprofile-list.md)|Коллекция [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)|Список свойств и связей объектов [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .|
|[Получение windows81SCEPCertificateProfile](../api/intune-deviceconfig-windows81scepcertificateprofile-get.md)|[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)|Чтение свойств и связей объекта [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .|
|[Создание windows81SCEPCertificateProfile](../api/intune-deviceconfig-windows81scepcertificateprofile-create.md)|[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)|Создание нового объекта [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .|
|[Удаление windows81SCEPCertificateProfile](../api/intune-deviceconfig-windows81scepcertificateprofile-delete.md)|Нет|Удаляет объект [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).|
|[Обновление windows81SCEPCertificateProfile](../api/intune-deviceconfig-windows81scepcertificateprofile-update.md)|[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)|Обновление свойств объекта [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция объектов string|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|Свойства renewalthresholdpercentage|Int32|Пороговое значение возобновления сертификата. Допустимые значения — от 1 до 99, наследуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|
|keyStorageProvider|[кэйсторажепровидероптион](../resources/intune-deviceconfig-keystorageprovideroption.md)|Поставщик хранилища ключей (KSP), наследуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md). Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|subjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Формат имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md). Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|Тип альтернативного имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md). Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|certificateValidityPeriodValue|Int32|Значение срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Масштаб срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md). Возможные значения: `days`, `months`, `years`.|
|екстендедкэйусажес|Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)|Параметры расширенного использования ключа (EKU). Эта коллекция может содержать не более 500 элементов. Наследуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)|
|customSubjectAlternativeNames|Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)|Настраиваемые параметры альтернативного имени субъекта. Эта коллекция может содержать не более 500 элементов. Наследуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)|
|сцепсерверурлс|Коллекция объектов string|URL-адреса сервера SCEP.|
|Свойства subjectnameformatstring|String|Настраиваемый формат для использования с SubjectNameFormat = Custom. Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US|
|кэйусаже|[кэйусажес](../resources/intune-deviceconfig-keyusages.md)|Использование ключа SCEP. Возможные значения: `keyEncipherment`, `digitalSignature`.|
|keySize|[keySize](../resources/intune-deviceconfig-keysize.md)|Размер ключа SCEP. Возможные значения: `size1024`, `size2048`.|
|хашалгорисм|[хашалгорисмс](../resources/intune-deviceconfig-hashalgorithms.md)|Алгоритм хеширования SCEP. Возможные значения: `sha1`, `sha2`.|
|subjectAlternativeNameFormatString|String|Настраиваемая строка, определяющая атрибут AAD.|
|certificateStore|[certificateStore](../resources/intune-deviceconfig-certificatestore.md)|Сертификат целевого хранилища. Возможные значения: `user`, `machine`.|

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
|рутцертификате|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Доверенный корневой сертификат|
|Manageddevicecertificatestates к объекту|Коллекция [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Состояние сертификата для устройств|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows81SCEPCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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
  "keyStorageProvider": "String",
  "subjectNameFormat": "String",
  "subjectAlternativeNameType": "String",
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ],
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "String",
      "name": "String"
    }
  ],
  "scepServerUrls": [
    "String"
  ],
  "subjectNameFormatString": "String",
  "keyUsage": "String",
  "keySize": "String",
  "hashAlgorithm": "String",
  "subjectAlternativeNameFormatString": "String",
  "certificateStore": "String"
}
```



