---
title: тип ресурса workbookOperationError
description: Представляет ошибку при сбойной операции книги.
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ef27d5c3efe782c4d865e2badfb306aa93068ccc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59119753"
---
# <a name="workbookoperationerror-resource-type"></a>тип ресурса workbookOperationError

Представляет ошибку при сбойной операции книги.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|code|String| Код ошибки.|
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


