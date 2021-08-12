---
title: тип ресурса educationWordResource
description: Подкласс educationResource.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 00ce0d3a31c62bc38c6a5f9893c69b51a58c3a32741e993691e234a753278385
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192532"
---
# <a name="educationwordresource-resource-type"></a>тип ресурса educationWordResource

Пространство имен: microsoft.graph

Подкласс [educationResource](educationresource.md). 

Это ресурс документа Word. Файл Word должен быть загружен в **каталог fileResource,** связанный с назначением или отправкой.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fileUrl|String|Расположение файла на диске.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


