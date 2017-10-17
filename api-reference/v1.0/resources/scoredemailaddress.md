# <a name="scoredemailaddress-resource-type"></a>тип ресурса scoredEmailAddress

Представляет оцененный адрес электронной почты.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|string|Адрес электронной почты.|
|relevanceScore|double|Оценка релевантности адреса электронной почты. Оценка релевантности выступает в роли ключа сортировки по отношению к другим возвращаемым результатам. Более высокий показатель релевантности говорит о высокой степени соответствия результата. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-связями. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024.0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
