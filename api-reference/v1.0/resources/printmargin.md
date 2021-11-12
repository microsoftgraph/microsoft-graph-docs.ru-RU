---
title: тип ресурса printMargin
description: Указывает ширину поля, используемую при печати.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 20ad208efdac2890a45dfbebdcf51ace8e49d061
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60924210"
---
# <a name="printmargin-resource-type"></a>тип ресурса printMargin

Пространство имен: microsoft.graph

Указывает ширину поля, используемую при печати.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|top|Int32|Маржа в микронах от верхнего края.|
|bottom|Int32|Маржа в микронах с нижнего края.|
|Правильно|Int32|Поле в микронах с правого края.|
|left|Int32|Поле в микронах с левого края.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printMargin"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printMargin",
  "top": "Integer",
  "bottom": "Integer",
  "right": "Integer",
  "left": "Integer"
}
```

