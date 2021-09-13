---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7ca5217159ef39d2a1914e2be2067e8e570177f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098792"
---
# <a name="deviceactionresult-resource-type"></a>Тип ресурса deviceActionResult

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Результат действия, касающегося устройства

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionName|String|Название действия|
|actionState|[actionState](../resources/intune-devices-actionstate.md)|Состояние действия. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Время начала действия|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления состояния действия|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




