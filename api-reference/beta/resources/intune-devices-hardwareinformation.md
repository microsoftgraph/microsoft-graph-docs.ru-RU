---
title: Тип ресурса Hardwareinformation.
description: Сведения об оборудовании для данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ad6b9c6681f8bca347e2b979570674ba64ca2e9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267392"
---
# <a name="hardwareinformation-resource-type"></a>Тип ресурса Hardwareinformation.

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения об оборудовании для данного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|serialNumber|String|Серийный номер.|
|тоталсторажеспаце|Int64|Общий объем хранилища устройства.|
|фристоражеспаце|Int64|Свободное место на устройстве.|
|imei|String|IMEI|
|meid|String|MEID|
|manufacturer|String|Производитель устройства|
|model|String|Модель устройства|
|phoneNumber|String|Номер телефона устройства|
|subscriberCarrier|String|Абонентская перевозчик устройства|
|целлулартечнологи|String|Технология сотовой связи устройства|
|вифимак|String|MAC-адрес устройства Wi-Fi|
|оператингсистемлангуаже|String|Язык операционной системы устройства|
|isSupervised|Boolean|Контролируемый режим устройства|
|isEncrypted|Boolean|Состояние шифрования устройства|
|баттерисериалнумбер|String|Серийный номер текущей батареи устройства|
|баттерихеалсперцентаже|Int32|Процент работоспособности текущего аккумулятора устройства. Допустимые значения: от 0 до 100|
|баттеричаржециклес|Int32|Количество циклов зарядки, прошедшей через текущий аккумулятор устройства. Допустимые значения — от 0 до 2147483647|
|Свойства isshareddevice|Boolean|Общие iPad|
|шареддевицекачедусерс|Коллекция [шаредаппледевицеусер](../resources/intune-devices-sharedappledeviceuser.md)|Все пользователи на общем устройстве Apple|
|тпмспеЦификатионверсион|String|Строка, указывающая версию спецификации.|
|оператингсистемедитион|String|Строка, задающая выпуск операционной системы.|
|девицефуллкуалифиеддомаиннаме|String|Возвращает полное доменное имя устройства (при наличии). Если устройство не присоединено к домену, возвращается пустая строка. |
|девицегуардвиртуализатионбаседсекуритихардваререкуирементстате|[девицегуардвиртуализатионбаседсекуритихардваререкуирементстате](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Состояние требования к оборудованию для обеспечения безопасности на основе виртуализации. Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|девицегуардвиртуализатионбаседсекуритистате|[девицегуардвиртуализатионбаседсекуритистате](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Состояние безопасности на основе виртуализации. . Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.|
|девицегуардлокалсистемаусоритикредентиалгуардстате|[девицегуардлокалсистемаусоритикредентиалгуардстате](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Состояние Credential Guard в администраторе локальной системы (LSA). . Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|
|осбуилднумбер|String|Номер сборки операционной системы на устройстве с Android|
|оператингсистемпродукттипе|Int32|Int, указывающий операционную систему Windows Продукттипе. Дополнительные сведения https://go.microsoft.com/fwlink/?linkid=2126950 . Допустимые значения — от 0 до 2147483647|
|ipAddressV4|String|IPAddressV4|
|субнетаддресс|String|субнетаддресс|

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
  "subnetAddress": "String"
}
```




