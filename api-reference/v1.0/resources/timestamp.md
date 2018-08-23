# <a name="timestamp-resource-type"></a><span data-ttu-id="2069d-101">Тип ресурса timeStamp</span><span class="sxs-lookup"><span data-stu-id="2069d-101">timeStamp resource type</span></span>

<span data-ttu-id="2069d-102">Сведения о дате и времени в определенный момент.</span><span class="sxs-lookup"><span data-stu-id="2069d-102">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2069d-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2069d-103">JSON representation</span></span>

<span data-ttu-id="2069d-104">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="2069d-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="2069d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2069d-105">Properties</span></span>
| <span data-ttu-id="2069d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2069d-106">Property</span></span>       | <span data-ttu-id="2069d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2069d-107">Type</span></span>    |<span data-ttu-id="2069d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2069d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2069d-109">date</span><span class="sxs-lookup"><span data-stu-id="2069d-109">date</span></span>|<span data-ttu-id="2069d-110">Date</span><span class="sxs-lookup"><span data-stu-id="2069d-110">Date</span></span>|<span data-ttu-id="2069d-111">Дата из метки времени.</span><span class="sxs-lookup"><span data-stu-id="2069d-111">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="2069d-112">time</span><span class="sxs-lookup"><span data-stu-id="2069d-112">time</span></span>|<span data-ttu-id="2069d-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2069d-113">TimeOfDay</span></span>|<span data-ttu-id="2069d-114">Время из метки времени.</span><span class="sxs-lookup"><span data-stu-id="2069d-114">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="2069d-115">timeZone</span><span class="sxs-lookup"><span data-stu-id="2069d-115">timeZone</span></span>|<span data-ttu-id="2069d-116">String</span><span class="sxs-lookup"><span data-stu-id="2069d-116">String</span></span>|<span data-ttu-id="2069d-117">Часовой пояс из метки времени — один из 24 часовых поясов планеты.</span><span class="sxs-lookup"><span data-stu-id="2069d-117">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->