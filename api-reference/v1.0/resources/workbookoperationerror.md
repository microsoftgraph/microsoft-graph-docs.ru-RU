---
title: Тип ресурса Воркбукоператионеррор
description: Представляет ошибку при выполнении неудачной операции с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a04d26a7bdeb14f35859e7c1b02e781b64189201
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408161"
---
# <a name="workbookoperationerror-resource-type"></a>Тип ресурса Воркбукоператионеррор

Представляет ошибку при выполнении неудачной операции с книгой.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|code|Строка| Код ошибки.|
|message|String| Сообщение об ошибке.|
|innererror|error object| Необязательное. Дополнительные объекты ошибки, которые могут быть более информативны, чем сообщение об ошибке верхнего уровня.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperationError",
  "baseType": null
}-->

```json
{
  "code": "String",
  "message": "String",
  "innererror": { "@odata.type": "odata.error" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
