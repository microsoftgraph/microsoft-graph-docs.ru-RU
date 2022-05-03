---
author: nilakhan
description: Представляет сведения для отправки документа для печати
title: Тип ресурса printDocumentUploadProperties
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: 219834eb64863d67dcc6e3ed75f33bc08eead768
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176897"
---
# <a name="printdocumentuploadproperties-resource-type"></a>Тип ресурса printDocumentUploadProperties

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описание передаваемого документа

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
| contentType | String    | Тип содержимого документа (MIME).
| documentName | Строка | Имя документа.
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
