---
title: Тип ресурса Ротатебитлоккеркэйсдевицеактионресулт
description: Результат действия устройства Ротатебитлоккеркэйс
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f4196c25146ba72e0b9fec5fc67dce9d521275d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299101"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a>Тип ресурса Ротатебитлоккеркэйсдевицеактионресулт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Результат действия устройства Ротатебитлоккеркэйс


Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionName|String|Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|errorCode|Int32|Код ошибки действия Ротатебитлоккеркэйс|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rotateBitLockerKeysDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rotateBitLockerKeysDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "errorCode": 1024
}
```




