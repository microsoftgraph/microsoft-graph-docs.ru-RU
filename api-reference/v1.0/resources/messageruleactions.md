# <a name="messageruleactions-resource-type"></a><span data-ttu-id="87678-101">Тип ресурса messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="87678-101">messageRuleActions resource type</span></span>


<span data-ttu-id="87678-102">Представляет набор действий, доступных для правила.</span><span class="sxs-lookup"><span data-stu-id="87678-102">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="87678-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="87678-103">Properties</span></span>
| <span data-ttu-id="87678-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="87678-104">Property</span></span>     | <span data-ttu-id="87678-105">Тип</span><span class="sxs-lookup"><span data-stu-id="87678-105">Type</span></span>   |<span data-ttu-id="87678-106">Описание</span><span class="sxs-lookup"><span data-stu-id="87678-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="87678-107">assignCategories</span><span class="sxs-lookup"><span data-stu-id="87678-107">assignCategories</span></span> | <span data-ttu-id="87678-108">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="87678-108">String collection</span></span> | <span data-ttu-id="87678-109">Список категорий, которые необходимо назначить сообщению.</span><span class="sxs-lookup"><span data-stu-id="87678-109">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="87678-110">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="87678-110">copyToFolder</span></span> | <span data-ttu-id="87678-111">String (строка)</span><span class="sxs-lookup"><span data-stu-id="87678-111">String</span></span> | <span data-ttu-id="87678-112">Идентификатор папки, в которую необходимо скопировать сообщение.</span><span class="sxs-lookup"><span data-stu-id="87678-112">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="87678-113">delete</span><span class="sxs-lookup"><span data-stu-id="87678-113">delete</span></span> | <span data-ttu-id="87678-114">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="87678-114">Boolean</span></span> | <span data-ttu-id="87678-115">Указывает, нужно ли перемещать сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="87678-115">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="87678-116">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="87678-116">forwardAsAttachmentTo</span></span> | <span data-ttu-id="87678-117">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="87678-117">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="87678-118">Электронные адреса получателей, которым необходимо переслать сообщение как вложение.</span><span class="sxs-lookup"><span data-stu-id="87678-118">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="87678-119">forwardTo</span><span class="sxs-lookup"><span data-stu-id="87678-119">forwardTo</span></span> | <span data-ttu-id="87678-120">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="87678-120">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="87678-121">Электронные адреса получателей, которым необходимо переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="87678-121">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="87678-122">markAsRead</span><span class="sxs-lookup"><span data-stu-id="87678-122">markAsRead</span></span> | <span data-ttu-id="87678-123">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="87678-123">Boolean</span></span> | <span data-ttu-id="87678-124">Указывает, необходимо ли отмечать сообщение как прочтенное.</span><span class="sxs-lookup"><span data-stu-id="87678-124">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="87678-125">markImportance</span><span class="sxs-lookup"><span data-stu-id="87678-125">markImportance</span></span> | <span data-ttu-id="87678-126">importance</span><span class="sxs-lookup"><span data-stu-id="87678-126">importance</span></span> | <span data-ttu-id="87678-127">Задает важность сообщения. Возможные значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="87678-127">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="87678-128">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="87678-128">moveToFolder</span></span> |  <span data-ttu-id="87678-129">String (строка)</span><span class="sxs-lookup"><span data-stu-id="87678-129">String</span></span>| <span data-ttu-id="87678-130">Идентификатор папки, в которую сообщение будет перемещено.</span><span class="sxs-lookup"><span data-stu-id="87678-130">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="87678-131">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="87678-131">permanentDelete</span></span> | <span data-ttu-id="87678-132">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="87678-132">Boolean</span></span> | <span data-ttu-id="87678-133">Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="87678-133">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="87678-134">redirectTo</span><span class="sxs-lookup"><span data-stu-id="87678-134">redirectTo</span></span> | <span data-ttu-id="87678-135">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="87678-135">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="87678-136">Электронные адреса, на которые должно быть перенаправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="87678-136">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="87678-137">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="87678-137">stopProcessingRules</span></span> | <span data-ttu-id="87678-138">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="87678-138">Boolean</span></span> | <span data-ttu-id="87678-139">Указывает, должны ли обрабатываться последующие правила.</span><span class="sxs-lookup"><span data-stu-id="87678-139">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87678-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87678-140">JSON representation</span></span>
<span data-ttu-id="87678-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87678-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->