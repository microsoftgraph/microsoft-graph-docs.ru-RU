# <a name="multivaluelegacyextendedproperty-resource-type"></a>Тип ресурса multiValueLegacyExtendedProperty

Расширенное свойство, содержащее коллекцию значений.

Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | Экземпляр поддерживаемого ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) или [contactFolder](../resources/contactfolder.md). Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются. | Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса. |
|[Получение](../api/multivaluelegacyextendedproperty_get.md) |Экземпляр поддерживаемого ресурса ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) или [post](../resources/post.md) группы), расширенный объектом [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md). |Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.|

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|id|string|Идентификатор свойства. Только для чтения.|
|значение|Коллекция строк|Коллекция значений свойств.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.multivaluelegacyextendedproperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->