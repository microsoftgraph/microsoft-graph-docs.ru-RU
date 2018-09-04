# <a name="followupflag-resource-type"></a><span data-ttu-id="4bf61-101">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="4bf61-101">followupFlag resource type</span></span>


<span data-ttu-id="4bf61-102">Позволяет установить отметку для пользователя, что к этому элементу необходимо вернуться позже.</span><span class="sxs-lookup"><span data-stu-id="4bf61-102">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="4bf61-103">К поддерживаемым элементам относятся [message](message.md) и [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="4bf61-103">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4bf61-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4bf61-104">Properties</span></span>
| <span data-ttu-id="4bf61-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bf61-105">Property</span></span>     | <span data-ttu-id="4bf61-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4bf61-106">Type</span></span>   |<span data-ttu-id="4bf61-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4bf61-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bf61-108">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bf61-108">completedDateTime</span></span>|[<span data-ttu-id="4bf61-109">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4bf61-109">dateTimeTimeZone</span></span>](dateTimeTimeZone.md)|<span data-ttu-id="4bf61-110">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="4bf61-110">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="4bf61-111">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="4bf61-111">dueDateTime</span></span>|<span data-ttu-id="4bf61-112">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="4bf61-112">**dateTimeTimeZone**</span></span>|<span data-ttu-id="4bf61-113">Дата и время, когда выполнение должно быть завершено.</span><span class="sxs-lookup"><span data-stu-id="4bf61-113">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="4bf61-114">flagStatus</span><span class="sxs-lookup"><span data-stu-id="4bf61-114">flagStatus</span></span>|<span data-ttu-id="4bf61-115">FollowupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="4bf61-115">followupFlagStatus values</span></span>|<span data-ttu-id="4bf61-116">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="4bf61-116">The status for follow-up for an item.</span></span> <span data-ttu-id="4bf61-117">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="4bf61-117">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="4bf61-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4bf61-118">startDateTime</span></span>|<span data-ttu-id="4bf61-119">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="4bf61-119">**dateTimeTimeZone**</span></span>|<span data-ttu-id="4bf61-120">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="4bf61-120">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4bf61-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4bf61-121">JSON representation</span></span>

<span data-ttu-id="4bf61-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bf61-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
