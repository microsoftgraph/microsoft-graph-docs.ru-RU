# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="b4fa3-101">Тип ресурса timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="b4fa3-101">timeZoneInformation resource type</span></span>


<span data-ttu-id="b4fa3-102">Представляет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="b4fa3-102">Represents information about a time zone.</span></span> <span data-ttu-id="b4fa3-103">Поддерживаются формат Windows и формат [часового пояса IANA](http://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).</span><span class="sxs-lookup"><span data-stu-id="b4fa3-103">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](http://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="b4fa3-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4fa3-104">Properties</span></span>
| <span data-ttu-id="b4fa3-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4fa3-105">Property</span></span>     | <span data-ttu-id="b4fa3-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b4fa3-106">Type</span></span>   |<span data-ttu-id="b4fa3-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b4fa3-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4fa3-108">alias</span><span class="sxs-lookup"><span data-stu-id="b4fa3-108">alias</span></span>|<span data-ttu-id="b4fa3-109">string</span><span class="sxs-lookup"><span data-stu-id="b4fa3-109">string</span></span>|<span data-ttu-id="b4fa3-110">Идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="b4fa3-110">An identifier for the time zone.</span></span>|
|<span data-ttu-id="b4fa3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b4fa3-111">displayName</span></span>|<span data-ttu-id="b4fa3-112">string</span><span class="sxs-lookup"><span data-stu-id="b4fa3-112">string</span></span>|<span data-ttu-id="b4fa3-113">Отображаемое имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="b4fa3-113">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4fa3-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b4fa3-114">JSON representation</span></span>

<span data-ttu-id="b4fa3-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4fa3-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->