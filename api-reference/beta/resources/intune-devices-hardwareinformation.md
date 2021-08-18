---
title: Тип ресурса hardwareInformation
description: Сведения о оборудовании данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1d8a94e44663bd6070d9b6f9d50a3fed7db9e22d12dcb70bc1cf9400f5342a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54148059"
---
# <a name="hardwareinformation-resource-type"></a>Тип ресурса hardwareInformation

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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
|cellularTechnology|Строка|Клеточная технология устройства|
|wifiMac|Строка|Mac-адрес WiFi устройства|
|operatingSystemLanguage|Строка|Язык операционной системы устройства|
|isSupervised|Boolean|Контролируемый режим устройства|
|isEncrypted|Boolean|Состояние шифрования устройства|
|batterySerialNumber|Строка|Серийный номер текущего аккумулятора устройства|
|batteryHealthPercentage|Int32|Процент состояния текущего аккумулятора устройства. Допустимые значения: от 0 до 100|
|batteryChargeCycles|Int32|Количество циклов заряда текущего аккумулятора устройства прошло. Допустимые значения от 0 до 2147483647|
|isSharedDevice|Логический|Общие iPad|
|sharedDeviceCachedUsers|[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection|Все пользователи на совместном устройстве Apple|
|tpmSpecificationVersion|Строка|Строка, которая указывает версию спецификации.|
|operatingSystemEdition|Строка|Строка, заданная в выпуске ОС.|
|deviceFullQualifiedDomainName|Строка|Возвращает полностью квалифицированное доменное имя устройства (если таково). Если устройство не присоединилось к домену, оно возвращает пустую строку. |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Состояние требований к оборудованию безопасности на основе виртуализации. Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Состояние безопасности на основе виртуализации. . Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Состояние охраны учетных данных местного управления системы (LSA). . Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|
|osBuildNumber|Строка|Номер сборки операционной системы на устройстве Android|
|operatingSystemProductType|Int32|Int, который указывает Windows productType операционной системы. Дополнительные сведения здесь https://go.microsoft.com/fwlink/?linkid=2126950 . Допустимые значения от 0 до 2147483647|
|ipAddressV4|String|IPAddressV4|
|subnetAddress|Строка|SubnetAddress|
|esimIdentifier|Строка|идентификатор eSIM|
|systemManagementBIOSVersion|Строка|Версия BIOS, как сообщает SMBIOS|
|tpmManufacturer|Строка|Идентифицирующие сведения, уникальные имена производителя TPM|
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




