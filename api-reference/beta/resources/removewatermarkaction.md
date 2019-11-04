---
title: Тип ресурса Ремовеватермаркактион
description: Представляет действие, задающее сведения о подложке контента, которая будет удалена из информации, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 34859dedd5e5e740aa776cdf78bb742399523fa2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939273"
---
# <a name="removewatermarkaction-resource-type"></a>Тип ресурса Ремовеватермаркактион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о подложке контента, которая будет удалена из информации, если это возможно. API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовеватермаркактион** , если водяной знак необходимо удалить в результате обновления или удаления метки. Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, который содержит Подводя содержимого, который использовался ранее.

## <a name="properties"></a>Свойства

| Свойство       | Тип              | Описание                           |
| :------------- | :---------------- | :------------------------------------ |
| уиелементнамес | Коллекция строк | Имя удаляемого элемента пользовательского интерфейса нижнего колонтитула. |

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