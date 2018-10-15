# <a name="timeconstraint-resource-type"></a><span data-ttu-id="6f344-101">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="6f344-101">timeConstraint resource type</span></span>

<span data-ttu-id="6f344-102">Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.</span><span class="sxs-lookup"><span data-stu-id="6f344-102">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f344-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f344-103">JSON representation</span></span>

<span data-ttu-id="6f344-104">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6f344-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="6f344-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f344-105">Properties</span></span>
| <span data-ttu-id="6f344-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f344-106">Property</span></span>     | <span data-ttu-id="6f344-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6f344-107">Type</span></span>   |<span data-ttu-id="6f344-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6f344-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f344-109">activityDomain</span><span class="sxs-lookup"><span data-stu-id="6f344-109">activityDomain</span></span>|<span data-ttu-id="6f344-110">activityDomain</span><span class="sxs-lookup"><span data-stu-id="6f344-110">activityDomain</span></span>|<span data-ttu-id="6f344-111">Характер действия (необязательно).</span><span class="sxs-lookup"><span data-stu-id="6f344-111">The nature of the activity, optional. Possible values are: , , , or .</span></span> <span data-ttu-id="6f344-112">Возможные значения: `work`, `personal`, `unrestricted` или `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6f344-112">The possible values are  `work`,  `personal`,  `unrestricted`, or  `unknown`.</span></span>|
|<span data-ttu-id="6f344-113">timeslots</span><span class="sxs-lookup"><span data-stu-id="6f344-113">timeslots</span></span>|<span data-ttu-id="6f344-114">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="6f344-114">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="6f344-115">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="6f344-115">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
