---
title: тип ресурса educationExternalResource
description: Подкласс educationResource. Это служба назначений типа ресурсов по умолчанию для картографии всех ресурсов, которые мы не выставим на график. Это позволяет всем звонителям SDK работать без проблем.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3bfefee10d387a34c783c3f8afec7ee00480a506
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220800"
---
# <a name="educationexternalresource-resource-type"></a>тип ресурса educationExternalResource

Пространство имен: microsoft.graph

Представляет общий тип для картографии ресурсов, не открытых в Microsoft Graph.

Наследует [от educationResource](educationresource.md).

Этот сложный тип позволяет всем звонителям SDK работать без проблем.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|webUrl|String|Расположение ресурса. Обязательная|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.educationExternalResource"
}-->

```json
{
  "webUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-09-21 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExternalResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
