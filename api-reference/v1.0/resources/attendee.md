# <a name="attendee-resource-type"></a><span data-ttu-id="98eb4-101">Тип ресурса attendee</span><span class="sxs-lookup"><span data-stu-id="98eb4-101">attendee resource type</span></span>

<span data-ttu-id="98eb4-102">Участник события.</span><span class="sxs-lookup"><span data-stu-id="98eb4-102">An event attendee.</span></span> <span data-ttu-id="98eb4-103">Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.</span><span class="sxs-lookup"><span data-stu-id="98eb4-103">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="98eb4-104">Тип, производный от [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="98eb4-104">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="98eb4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="98eb4-105">Properties</span></span>
| <span data-ttu-id="98eb4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="98eb4-106">Property</span></span>     | <span data-ttu-id="98eb4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="98eb4-107">Type</span></span>   |<span data-ttu-id="98eb4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="98eb4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98eb4-109">status</span><span class="sxs-lookup"><span data-stu-id="98eb4-109">status</span></span>|[<span data-ttu-id="98eb4-110">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="98eb4-110">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="98eb4-111">Ответ участника (нет, принято, отклонено и т. д.) на событие, а также дата и время отправки ответа.</span><span class="sxs-lookup"><span data-stu-id="98eb4-111">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="98eb4-112">type</span><span class="sxs-lookup"><span data-stu-id="98eb4-112">type</span></span>|<span data-ttu-id="98eb4-113">String</span><span class="sxs-lookup"><span data-stu-id="98eb4-113">String</span></span>|<span data-ttu-id="98eb4-114">Тип участника: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="98eb4-114">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="98eb4-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="98eb4-115">emailAddress</span></span>|[<span data-ttu-id="98eb4-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="98eb4-116">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="98eb4-117">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="98eb4-117">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98eb4-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="98eb4-118">JSON representation</span></span>

<span data-ttu-id="98eb4-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98eb4-119">Here is a JSON representation of the resource</span></span>

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