---
title: Тип ресурса androidForWorkScepCertificateProfile
description: Профиль сертификата SCEP для работы с Android
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b36b671027b36cd51b98478846184ec11a0ef10a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33948557"
---
# <a name="androidforworkscepcertificateprofile-resource-type"></a>Тип ресурса androidForWorkScepCertificateProfile

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль сертификата SCEP для работы с Android


Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроидфорворксцепцертификатепрофилес](../api/intune-deviceconfig-androidforworkscepcertificateprofile-list.md)|Коллекция [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)|Список свойств и связей объектов [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .|
|[Получение androidForWorkScepCertificateProfile](../api/intune-deviceconfig-androidforworkscepcertificateprofile-get.md)|[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)|Чтение свойств и связей объекта [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .|
|[Создание androidForWorkScepCertificateProfile](../api/intune-deviceconfig-androidforworkscepcertificateprofile-create.md)|[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)|Создание нового объекта [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .|
|[Удаление androidForWorkScepCertificateProfile](../api/intune-deviceconfig-androidforworkscepcertificateprofile-delete.md)|Нет|Удаляет объект [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).|
|[Обновление androidForWorkScepCertificateProfile](../api/intune-deviceconfig-androidforworkscepcertificateprofile-update.md)|[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)|Обновление свойств объекта [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Свойства renewalthresholdpercentage|Int32|Пороговое значение возобновления сертификата. Допустимые значения — от 1 до 99, наследуемые от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)|
|subjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Формат имени субъекта сертификата. Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md). Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|certificateValidityPeriodValue|Int32|Значение срока действия сертификата. Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Масштаб срока действия сертификата. Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md). Возможные значения: `days`, `months`, `years`.|
|Екстендедкэйусажес|Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)|Параметры расширенного использования ключа (EKU). Эта коллекция может содержать не более 500 элементов. Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|Тип альтернативного имени субъекта сертификата. Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md). Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|Сцепсерверурлс|Коллекция строк|URL-адреса сервера SCEP|
|Свойства subjectnameformatstring|Строка|Настраиваемый формат для использования с SubjectNameFormat = Custom. Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US|
|Кэйусаже|[Кэйусажес](../resources/intune-deviceconfig-keyusages.md)|Использование ключа SCEP. Возможные значения: `keyEncipherment`, `digitalSignature`.|
|keySize|[keySize](../resources/intune-deviceconfig-keysize.md)|Размер ключа SCEP. Возможные значения: `size1024`, `size2048`.|
|Хашалгорисм|[Хашалгорисмс](../resources/intune-deviceconfig-hashalgorithms.md)|Алгоритм хеширования SCEP. Возможные значения: `sha1`, `sha2`.|
|subjectAlternativeNameFormatString|Строка|Настраиваемая строка, определяющая атрибут AAD.|
|certificateStore|[certificateStore](../resources/intune-deviceconfig-certificatestore.md)|Сертификат целевого хранилища. Возможные значения: `user`, `machine`.|
|customSubjectAlternativeNames|Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)|Настраиваемые параметры альтернативного имени субъекта. Эта коллекция может содержать не более 500 элементов.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Рутцертификате|[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)|Доверенный корневой сертификат. Наследуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)|
|Manageddevicecertificatestates к объекту|Коллекция [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Состояние сертификата для устройств|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkScepCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
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
  "scepServerUrls": [
    "String"
  ],
  "subjectNameFormatString": "String",
  "keyUsage": "String",
  "keySize": "String",
  "hashAlgorithm": "String",
  "subjectAlternativeNameFormatString": "String",
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




