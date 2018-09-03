# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="76600-101">Тип ресурса automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="76600-101">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="76600-102">Подсказки ([MailTips](../resources/mailtips.md)) об автоматических ответах, настроенных для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="76600-102">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="76600-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="76600-103">Properties</span></span>
| <span data-ttu-id="76600-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="76600-104">Property</span></span>     | <span data-ttu-id="76600-105">Тип</span><span class="sxs-lookup"><span data-stu-id="76600-105">Type</span></span>   |<span data-ttu-id="76600-106">Описание</span><span class="sxs-lookup"><span data-stu-id="76600-106">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="76600-107">message</span><span class="sxs-lookup"><span data-stu-id="76600-107">message</span></span> | <span data-ttu-id="76600-108">String (строка)</span><span class="sxs-lookup"><span data-stu-id="76600-108">String</span></span> | <span data-ttu-id="76600-109">Автоматическое ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="76600-109">The automatic reply message.</span></span> |
| <span data-ttu-id="76600-110">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="76600-110">messageLanguage</span></span> | [<span data-ttu-id="76600-111">localeInfo</span><span class="sxs-lookup"><span data-stu-id="76600-111">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="76600-112">Язык, на котором написано автоматическое ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="76600-112">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="76600-113">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="76600-113">scheduledEndTime</span></span> | [<span data-ttu-id="76600-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="76600-114">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="76600-115">Дата и время завершения отправки автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="76600-115">The date and time that automatic replies are set to end, if Status is set to .</span></span> |
| <span data-ttu-id="76600-116">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="76600-116">scheduledStartTime</span></span> | [<span data-ttu-id="76600-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="76600-117">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="76600-118">Дата и время начала действия автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="76600-118">The date and time that automatic replies are set to begin, if Status is set to .</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76600-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76600-119">JSON representation</span></span>

<span data-ttu-id="76600-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76600-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->