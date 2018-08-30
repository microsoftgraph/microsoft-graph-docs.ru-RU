# <a name="locationconstraint-resource-type"></a><span data-ttu-id="c5a6b-101">Тип ресурсов locationConstraint</span><span class="sxs-lookup"><span data-stu-id="c5a6b-101">locationConstraint resource type</span></span>

<span data-ttu-id="c5a6b-102">Условия, заданные клиентом в отношении расположения для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="c5a6b-102">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5a6b-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c5a6b-103">JSON representation</span></span>

<span data-ttu-id="c5a6b-104">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c5a6b-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="c5a6b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5a6b-105">Properties</span></span>
| <span data-ttu-id="c5a6b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5a6b-106">Property</span></span>     | <span data-ttu-id="c5a6b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c5a6b-107">Type</span></span>   |<span data-ttu-id="c5a6b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c5a6b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5a6b-109">isRequired</span><span class="sxs-lookup"><span data-stu-id="c5a6b-109">isRequired</span></span>|<span data-ttu-id="c5a6b-110">Логический</span><span class="sxs-lookup"><span data-stu-id="c5a6b-110">Boolean</span></span>|<span data-ttu-id="c5a6b-p101">Клиент запрашивает у службы включение в отклик данных о расположении для проведения собрания. Если задано значение true и все ресурсы заняты, [findMeetingTimes](../api/user_findmeetingtimes.md) не вернет вариантов времени для проведения собрания. Если задано значение false и все ресурсы заняты, **findMeetingTimes** все равно будет искать варианты времени для проведения собрания, но без указания расположений.</span><span class="sxs-lookup"><span data-stu-id="c5a6b-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user_findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="c5a6b-114">locations</span><span class="sxs-lookup"><span data-stu-id="c5a6b-114">locations</span></span>|<span data-ttu-id="c5a6b-115">Коллекция [locationConstraintItem](locationconstraintitem.md)</span><span class="sxs-lookup"><span data-stu-id="c5a6b-115">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="c5a6b-116">Ограниченные сведения об одном или нескольких расположениях, которые клиент запрашивает для собрания.</span><span class="sxs-lookup"><span data-stu-id="c5a6b-116">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="c5a6b-117">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="c5a6b-117">suggestLocation</span></span>|<span data-ttu-id="c5a6b-118">Логический</span><span class="sxs-lookup"><span data-stu-id="c5a6b-118">Boolean</span></span>|<span data-ttu-id="c5a6b-119">Клиент запрашивает у службы один или несколько вариантов расположений для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="c5a6b-119">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->