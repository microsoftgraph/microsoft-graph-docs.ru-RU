# <a name="attendee-resource-type"></a><span data-ttu-id="69d28-101">Тип ресурса attendee</span><span class="sxs-lookup"><span data-stu-id="69d28-101">attendee resource type</span></span>

<span data-ttu-id="69d28-102">Участник события.</span><span class="sxs-lookup"><span data-stu-id="69d28-102">An event attendee.</span></span>

<span data-ttu-id="69d28-103">Тип, производный от [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="69d28-103">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="69d28-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="69d28-104">Properties</span></span>
| <span data-ttu-id="69d28-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="69d28-105">Property</span></span>     | <span data-ttu-id="69d28-106">Тип</span><span class="sxs-lookup"><span data-stu-id="69d28-106">Type</span></span>   |<span data-ttu-id="69d28-107">Описание</span><span class="sxs-lookup"><span data-stu-id="69d28-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69d28-108">status</span><span class="sxs-lookup"><span data-stu-id="69d28-108">status</span></span>|[<span data-ttu-id="69d28-109">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="69d28-109">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="69d28-110">Ответ участника (нет, принято, отклонено и т. д.) на событие, а также дата и время отправки ответа.</span><span class="sxs-lookup"><span data-stu-id="69d28-110">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="69d28-111">type</span><span class="sxs-lookup"><span data-stu-id="69d28-111">type</span></span>|<span data-ttu-id="69d28-112">String</span><span class="sxs-lookup"><span data-stu-id="69d28-112">String</span></span>|<span data-ttu-id="69d28-113">Тип участника: `Required`, `Optional`, `Resource`.</span><span class="sxs-lookup"><span data-stu-id="69d28-113">The attendee type: `Required`, `Optional`, `Resource`.</span></span>|
|<span data-ttu-id="69d28-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="69d28-114">emailAddress</span></span>|[<span data-ttu-id="69d28-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="69d28-115">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="69d28-116">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="69d28-116">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69d28-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="69d28-117">JSON representation</span></span>

<span data-ttu-id="69d28-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69d28-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->