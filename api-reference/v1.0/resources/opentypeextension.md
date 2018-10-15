# <a name="opentypeextension-resource-type-open-extensions"></a>Тип ресурса openTypeExtension (открытые расширения)

Открытые расширения (ранее известные как модули обработки данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.

Открытые расширения представлены ресурсом **openTypeExtension**. Все открытые расширения, добавленные в ресурс, отображаются в свойстве навигации **extensions**, которое является производным от абстрактного типа [extension](extension.md). Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство для всех расширений.

Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных DNS, который зависит от _принадлежащего вам домена_, например `Com.Contoso.ContactInfo`. Не указывайте домен Майкрософт (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения.

Пример открытого расширения. [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](../../../concepts/extensibility_open_users.md).

Открытые расширения поддерживаются указанными ниже ресурсами в соответствующих версиях — общедоступной (1.0 или бета-версии) или предварительной (бета-версии).

|Ресурс |Версия |
|:---------------|:-------|
| [administrativeUnit](../../beta/resources/administrativeunit.md)  | Только предварительная версия |
| [[event](event.md) для календаря](event.md) | Общедоступная версия |
| [event](event.md) для календаря группы | Общедоступная версия |
| [post](post.md) цепочки беседы группы | Общедоступная версия |
| [device](device.md) | Общедоступная версия |
| [group](group.md) | Общедоступная версия |
| [message](message.md) | Общедоступная версия |
| [organization](organization.md) | Общедоступная версия |
| [[contact](contact.md) (личный контакт)](contact.md) | Общедоступная версия |
| [user](user.md) | Общедоступная версия |

## <a name="outlook-specific-considerations"></a>Особенности при работе с Outlook

Каждое открытое расширение для ресурса Outlook (событие, сообщение или личный контакт) хранится в [именованном свойстве MAPI](https://msdn.microsoft.com/en-us/library/cc765864(v=office.15).aspx). При создании открытых расширений для Outlook необходимо учитывать, что именованные свойства MAPI — это ограниченные ресурсы в почтовом ящике пользователя. Когда квота на именованные свойства исчерпается, создавать их для этого пользователя будет невозможно. Это может привести к непредсказуемым реакциям со стороны клиентов, зависящих от именованных свойств функции.

При создании открытых расширений ресурсов Outlook следуйте рекомендациям, приведенным ниже.

- Создайте минимальное число необходимых расширений. Для большинства приложений должно требоваться не более одного расширения. У расширения не должно быть свойств или структуры, определенных набором, чтобы можно было хранить множество значений в одном расширении.
- Избегайте именования расширений так же, как переменных (например, на основе введенных пользователем данных и т. д.). Каждый раз, когда создается открытое расширение с новым именем, которое ранее не использовалось в почтовом ящике пользователя, также создается новое именованное свойство MAPI. Удаление расширения не удаляет именованное свойство.

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Случаи применения открытых расширений (для ресурсов Outlook) и расширенных свойств

Открытые расширения — рекомендуемое решение для большинства случаев, предусматривающих хранение пользовательских данных и доступ к ним. |||UNTRANSLATED_CONTENT_START|||If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](http://developer.microsoft.com/en-us/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).|||UNTRANSLATED_CONTENT_END||| Можно проверить, какие метаданные представлены в [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.extension",
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a>Свойства

|Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|extensionName|String (строка)|Уникальный текстовый идентификатор для открытых расширений открытого типа. Обязательно свойство.|
|id|String (строка)| Полный идентификатор, в котором сцеплены тип расширения и свойство **extensionName**. Только для чтения.|

## <a name="relationships"></a>Связи

Нет

## <a name="methods"></a>Методы

|Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension_post_opentypeextension.md) | Объект [openTypeExtension](opentypeextension.md) (в существующем экземпляре ресурса) либо новый ресурс [contact](../resources/contact.md), [event](../resources/event.md) или [message](../resources/message.md), содержащий объект openTypeExtension. | Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.|
|[Get](../api/opentypeextension_get.md) | [openTypeExtension](opentypeextension.md) |Чтение свойств и связей объекта openTypeExtension.|
|[Update](../api/opentypeextension_update.md) | [openTypeExtension](opentypeextension.md) |Обновление объекта openTypeExtension. |
|[Delete](../api/opentypeextension_delete.md) | Нет |Удаление объекта openTypeExtension. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
