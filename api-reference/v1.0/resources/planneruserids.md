<span data-ttu-id="36cdb-p102">Клиент может определять свойства открытого типа. В этом случае клиент должен предоставить идентификаторы пользователей в качестве свойств, причем они должны иметь значение `true` (логическое). Если больше не нужно предоставлять доступ для идентификаторов пользователей, задайте для свойств значение `false` (логическое), и свойства будут автоматически удалены.</span><span class="sxs-lookup"><span data-stu-id="36cdb-p102">Properties of an Open Type can be defined by the client. In this case, the client should provide user ids as properties with their values being the `true` boolean. When user ids are no longer shared with, properties are automatically removed by setting their values to the `false` boolean.</span></span>
Клиент может определять свойства открытого типа. В этом случае клиент должен предоставить идентификаторы пользователей в качестве свойств, причем они должны иметь значение `true` (логическое). Если больше не нужно предоставлять доступ для идентификаторов пользователей, задайте для свойств значение `false` (логическое), и свойства будут автоматически удалены.


## <span data-ttu-id="36cdb-110">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="36cdb-110">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="36cdb-111">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36cdb-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="36cdb-112">Пример:</span><span class="sxs-lookup"><span data-stu-id="36cdb-112">// Example</span></span>
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->