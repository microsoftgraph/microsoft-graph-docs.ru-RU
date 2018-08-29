# <a name="attendeebase-resource-type"></a><span data-ttu-id="c541b-101">Тип ресурсов attendeeBase</span><span class="sxs-lookup"><span data-stu-id="c541b-101">attendeeBase resource type</span></span>

<span data-ttu-id="c541b-102">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="c541b-102">The type of attendee.</span></span>

<span data-ttu-id="c541b-103">Тип, производный от [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="c541b-103">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c541b-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c541b-104">JSON representation</span></span>

<span data-ttu-id="c541b-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c541b-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="c541b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c541b-106">Properties</span></span>
| <span data-ttu-id="c541b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c541b-107">Property</span></span>     | <span data-ttu-id="c541b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c541b-108">Type</span></span>   |<span data-ttu-id="c541b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c541b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c541b-110">type</span><span class="sxs-lookup"><span data-stu-id="c541b-110">type</span></span>|<span data-ttu-id="c541b-111">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="c541b-111">AttendeeType</span></span>| <span data-ttu-id="c541b-112">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="c541b-112">The type of attendee.</span></span> <span data-ttu-id="c541b-113">Возможные значения: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="c541b-113">The possible values are `required`, `optional`, `resource`, , , , , , , , , or .</span></span> <span data-ttu-id="c541b-114">В настоящее время, если участник является человеком, действие [findMeetingTimes](../api/user_findmeetingtimes.md) всегда предполагает, что человек имеет тип `Required`.</span><span class="sxs-lookup"><span data-stu-id="c541b-114">The type of attendee. Possible values are: , , . Currently if the attendee is a person, [findMeetingTimes](../api/user_findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="c541b-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c541b-115">emailAddress</span></span>|[<span data-ttu-id="c541b-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c541b-116">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="c541b-117">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="c541b-117">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
