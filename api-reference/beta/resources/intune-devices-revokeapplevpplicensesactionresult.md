---
title: Тип ресурса Ревокеапплевпплиценсесактионресулт
description: Отзыв результатов действий для лицензий Apple VPP
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 09843bbce769594e2729421121b7a936dcd19c4a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724504"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a>Тип ресурса Ревокеапплевпплиценсесактионресулт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Отзыв результатов действий для лицензий Apple VPP


Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionName|String|Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).|
|тоталлиценсескаунт|Int32|Общее количество связанных лицензий Apple VPP|
|фаиледлиценсескаунт|Int32|Общее количество лицензий Apple VPP, которые не удалось отозвать|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```





