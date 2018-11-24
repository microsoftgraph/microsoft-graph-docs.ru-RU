# <a name="followupflag-resource-type"></a><span data-ttu-id="e5f86-101">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="e5f86-101">followupFlag resource type</span></span>


<span data-ttu-id="e5f86-102">Позволяет флаг в элементе для пользователя к исполнению более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="e5f86-102">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="e5f86-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5f86-103">Properties</span></span>
| <span data-ttu-id="e5f86-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5f86-104">Property</span></span>     | <span data-ttu-id="e5f86-105">Тип</span><span class="sxs-lookup"><span data-stu-id="e5f86-105">Type</span></span>   |<span data-ttu-id="e5f86-106">Описание</span><span class="sxs-lookup"><span data-stu-id="e5f86-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5f86-107">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5f86-107">completedDateTime</span></span>|[<span data-ttu-id="e5f86-108">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e5f86-108">dateTimeTimeZone</span></span>](dateTimeTimeZone.md)|<span data-ttu-id="e5f86-109">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="e5f86-109">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="e5f86-110">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="e5f86-110">dueDateTime</span></span>|<span data-ttu-id="e5f86-111">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="e5f86-111">**dateTimeTimeZone**</span></span>|<span data-ttu-id="e5f86-112">Дата и время, когда выполнение должно быть завершено.</span><span class="sxs-lookup"><span data-stu-id="e5f86-112">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="e5f86-113">flagStatus</span><span class="sxs-lookup"><span data-stu-id="e5f86-113">flagStatus</span></span>|<span data-ttu-id="e5f86-114">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="e5f86-114">followupFlagStatus</span></span>|<span data-ttu-id="e5f86-115">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="e5f86-115">The status for follow-up for an item.</span></span> <span data-ttu-id="e5f86-116">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="e5f86-116">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="e5f86-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e5f86-117">startDateTime</span></span>|<span data-ttu-id="e5f86-118">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="e5f86-118">**dateTimeTimeZone**</span></span>|<span data-ttu-id="e5f86-119">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="e5f86-119">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5f86-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5f86-120">JSON representation</span></span>

<span data-ttu-id="e5f86-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5f86-121">Here is a JSON representation of the resource</span></span>

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
