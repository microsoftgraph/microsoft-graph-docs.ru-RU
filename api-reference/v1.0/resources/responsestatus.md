# <a name="responsestatus-resource-type"></a><span data-ttu-id="f83bc-101">Тип ресурса responseStatus</span><span class="sxs-lookup"><span data-stu-id="f83bc-101">responseStatus resource type</span></span>

<span data-ttu-id="f83bc-102">Состояние ответа к приглашению на собрание.</span><span class="sxs-lookup"><span data-stu-id="f83bc-102">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="f83bc-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="f83bc-103">Properties</span></span>

| <span data-ttu-id="f83bc-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="f83bc-104">Property</span></span> | <span data-ttu-id="f83bc-105">Тип</span><span class="sxs-lookup"><span data-stu-id="f83bc-105">Type</span></span>           | <span data-ttu-id="f83bc-106">Описание</span><span class="sxs-lookup"><span data-stu-id="f83bc-106">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="f83bc-107">response</span><span class="sxs-lookup"><span data-stu-id="f83bc-107">response</span></span> | <span data-ttu-id="f83bc-108">responseType</span><span class="sxs-lookup"><span data-stu-id="f83bc-108">ResponseType</span></span>   | <span data-ttu-id="f83bc-109">Тип ответа.</span><span class="sxs-lookup"><span data-stu-id="f83bc-109">The response type.</span></span> <span data-ttu-id="f83bc-110">Возможные значения: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="f83bc-110">The possible values are `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`, , , , , , or .</span></span>
| <span data-ttu-id="f83bc-111">time</span><span class="sxs-lookup"><span data-stu-id="f83bc-111">time</span></span>     | <span data-ttu-id="f83bc-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f83bc-112">DateTimeOffset</span></span> | <span data-ttu-id="f83bc-p102">Дата и время возвращения ответа. Они представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f83bc-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="f83bc-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f83bc-116">JSON representation</span></span>

<span data-ttu-id="f83bc-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f83bc-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
