# <a name="educationterm-resource-type"></a><span data-ttu-id="bd403-101">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="bd403-101">educationTerm resource type</span></span>

<span data-ttu-id="bd403-102">Срок.</span><span class="sxs-lookup"><span data-stu-id="bd403-102">A term.</span></span> <span data-ttu-id="bd403-103">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="bd403-103">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="bd403-104">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="bd403-104">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bd403-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd403-105">Properties</span></span>
| <span data-ttu-id="bd403-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd403-106">Property</span></span>     | <span data-ttu-id="bd403-107">Тип</span><span class="sxs-lookup"><span data-stu-id="bd403-107">Type</span></span>   |<span data-ttu-id="bd403-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bd403-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd403-109">displayName</span><span class="sxs-lookup"><span data-stu-id="bd403-109">displayName</span></span>| <span data-ttu-id="bd403-110">String</span><span class="sxs-lookup"><span data-stu-id="bd403-110">String</span></span>| <span data-ttu-id="bd403-111">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="bd403-111">Display name of the template.</span></span>| 
|<span data-ttu-id="bd403-112">externalId</span><span class="sxs-lookup"><span data-stu-id="bd403-112">externalId</span></span>|<span data-ttu-id="bd403-113">String</span><span class="sxs-lookup"><span data-stu-id="bd403-113">String</span></span>| <span data-ttu-id="bd403-114">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bd403-114">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="bd403-115">startDate</span><span class="sxs-lookup"><span data-stu-id="bd403-115">startDate</span></span>|<span data-ttu-id="bd403-116">Date</span><span class="sxs-lookup"><span data-stu-id="bd403-116">Date</span></span>|<span data-ttu-id="bd403-117">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="bd403-117">Start of the term.</span></span>|
|<span data-ttu-id="bd403-118">endDate</span><span class="sxs-lookup"><span data-stu-id="bd403-118">endDate</span></span>|<span data-ttu-id="bd403-119">Date</span><span class="sxs-lookup"><span data-stu-id="bd403-119">Date</span></span>|<span data-ttu-id="bd403-120">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="bd403-120">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd403-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bd403-121">JSON representation</span></span>

<span data-ttu-id="bd403-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd403-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->