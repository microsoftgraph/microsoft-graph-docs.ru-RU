---
title: Тип ресурса Hardwareinformation.
description: Сведения об оборудовании для данного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ad73731be7f3fd3d18798b7dc84ce7865449529
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942012"
---
# <a name="hardwareinformation-resource-type"></a>Тип ресурса Hardwareinformation.

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения об оборудовании для данного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|serialNumber|Строка|Серийный номер.|
|Тоталсторажеспаце|Int64|Общий объем хранилища устройства.|
|Фристоражеспаце|Int64|Свободное место на устройстве.|
|imei|Строка|IMEI|
|meid|String|MEID|
|manufacturer|Строка|Производитель устройства|
|model|Строка|Модель устройства|
|phoneNumber|Строка|Номер телефона устройства|
|subscriberCarrier|Строка|Абонентская перевозчик устройства|
|Целлулартечнологи|Строка|Технология сотовой связи устройства|
|Вифимак|Строка|MAC-адрес устройства Wi-Fi|
|Оператингсистемлангуаже|Строка|Язык операционной системы устройства|
|isSupervised|Логический|Контролируемый режим устройства|
|isEncrypted|Boolean|Состояние шифрования устройства|
|Свойства isshareddevice|Логический|Общие iPad|
|Шареддевицекачедусерс|Коллекция [шаредаппледевицеусер](../resources/intune-devices-sharedappledeviceuser.md)|Все пользователи на общем устройстве Apple|
|ТпмспеЦификатионверсион|Строка|Строка, указывающая версию спецификации.|
|Оператингсистемедитион|Строка|Строка, задающая выпуск операционной системы.|
|Девицефуллкуалифиеддомаиннаме|Строка|Возвращает полное доменное имя устройства (при наличии). Если устройство не присоединено к домену, возвращается пустая строка. |
|Девицегуардвиртуализатионбаседсекуритихардваререкуирементстате|[Девицегуардвиртуализатионбаседсекуритихардваререкуирементстате](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Состояние требования к оборудованию для обеспечения безопасности на основе виртуализации. Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|Девицегуардвиртуализатионбаседсекуритистате|[Девицегуардвиртуализатионбаседсекуритистате](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Состояние безопасности на основе виртуализации. . Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.|
|Девицегуардлокалсистемаусоритикредентиалгуардстате|[Девицегуардлокалсистемаусоритикредентиалгуардстате](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Состояние Credential Guard в администраторе локальной системы (LSA). . Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|

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
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
}
```




