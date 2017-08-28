# <a name="recurrencerange-resource-type"></a><span data-ttu-id="bd8c7-101">Тип ресурса recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="bd8c7-101">recurrenceRange resource type</span></span>

<span data-ttu-id="bd8c7-102">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-102">The duration of an event.</span></span>

## <a name="properties"></a><span data-ttu-id="bd8c7-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd8c7-103">Properties</span></span>

| <span data-ttu-id="bd8c7-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd8c7-104">Property</span></span>     | <span data-ttu-id="bd8c7-105">Тип</span><span class="sxs-lookup"><span data-stu-id="bd8c7-105">Type</span></span>   |<span data-ttu-id="bd8c7-106">Описание</span><span class="sxs-lookup"><span data-stu-id="bd8c7-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd8c7-107">endDate</span><span class="sxs-lookup"><span data-stu-id="bd8c7-107">endDate</span></span>|<span data-ttu-id="bd8c7-108">Date</span><span class="sxs-lookup"><span data-stu-id="bd8c7-108">Date</span></span>|<span data-ttu-id="bd8c7-109">Дата окончания ряда.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-109">The end date of the series.</span></span>|
|<span data-ttu-id="bd8c7-110">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="bd8c7-110">numberOfOccurrences</span></span>|<span data-ttu-id="bd8c7-111">Int32</span><span class="sxs-lookup"><span data-stu-id="bd8c7-111">Int32</span></span>|<span data-ttu-id="bd8c7-112">Количество повторений события.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-112">How many times to repeat the event.</span></span>|
|<span data-ttu-id="bd8c7-113">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="bd8c7-113">recurrenceTimeZone</span></span>|<span data-ttu-id="bd8c7-114">String</span><span class="sxs-lookup"><span data-stu-id="bd8c7-114">String</span></span> |<span data-ttu-id="bd8c7-115">Часовой пояс для свойств **startDate** и **endDate**.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-115">Time zone for the **startDate** and **endDate** properties.</span></span> |
|<span data-ttu-id="bd8c7-116">startDate</span><span class="sxs-lookup"><span data-stu-id="bd8c7-116">startDate</span></span>|<span data-ttu-id="bd8c7-117">Date</span><span class="sxs-lookup"><span data-stu-id="bd8c7-117">Date</span></span>|<span data-ttu-id="bd8c7-118">Дата начала ряда.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-118">The start date of the series.</span></span>|
|<span data-ttu-id="bd8c7-119">type</span><span class="sxs-lookup"><span data-stu-id="bd8c7-119">type</span></span>|<span data-ttu-id="bd8c7-120">String</span><span class="sxs-lookup"><span data-stu-id="bd8c7-120">String</span></span>|<span data-ttu-id="bd8c7-p101">Диапазон повторения: EndDate = 0, NoEnd = 1, Numbered = 2. Возможные значения: `EndDate`, `NoEnd`, `Numbered`.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-p101">The recurrence range: EndDate = 0, NoEnd = 1, Numbered = 2. Possible values are: `EndDate`, `NoEnd`, `Numbered`.</span></span>||

## <a name="json-representation"></a><span data-ttu-id="bd8c7-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd8c7-123">JSON representation</span></span>

<span data-ttu-id="bd8c7-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencerange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
