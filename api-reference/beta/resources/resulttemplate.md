---
title: тип ресурса resultTemplate
description: Словарь resultTemplateIds и связанных с ними значений, которые включают имя и схему JSON шаблонов результатов.
localization_priority: Normal
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 402b60efc278e72102d9bba4eb89be2dda38916b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211374"
---
# <a name="resulttemplate-resource-type"></a>тип ресурса resultTemplate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Словарь **resultTemplateIds** и связанных значений, который включает имя и схему JSON шаблонов результатов.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|key|String|ID шаблона результатов. Он должен сопопозить **с resultTemplateId** в [searchHit.](searchhit.md)|
|displayName|String|Имя шаблона результатов.|
|body|Json|Схема шаблона результатов JSON.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplate",
  "baseType": null
}-->


```json
{
  "resultTemplateId": {
                    "displayName": "String",
                    "body": "Json schema"
                }
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


