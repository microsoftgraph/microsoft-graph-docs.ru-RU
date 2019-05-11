---
title: Тип ресурса Андроидфорворкимпортедпфксцертификатепрофиле
description: Профиль импорта PFX-сертификата для Android для работы с Android
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e79238e1ee4546cbb8e4c5b9601b970bcb1e812d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33948606"
---
# <a name="androidforworkimportedpfxcertificateprofile-resource-type"></a>Тип ресурса Андроидфорворкимпортедпфксцертификатепрофиле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль импорта PFX-сертификата для Android для работы с Android


Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроидфорворкимпортедпфксцертификатепрофилес](../api/intune-deviceconfig-androidforworkimportedpfxcertificateprofile-list.md)|Коллекция [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)|Список свойств и связей объектов [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .|
|[Получение Андроидфорворкимпортедпфксцертификатепрофиле](../api/intune-deviceconfig-androidforworkimportedpfxcertificateprofile-get.md)|[androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)|Чтение свойств и связей объекта [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .|
|[Создание Андроидфорворкимпортедпфксцертификатепрофиле](../api/intune-deviceconfig-androidforworkimportedpfxcertificateprofile-create.md)|[androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)|Создание нового объекта [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .|
|[Удаление Андроидфорворкимпортедпфксцертификатепрофиле](../api/intune-deviceconfig-androidforworkimportedpfxcertificateprofile-delete.md)|Нет|Удаляет объект [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).|
|[Обновление Андроидфорворкимпортедпфксцертификатепрофиле](../api/intune-deviceconfig-androidforworkimportedpfxcertificateprofile-update.md)|[androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)|Обновление свойств объекта [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Свойства renewalthresholdpercentage|Int32|Пороговое значение возобновления сертификата. Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|
|subjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Формат имени субъекта сертификата. Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md). Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|Тип альтернативного имени субъекта сертификата. Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md). Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|certificateValidityPeriodValue|Int32|Значение срока действия сертификата. Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Масштаб срока действия сертификата. Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md). Возможные значения: `days`, `months`, `years`.|
|Екстендедкэйусажес|Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)|Параметры расширенного использования ключа (EKU). Эта коллекция может содержать не более 500 элементов. Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|
|intendedPurpose|[intendedPurpose](../resources/intune-deviceconfig-intendedpurpose.md)|Еще не задокументировано. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|

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
|Рутцертификате|[Андроидтрустедрутцертификате](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)|Доверенный корневой сертификат. Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|
|Manageddevicecertificatestates к объекту|Коллекция [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Состояние сертификата для устройств|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkImportedPFXCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
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
  "intendedPurpose": "String"
}
```




