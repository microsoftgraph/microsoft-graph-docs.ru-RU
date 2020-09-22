---
title: Тип ресурса Ремовеватермаркактион
description: Представляет действие, задающее сведения о подложке контента, которая будет удалена из информации, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0b75a001e7673bbeb1513eaac82555d228d712f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023963"
---
# <a name="removewatermarkaction-resource-type"></a>Тип ресурса Ремовеватермаркактион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о подложке контента, которая будет удалена из информации, если это возможно. API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовеватермаркактион** , если водяной знак необходимо удалить в результате обновления или удаления метки. Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, который содержит Подводя содержимого, который использовался ранее.

## <a name="properties"></a>Свойства

| Свойство       | Тип              | Описание                           |
| :------------- | :---------------- | :------------------------------------ |
| уиелементнамес | Коллекция String | Имя удаляемого элемента пользовательского интерфейса нижнего колонтитула. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeWatermarkAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "uiElementNames": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "removeWatermarkAction resource",
  "keywords": "",  
  "section": "documentation",
  "tocPath": ""
}-->

