# <a name="messageruleactions-resource-type"></a><span data-ttu-id="fdc76-101">Тип ресурса messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="fdc76-101">messageRuleActions resource type</span></span>


<span data-ttu-id="fdc76-102">Представляет набор действий, доступных для правила.</span><span class="sxs-lookup"><span data-stu-id="fdc76-102">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="fdc76-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdc76-103">Properties</span></span>
| <span data-ttu-id="fdc76-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdc76-104">Property</span></span>     | <span data-ttu-id="fdc76-105">Тип</span><span class="sxs-lookup"><span data-stu-id="fdc76-105">Type</span></span>   |<span data-ttu-id="fdc76-106">Описание</span><span class="sxs-lookup"><span data-stu-id="fdc76-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fdc76-107">assignCategories</span><span class="sxs-lookup"><span data-stu-id="fdc76-107">assignCategories</span></span> | <span data-ttu-id="fdc76-108">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fdc76-108">String collection</span></span> | <span data-ttu-id="fdc76-109">Список категорий, которые необходимо назначить сообщению.</span><span class="sxs-lookup"><span data-stu-id="fdc76-109">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="fdc76-110">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="fdc76-110">copyToFolder</span></span> | <span data-ttu-id="fdc76-111">String</span><span class="sxs-lookup"><span data-stu-id="fdc76-111">String</span></span> | <span data-ttu-id="fdc76-112">Идентификатор папки, в которую необходимо скопировать сообщение.</span><span class="sxs-lookup"><span data-stu-id="fdc76-112">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="fdc76-113">delete</span><span class="sxs-lookup"><span data-stu-id="fdc76-113">delete</span></span> | <span data-ttu-id="fdc76-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc76-114">Boolean</span></span> | <span data-ttu-id="fdc76-115">Указывает, нужно ли перемещать сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="fdc76-115">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="fdc76-116">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="fdc76-116">forwardAsAttachmentTo</span></span> | <span data-ttu-id="fdc76-117">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="fdc76-117">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="fdc76-118">Электронные адреса получателей, которым необходимо переслать сообщение как вложение.</span><span class="sxs-lookup"><span data-stu-id="fdc76-118">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="fdc76-119">forwardTo</span><span class="sxs-lookup"><span data-stu-id="fdc76-119">forwardTo</span></span> | <span data-ttu-id="fdc76-120">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="fdc76-120">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="fdc76-121">Электронные адреса получателей, которым необходимо переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="fdc76-121">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="fdc76-122">markAsRead</span><span class="sxs-lookup"><span data-stu-id="fdc76-122">markAsRead</span></span> | <span data-ttu-id="fdc76-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc76-123">Boolean</span></span> | <span data-ttu-id="fdc76-124">Указывает, необходимо ли отмечать сообщение как прочтенное.</span><span class="sxs-lookup"><span data-stu-id="fdc76-124">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="fdc76-125">markImportance</span><span class="sxs-lookup"><span data-stu-id="fdc76-125">markImportance</span></span> | <span data-ttu-id="fdc76-126">String</span><span class="sxs-lookup"><span data-stu-id="fdc76-126">String</span></span> | <span data-ttu-id="fdc76-127">Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="fdc76-127">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="fdc76-128">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="fdc76-128">moveToFolder</span></span> |  <span data-ttu-id="fdc76-129">String</span><span class="sxs-lookup"><span data-stu-id="fdc76-129">String</span></span>| <span data-ttu-id="fdc76-130">Идентификатор папки, в которую сообщение будет перемещено.</span><span class="sxs-lookup"><span data-stu-id="fdc76-130">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="fdc76-131">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="fdc76-131">permanentDelete</span></span> | <span data-ttu-id="fdc76-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc76-132">Boolean</span></span> | <span data-ttu-id="fdc76-133">Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="fdc76-133">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="fdc76-134">redirectTo</span><span class="sxs-lookup"><span data-stu-id="fdc76-134">redirectTo</span></span> | [<span data-ttu-id="fdc76-135">recipient</span><span class="sxs-lookup"><span data-stu-id="fdc76-135">recipient</span></span>](recipient.md) | <span data-ttu-id="fdc76-136">Электронный адрес, на который должно быть перенаправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="fdc76-136">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="fdc76-137">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="fdc76-137">stopProcessingRules</span></span> | <span data-ttu-id="fdc76-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc76-138">Boolean</span></span> | <span data-ttu-id="fdc76-139">Указывает, должны ли обрабатываться последующие правила.</span><span class="sxs-lookup"><span data-stu-id="fdc76-139">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="fdc76-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdc76-140">JSON representation</span></span>
<span data-ttu-id="fdc76-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdc76-141">Here is a JSON representation of the resource.</span></span>

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
  "redirectTo": {"@odata.type": "microsoft.graph.recipient"},
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