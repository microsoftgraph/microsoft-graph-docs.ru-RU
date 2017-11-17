<a id="plannerexternalreference-resource-type" class="xliff"></a>

# Тип ресурса plannerExternalReference

Ресурс **plannerExternalReference** представляет метаданные справочных материалов (такие вложения, как файл, URL-адрес). Это значение пар "свойство-значение" в объекте [externalReferences](plannerexternalreferences.md).



<a id="properties" class="xliff"></a>

## Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|alias|String|Псевдоним имени для описания справочных материалов.|
|lastModifiedBy|[identitySet](identityset.md)|Только для чтения. Идентификатор автора последних изменений.|
|lastModifiedDateTime|DateTimeOffset|Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|previewPriority|String|Позволяет задать порядок относительного приоритета, согласно которому справочные материалы будут отображаться при предварительном просмотре для задачи.|
|type|String|Используется для описания типа справочных материалов. Типы: `PowerPoint`, `Word`, `Excel`, `Other`.|

<a id="json-representation" class="xliff"></a>

## Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->