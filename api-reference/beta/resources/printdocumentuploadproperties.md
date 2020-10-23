---
author: nilakhan
description: Представляет сведения для отправки документа на печать
title: Тип ресурса Принтдокументуплоадпропертиес
localization_priority: Normal
doc_type: resourcePageType
ms.prod: universal-print
ms.openlocfilehash: 1249eaae4d62cffe14935587c655ba402237b0ed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727971"
---
# <a name="printdocumentuploadproperties-resource-type"></a>Тип ресурса Принтдокументуплоадпропертиес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает отправляемый документ

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.printDocumentUploadProperties",
  "baseType": null
}-->

```json
{
  "contentType": "String",
  "documentName": "String",
  "size": "Int64",
}
```

## <a name="properties"></a>Свойства


| Свойство       | Тип              |Описание
|:-------------------|:------------------|:------------------------------------
| contentType | String    | Тип контента документа (MIME).
| Имя_документа | Строка | Имя документа.
| size          | Int64            | Размер документа в байтах.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "printDocumentUploadProperties",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
