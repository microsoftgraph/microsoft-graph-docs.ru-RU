# <a name="messagerule-resource-type"></a><span data-ttu-id="0b0c4-101">Тип ресурса messageRule</span><span class="sxs-lookup"><span data-stu-id="0b0c4-101">messageRule resource type</span></span>


<span data-ttu-id="0b0c4-102">Правило, которое применяется к сообщениям в папке "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-102">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="0b0c4-103">В Outlook можно настроить правила для сообщений в папке "Входящие", согласно которым при соблюдении определенных условий выполняются нужные действия.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-103">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="0b0c4-104">Программным способом можно получить доступ к правилам, используя свойство навигации **messageRules** [папки](mailfolder.md) "Входящие".</span><span class="sxs-lookup"><span data-stu-id="0b0c4-104">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="0b0c4-105">Каждое правило определено ресурсом **messageRule**, доступные действия правил определяются сложным типом [messageRuleActions](messageruleactions.md), а доступные условия и исключения для правил — сложным типом [messageRulePredicates](messagerulepredicates.md).</span><span class="sxs-lookup"><span data-stu-id="0b0c4-105">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="0b0c4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b0c4-106">Properties</span></span>
| <span data-ttu-id="0b0c4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b0c4-107">Property</span></span>     | <span data-ttu-id="0b0c4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0b0c4-108">Type</span></span>   |<span data-ttu-id="0b0c4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0b0c4-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b0c4-110">actions</span><span class="sxs-lookup"><span data-stu-id="0b0c4-110">actions</span></span> | [<span data-ttu-id="0b0c4-111">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="0b0c4-111">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="0b0c4-112">Действия, которые нужно применить к сообщению при выполнении определенных условий.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-112">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="0b0c4-113">conditions</span><span class="sxs-lookup"><span data-stu-id="0b0c4-113">conditions</span></span> | [<span data-ttu-id="0b0c4-114">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="0b0c4-114">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="0b0c4-115">Условия, при соблюдении которых с указанным правилом выполняются соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-115">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="0b0c4-116">displayName</span><span class="sxs-lookup"><span data-stu-id="0b0c4-116">displayName</span></span> | <span data-ttu-id="0b0c4-117">String (строка)</span><span class="sxs-lookup"><span data-stu-id="0b0c4-117">String</span></span> | <span data-ttu-id="0b0c4-118">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-118">The display name of the rule.</span></span> |
| <span data-ttu-id="0b0c4-119">exceptions</span><span class="sxs-lookup"><span data-stu-id="0b0c4-119">exceptions</span></span> | [<span data-ttu-id="0b0c4-120">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="0b0c4-120">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="0b0c4-121">Условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-121">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="0b0c4-122">hasError</span><span class="sxs-lookup"><span data-stu-id="0b0c4-122">hasError</span></span> | <span data-ttu-id="0b0c4-123">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="0b0c4-123">Boolean</span></span> | <span data-ttu-id="0b0c4-124">Указывает, является ли правило ошибкой.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-124">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="0b0c4-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-125">Read-only.</span></span> |
| <span data-ttu-id="0b0c4-126">id</span><span class="sxs-lookup"><span data-stu-id="0b0c4-126">id</span></span> |<span data-ttu-id="0b0c4-127">String (строка)</span><span class="sxs-lookup"><span data-stu-id="0b0c4-127">String</span></span>|<span data-ttu-id="0b0c4-128">Уникальный идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-128">The unique identifier of the rule.</span></span> <span data-ttu-id="0b0c4-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-129">Read-only.</span></span>|
| <span data-ttu-id="0b0c4-130">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0b0c4-130">isEnabled</span></span> | <span data-ttu-id="0b0c4-131">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="0b0c4-131">Boolean</span></span> | <span data-ttu-id="0b0c4-132">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-132">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="0b0c4-133">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="0b0c4-133">isReadOnly</span></span> | <span data-ttu-id="0b0c4-134">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="0b0c4-134">Boolean</span></span> | <span data-ttu-id="0b0c4-135">Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-135">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="0b0c4-136">sequence</span><span class="sxs-lookup"><span data-stu-id="0b0c4-136">sequence</span></span> | <span data-ttu-id="0b0c4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0b0c4-137">Int32</span></span> | <span data-ttu-id="0b0c4-138">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-138">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="0b0c4-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b0c4-139">JSON representation</span></span>
<span data-ttu-id="0b0c4-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
   "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.messageRule"
}-->

```json
{
  "actions": {"@odata.type": "microsoft.graph.messageRuleActions"},
  "conditions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "displayName": "String",
  "exceptions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "hasError": "Boolean",
  "id": "String",
  "isEnabled": "Boolean",
  "isReadOnly": "Boolean",
  "sequence": "Int32"
}

```

## <a name="methods"></a><span data-ttu-id="0b0c4-141">Методы</span><span class="sxs-lookup"><span data-stu-id="0b0c4-141">Methods</span></span>
| <span data-ttu-id="0b0c4-142">Метод</span><span class="sxs-lookup"><span data-stu-id="0b0c4-142">Method</span></span>           | <span data-ttu-id="0b0c4-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0b0c4-143">Return Type</span></span>    |<span data-ttu-id="0b0c4-144">Описание</span><span class="sxs-lookup"><span data-stu-id="0b0c4-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b0c4-145">Список правил</span><span class="sxs-lookup"><span data-stu-id="0b0c4-145">List rules</span></span>](../api/mailfolder_list_messagerules.md) | <span data-ttu-id="0b0c4-146">Коллекция [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="0b0c4-146">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="0b0c4-147">Получает все объекты **messageRule**, определенные для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-147">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="0b0c4-148">Получение правила</span><span class="sxs-lookup"><span data-stu-id="0b0c4-148">Get rule</span></span>](../api/messagerule_get.md) | [<span data-ttu-id="0b0c4-149">messageRule</span><span class="sxs-lookup"><span data-stu-id="0b0c4-149">messageRule</span></span>](messagerule.md) |<span data-ttu-id="0b0c4-150">Считывает свойства и отношения объекта **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-150">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="0b0c4-151">Создание</span><span class="sxs-lookup"><span data-stu-id="0b0c4-151">Create</span></span>](../api/mailfolder_post_messagerules.md) | [<span data-ttu-id="0b0c4-152">messageRule</span><span class="sxs-lookup"><span data-stu-id="0b0c4-152">messageRule</span></span>](messagerule.md) |<span data-ttu-id="0b0c4-153">Создает объект **messageRule**, определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-153">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="0b0c4-154">Обновление</span><span class="sxs-lookup"><span data-stu-id="0b0c4-154">Update</span></span>](../api/messagerule_update.md) | [<span data-ttu-id="0b0c4-155">messageRule</span><span class="sxs-lookup"><span data-stu-id="0b0c4-155">messageRule</span></span>](messagerule.md) |<span data-ttu-id="0b0c4-156">Изменяет записываемые свойства объекта **messageRule** и сохраняет изменения.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-156">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="0b0c4-157">Удаление</span><span class="sxs-lookup"><span data-stu-id="0b0c4-157">Delete</span></span>](../api/messagerule_delete.md) | <span data-ttu-id="0b0c4-158">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="0b0c4-158">None</span></span> |<span data-ttu-id="0b0c4-159">Удаляет указанный объект **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="0b0c4-159">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->