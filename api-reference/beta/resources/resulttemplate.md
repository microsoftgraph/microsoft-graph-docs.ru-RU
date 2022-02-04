---
title: тип ресурса resultTemplate
description: 'Словарь resultTemplateIds и связанных с ними значений, которые включают имя и схему JSON шаблонов результатов.'
ms.localizationpriority: medium
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
---

# <a name="resulttemplate-resource-type"></a>тип ресурса resultTemplate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Словарь **resultTemplateIds** и связанных значений, который включает имя и схему JSON шаблонов результатов.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|key|Строка|ID шаблона результатов. Он должен сопопозить **с resultTemplateId** в [searchHit](searchhit.md).|
|displayName|Строка|Имя шаблона результатов.|
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


