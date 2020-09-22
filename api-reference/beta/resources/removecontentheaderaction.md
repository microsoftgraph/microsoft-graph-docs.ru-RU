---
title: Тип ресурса Ремовеконтенсеадерактион
description: Представляет действие, задающее сведения о заголовке контента, которые необходимо удалить из информации (если это возможно).
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63dc9556ace567f4505b40c1882bd56b087a7835
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073427"
---
# <a name="removecontentheaderaction-resource-type"></a>Тип ресурса Ремовеконтенсеадерактион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о заголовке контента, которые необходимо удалить из информации (если это возможно). API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовеконтенсеадерактион** , если заголовок будет удален в результате обновления или удаления метки. Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, который содержит заданный ранее заголовок контента.

## <a name="properties"></a>Свойства

| Свойство       | Тип              | Описание                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| уиелементнамес | Коллекция String | Имя элемента пользовательского интерфейса заголовка, который требуется удалить. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentHeaderAction",
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
  "description": "removeContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

