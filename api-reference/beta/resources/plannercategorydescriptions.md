<a id="plannercategorydescriptions-resource-type" class="xliff"></a>

# Тип ресурса plannerCategoryDescriptions

Ресурс **plannerCategoryDescriptions** представляет описательные метки категорий, заданных для плана. Он принадлежит объекту [сведений о плане](plannerplandetails.md). Можно задать до 6 категорий. 


<a id="properties" class="xliff"></a>

## Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|category1|String|Метка, сопоставленная с категорией 1.|
|category2|String|Метка, сопоставленная с категорией 2.|
|category3|String|Метка, сопоставленная с категорией 3.|
|category4|String|Метка, сопоставленная с категорией 4.|
|category5|String|Метка, сопоставленная с категорией 5.|
|category6|String|Метка, сопоставленная с категорией 6.|

<a id="json-representation" class="xliff"></a>

## Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->