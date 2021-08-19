---
title: тип ресурса workbookOperationError
description: Представляет ошибку при сбойной операции книги.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9c5e3fa689cc830bf1041c240bf135de2fbab116ef876871a086fe66595b3e89
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241116"
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


