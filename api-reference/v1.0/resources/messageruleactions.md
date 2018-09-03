# <a name="messageruleactions-resource-type"></a>Тип ресурса messageRuleActions


Представляет набор действий, доступных для правила.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| assignCategories | Коллекция String | Список категорий, которые необходимо назначить сообщению. |
| copyToFolder | String (строка) | Идентификатор папки, в которую необходимо скопировать сообщение. |
| delete | Boolean (логический) | Указывает, нужно ли перемещать сообщение в папку "Удаленные". |
| forwardAsAttachmentTo | Коллекция [recipient](recipient.md) | Электронные адреса получателей, которым необходимо переслать сообщение как вложение. |
| forwardTo | Коллекция [recipient](recipient.md) | Электронные адреса получателей, которым необходимо переслать сообщение. |
| markAsRead | Boolean (логический) | Указывает, необходимо ли отмечать сообщение как прочтенное. |
| markImportance | importance | Задает важность сообщения. Возможные значения: `low`, `normal`, `high`. |
| moveToFolder |  String (строка)| Идентификатор папки, в которую сообщение будет перемещено. |
| permanentDelete | Boolean (логический) | Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные". |
| redirectTo | Коллекция [recipient](recipient.md) | Электронные адреса, на которые должно быть перенаправлено сообщение. |
| stopProcessingRules | Boolean (логический) | Указывает, должны ли обрабатываться последующие правила. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->