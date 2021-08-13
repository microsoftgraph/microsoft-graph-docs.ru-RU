---
title: тип ресурса printMargin
description: Указывает ширину поля, используемую при печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d15b488985bbf1c51f03a0c030fab16fdf3d25cbd8c8b53b29368e4f0af2d151
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196567"
---
# <a name="printmargin-resource-type"></a>тип ресурса printMargin

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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

