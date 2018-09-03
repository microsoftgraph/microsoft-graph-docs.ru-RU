# <a name="customtimezone-resource-type"></a><span data-ttu-id="fcea1-101">Тип ресурса customTimeZone</span><span class="sxs-lookup"><span data-stu-id="fcea1-101">customTimeZone resource type</span></span>

<span data-ttu-id="fcea1-102">Представляет часовой пояс c нестандартным переходом на летнее время и обратно.</span><span class="sxs-lookup"><span data-stu-id="fcea1-102">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="fcea1-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcea1-103">Properties</span></span>
| <span data-ttu-id="fcea1-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcea1-104">Property</span></span>     | <span data-ttu-id="fcea1-105">Тип</span><span class="sxs-lookup"><span data-stu-id="fcea1-105">Type</span></span>   |<span data-ttu-id="fcea1-106">Описание</span><span class="sxs-lookup"><span data-stu-id="fcea1-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fcea1-107">bias</span><span class="sxs-lookup"><span data-stu-id="fcea1-107">bias</span></span> | <span data-ttu-id="fcea1-108">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fcea1-108">Edm.Int32</span></span> | <span data-ttu-id="fcea1-109">Смещение времени часового пояса относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="fcea1-109">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="fcea1-110">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="fcea1-110">This value is in minutes.</span></span> <span data-ttu-id="fcea1-111">Часовые пояса с положительным смещением от UTC опережают время UTC, а с отрицательным смещением — отстают от него.</span><span class="sxs-lookup"><span data-stu-id="fcea1-111">Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="fcea1-112">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="fcea1-112">daylightOffset</span></span> | [<span data-ttu-id="fcea1-113">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="fcea1-113">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="fcea1-114">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="fcea1-114">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="fcea1-115">name</span><span class="sxs-lookup"><span data-stu-id="fcea1-115">name</span></span> | <span data-ttu-id="fcea1-116">строка</span><span class="sxs-lookup"><span data-stu-id="fcea1-116">string</span></span> | <span data-ttu-id="fcea1-117">Имя настраиваемого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="fcea1-117">The name of the custom time zone.</span></span> |
| <span data-ttu-id="fcea1-118">standardOffset</span><span class="sxs-lookup"><span data-stu-id="fcea1-118">standardOffset</span></span> | [<span data-ttu-id="fcea1-119">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="fcea1-119">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="fcea1-120">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="fcea1-120">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="fcea1-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcea1-121">JSON representation</span></span>

<span data-ttu-id="fcea1-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcea1-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.timeZoneBase",
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->