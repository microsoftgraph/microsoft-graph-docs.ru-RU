# <a name="post-resource-type"></a>Тип ресурса Post
Представляет отдельный элемент Post в сущности [conversationThread](conversationthread.md).

Хотя явно создать экземпляр post невозможно, он будет создан в результате выполнения любого из указанных ниже действий.

- [Добавление ответа к существующей публикации](../api/post_reply.md). 
- [Добавление ответа к существующей цепочке](../api/conversationthread_reply.md). 
- [Создание цепочки в новой беседе](../api/group_post_threads.md).
- [Создание беседы](../api/group_post_conversations.md)

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](../../../concepts/extensibility_overview.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Вывод списка публикаций](../api/conversationthread_list_posts.md) | [post](post.md) |Получение публикаций из указанной цепочки. |
|[Получение публикации](../api/post_get.md) | [post](post.md) |Получение свойств и связей публикации в указанной цепочке.|
|[Ответ](../api/post_reply.md)|Нет|Ответ на публикацию и добавление новой публикации в указанную цепочку беседы группы.|
|[Переадресация](../api/post_forward.md)|Нет|Переадресация публикации получателю.|
|**Вложения**| | |
|[Вывод списка вложений](../api/post_list_attachments.md) |Коллекция [attachment](attachment.md) | Получает все вложения для экземпляра post.|
|[Добавление вложения](../api/post_post_attachments.md) |[attachment](attachment.md)| Добавление вложения в публикацию. |
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.|
|[Получение открытого расширения](../api/opentypeextension_get.md) |Коллекция [openTypeExtension](opentypeextension.md)| Получение объекта или объектов открытого расширения, которые определяются по имени или полному имени.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](../../../concepts/extensibility_schema_groups.md) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|**Расширенные свойства**| | |
|[Создание однозначного расширенного свойства](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[post](post.md)  |Создание одного или нескольких расширенных свойств с одним значением в новой или существующей публикации.   |
|[Получение публикации с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty_get.md)  | [post](post.md) | Получение публикаций, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [post](post.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новой или существующей публикации.  |
|[Получение публикации с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty_get.md)  | [post](post.md) | Получение публикации, которая содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|body|[itemBody](itembody.md)|Содержимое публикации. Это свойство используется по умолчанию. Это свойство может иметь значение null.|
|categories|Коллекция строк|Категории, сопоставленные с публикацией.|
|changeKey|String|Указывает версию публикации. При каждом изменении публикации также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|conversationId|String|Уникальный идентификатор беседы. Только для чтения.|
|conversationThreadId|String|Уникальный идентификатор цепочки беседы. Только для чтения.|
|createdDateTime|DateTimeOffset|Указывает, когда была создана публикация. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|from|[recipient](recipient.md)|Используется в сценариях делегированного доступа. Указывает, кто опубликовал сообщение от имени другого пользователя. Это свойство используется по умолчанию.|
|hasAttachments|Логическое|Указывает, есть ли в публикации хотя бы одно вложение. Это свойство используется по умолчанию.|
|id|String| Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Указывает дату и время последнего изменения публикации. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|newParticipants|Коллекция объектов [recipient](recipient.md)|Участники беседы, которые были добавлены в цепочку в рамках этой публикации.|
|receivedDateTime|DateTimeOffset|Указывает, когда была получена публикация. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|sender|[recipient](recipient.md)|Содержит электронный адрес отправителя. Если получатель не указан, то в качестве значения Sender используется адрес пользователя, прошедшего проверку подлинности. Это свойство используется по умолчанию.|

## <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [Attachment](attachment.md)| Только для чтения. Допускается значение null.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для публикации. Только для чтения. Допускается значение null.|
|inReplyTo|[post](post.md)| Только для чтения.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для публикации. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для публикации. Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.post"
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](../../../concepts/extensibility_overview.md)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](../../../concepts/extensibility_open_users.md)
- [Добавление пользовательских данных в группы с помощью расширений схемы](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
