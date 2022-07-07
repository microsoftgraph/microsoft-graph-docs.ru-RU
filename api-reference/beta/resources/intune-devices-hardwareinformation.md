---
title: Тип ресурса hardwareInformation
description: Сведения об оборудовании заданного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 09dde616eee8d4740f33499baebcf784967ad93d
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670318"
---
# <a name="hardwareinformation-resource-type"></a>Тип ресурса hardwareInformation

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения об оборудовании заданного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|serialNumber|String|Серийный номер.|
|totalStorageSpace|Int64|Общее пространство хранения устройства.|
|freeStorageSpace|Int64|Свободное место в хранилище устройства.|
|imei|String|IMEI|
|meid|String|MEID|
|manufacturer|String|Производитель устройства|
|model|String|Модель устройства|
|phoneNumber|String|Номер телефона устройства|
|subscriberCarrier|String|Оператор подписчика устройства|
|cellularTechnology|String|Технология сотовой связи устройства|
|wifiMac|String|MAC-адрес Wi-Fi устройства|
|operatingSystemLanguage|String|Язык операционной системы устройства|
|isSupervised|Boolean|Защищенный режим устройства|
|isEncrypted|Boolean|Состояние шифрования устройства|
|batterySerialNumber|String|Серийный номер текущего аккумулятора устройства|
|batteryHealthPercentage|Int32|Процент работоспособности текущего аккумулятора устройства. Допустимые значения: от 0 до 100|
|batteryChargeCycles|Int32|Количество циклов заряда, за которые прошло текущее аккумуляторное устройство. Допустимые значения от 0 до 2147483647|
|isSharedDevice|Логическое|Общий iPad|
|sharedDeviceCachedUsers|[Коллекция sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)|Все пользователи на общем устройстве Apple|
|tpmSpecificationVersion|String|Строка, указывавая версию спецификации.|
|operatingSystemEdition|String|Строка, задающее выпуск ОС.|
|deviceFullQualifiedDomainName|String|Возвращает полное доменное имя устройства (если оно есть). Если устройство не присоединено к домену, оно возвращает пустую строку. |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Состояние требований к оборудованию безопасности на основе виртуализации. Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Состояние безопасности на основе виртуализации. . Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Состояние защиты учетных данных локального системного центра (LSA). . Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|
|osBuildNumber|String|Номер сборки операционной системы на устройстве Android|
|operatingSystemProductType|Int32|Значение Int, указывающее productType операционной системы Windows. Дополнительные сведения см. здесь https://go.microsoft.com/fwlink/?linkid=2126950. Допустимые значения от 0 до 2147483647|
|ipAddressV4|String|IPAddressV4|
|subnetAddress|String|SubnetAddress|
|esimIdentifier|String|Идентификатор eSIM|
|systemManagementBIOSVersion|String|Версия BIOS, сообщаемая SMBIOS|
|tpmManufacturer|String|Идентификация сведений, однозначно именующий производителя доверенного платформенного модуля|
|tpmVersion|String|Версия доверенного платформенного модуля, указанная изготовителем|
|wiredIPv4Addresses|Коллекция String|Список проводных IPv4-адресов. Частота обновления (максимальная задержка для синхронизации значения свойства с устройства в облачное хранилище) этого свойства ежедневно. Обратите внимание, что это свойство в настоящее время поддерживается только на устройствах под управлением Windows.|
|batteryLevelPercentage|Двойное с плавающей точкой|Уровень батареи в диапазоне от 0,0 до 100 или значение NULL, если не удается определить уровень батареи. Частота обновления этого свойства определяется для каждой проверки. Обратите внимание, что это свойство в настоящее время поддерживается только на устройствах под управлением iOS 5.0 и более поздних версий и доступно только при наличии права доступа к сведениям об устройстве. Допустимые значения: от 0 до 100|
|residentUsersCount|Int32|Количество пользователей, которые в настоящее время находятся на этом устройстве, или значение NULL (по умолчанию), если значение этого свойства не может быть определено. Частота обновления этого свойства определяется для каждой проверки. Обратите внимание, что это свойство в настоящее время поддерживается только на устройствах под управлением iOS 13.4 и более поздних версий и доступно только при наличии права доступа к сведениям об устройстве. Допустимые значения от 0 до 2147483647|
|productName|String|Имя продукта, например iPad8,12 и т. д. Частота обновления этого свойства — еженедельно. Обратите внимание, что это свойство в настоящее время поддерживается только на устройствах iOS или MacOS и доступно только при наличии права доступа к сведениям об устройстве.|
|deviceLicensingStatus|[deviceLicensingStatus](../resources/intune-devices-devicelicensingstatus.md)|Состояние лицензирования подписки на основе устройств. Частота обновления этого свойства ежедневно. Обратите внимание, что в настоящее время это свойство поддерживается только для лицензирования подписки на устройства на основе Windows. Если он не поддерживается, значение будет равно неизвестному (-1). Возможные значения: `licenseRefreshStarted`, `licenseRefreshPending`, `deviceIsNotAzureActiveDirectoryJoined`, `verifyingMicrosoftDeviceIdentity`, `deviceIdentityVerificationFailed`, `verifyingMirosoftAccountIdentity`, `mirosoftAccountVerificationFailed`, `acquiringDeviceLicense`, `refreshingDeviceLicense`, `deviceLicenseRefreshSucceed`, `deviceLicenseRefreshFailed`, `removingDeviceLicense`, `deviceLicenseRemoveSucceed`, `deviceLicenseRemoveFailed`, `unknownFutureValue`, `unknown`.|
|deviceLicensingLastErrorCode|Int32|Стандартный код ошибки, указывающий на последнюю ошибку, или 0, указывающий на отсутствие ошибки (по умолчанию). Частота обновления этого свойства ежедневно. Обратите внимание, что в настоящее время это свойство поддерживается только для лицензирования подписки на устройства на основе Windows. Допустимые значения от 0 до 2147483647|
|deviceLicensingLastErrorDescription|String|Текстовое сообщение об ошибке в виде декриптора для deviceLicensingLastErrorCode. Частота обновления этого свойства ежедневно. Обратите внимание, что в настоящее время это свойство поддерживается только для лицензирования подписки на устройства на основе Windows.|

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
  "tpmVersion": "String",
  "wiredIPv4Addresses": [
    "String"
  ],
  "batteryLevelPercentage": "4.2",
  "residentUsersCount": 1024,
  "productName": "String",
  "deviceLicensingStatus": "String",
  "deviceLicensingLastErrorCode": 1024,
  "deviceLicensingLastErrorDescription": "String"
}
```




