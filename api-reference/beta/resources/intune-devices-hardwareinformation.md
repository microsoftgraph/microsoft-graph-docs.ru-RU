---
title: Тип ресурса hardwareInformation
description: Сведения о оборудовании данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e17df5baad3df0237218f314cdb1c5ee99f03c6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868178"
---
# <a name="hardwareinformation-resource-type"></a>Тип ресурса hardwareInformation

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о оборудовании данного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|serialNumber|String|Серийный номер.|
|totalStorageSpace|Int64|Общее пространство хранилища устройства.|
|freeStorageSpace|Int64|Свободное пространство для хранения устройства.|
|imei|String|IMEI|
|meid|String|MEID|
|manufacturer|String|Производитель устройства|
|model|String|Модель устройства|
|phoneNumber|String|Номер телефона устройства|
|subscriberCarrier|String|Оператор абонента устройства|
|cellularTechnology|String|Клеточная технология устройства|
|wifiMac|String|Mac-адрес WiFi устройства|
|operatingSystemLanguage|String|Язык операционной системы устройства|
|isSupervised|Boolean|Контролируемый режим устройства|
|isEncrypted|Boolean|Состояние шифрования устройства|
|batterySerialNumber|String|Серийный номер текущего аккумулятора устройства|
|batteryHealthPercentage|Int32|Процент состояния текущего аккумулятора устройства. Допустимые значения: от 0 до 100|
|batteryChargeCycles|Int32|Количество циклов заряда текущего аккумулятора устройства прошло. Допустимые значения от 0 до 2147483647|
|isSharedDevice|Логический|Общий iPad|
|sharedDeviceCachedUsers|[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection|Все пользователи на совместном устройстве Apple|
|tpmSpecificationVersion|String|Строка, которая указывает версию спецификации.|
|operatingSystemEdition|String|Строка, заданная в выпуске ОС.|
|deviceFullQualifiedDomainName|String|Возвращает полностью квалифицированное доменное имя устройства (если таково). Если устройство не присоединилось к домену, оно возвращает пустую строку. |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Состояние требований к оборудованию безопасности на основе виртуализации. Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Состояние безопасности на основе виртуализации. . Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Состояние охраны учетных данных местного управления системы (LSA). . Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|
|osBuildNumber|String|Номер сборки операционной системы на устройстве Android|
|operatingSystemProductType|Int32|Int, который указывает продукт Операционной системы Windows. Дополнительные сведения здесь https://go.microsoft.com/fwlink/?linkid=2126950 . Допустимые значения от 0 до 2147483647|
|ipAddressV4|String|IPAddressV4|
|subnetAddress|String|SubnetAddress|
|esimIdentifier|String|идентификатор eSIM|
|systemManagementBIOSVersion|String|Версия BIOS, как сообщает SMBIOS|
|tpmManufacturer|String|Идентифицирующие сведения, уникальные имена производителя TPM|
|tpmVersion|String|Версия TPM, указанная производителем|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "batterySerialNumber": "String",
  "batteryHealthPercentage": 1024,
  "batteryChargeCycles": 1024,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
  "osBuildNumber": "String",
  "operatingSystemProductType": 1024,
  "ipAddressV4": "String",
  "subnetAddress": "String",
  "esimIdentifier": "String",
  "systemManagementBIOSVersion": "String",
  "tpmManufacturer": "String",
  "tpmVersion": "String"
}
```




