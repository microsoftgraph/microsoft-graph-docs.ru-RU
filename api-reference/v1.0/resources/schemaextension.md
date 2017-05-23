# <a name="schemaextension-resource-type-schema-extensions"></a>Тип ресурса schemaExtension (расширения схемы)

С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип. 

Расширения схемы поддерживаются в ресурсах указанных ниже типов.

 - [contact](contact.md)
 - [device](device.md)
 - [event](event.md) (для пользователя или календаря группы Office 365)
 - [post](post.md) (для группы Office 365)
 - [group](group.md)
 - [message](message.md) 
 - [organization](organization.md)
 - [user](user.md)

Сведения о том, как добавлять пользовательские данные в группы, см. в [примере расширения схемы](../../../concepts/extensibility_schema_groups.md).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание](../api/schemaextension_post_schemaextensions.md) | schemaExtension |Создание определения расширения схемы.|
|[Перечисление](../api/schemaextension_list.md) | schemaExtension |Создание списка доступных определений schemaExtension и их свойств.|
|[Получение](../api/schemaextension_get.md) | schemaExtension |Получение свойств указанного определения schemaExtension.|
|[Обновление](../api/schemaextension_update.md) | schemaExtension    |Обновление определения schemaExtension. |
|[Удаление](../api/schemaextension_delete.md) | Нет |Удаление определения schemaExtension. |

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|description|String|Описание расширения схемы.|
|id|String|Уникальный идентификатор определения расширения схемы. Значение должно представлять собой объединение одного из проверенных доменов (например, contoso.com) и имени расширения схемы. Пример: *contoso_mySchema*. |
|owner|String|appId приложения, создавшего расширение схемы. Только для чтения.|
|properties|Коллекция [extensionSchemaProperty](extensionschemaproperty.md)|Коллекция имен и типов свойств, составляющих определение расширения схемы.|
|status|String|Состояние жизненного цикла расширения схемы. Возможные состояния: **InDevelopment**, **Available** и **Deprecated**. При создании свойство автоматически получает значение **InDevelopment**. [Расширения схемы](../../../concepts/extensibility_overview.md#schema-extensions) предоставляют дополнительные сведения о возможных переходах из одного состояния в другое и об их поведении.|
|targetTypes|Коллекция String|Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы. Возможные варианты: **contact**, **device**, **event**, **group**, **message**, **organization**, **post** или **user**.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->