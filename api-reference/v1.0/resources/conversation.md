# <a name="conversation-resource-type"></a><span data-ttu-id="c656e-101">Тип ресурса conversation</span><span class="sxs-lookup"><span data-stu-id="c656e-101">conversation resource type</span></span>

<span data-ttu-id="c656e-p101">Беседа — коллекция [цепочек](conversationthread.md), содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.</span><span class="sxs-lookup"><span data-stu-id="c656e-p101">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="c656e-104">Этот ресурс поддерживает подписку на [уведомления об изменении](../../../concepts/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="c656e-104">This resource supports subscribing to [change notifications](../../../concepts/webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c656e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c656e-105">Methods</span></span>

| <span data-ttu-id="c656e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="c656e-106">Method</span></span>       | <span data-ttu-id="c656e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c656e-107">Return Type</span></span>  |<span data-ttu-id="c656e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c656e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c656e-109">Список бесед</span><span class="sxs-lookup"><span data-stu-id="c656e-109">List conversations</span></span>](../api/group_list_conversations.md) | <span data-ttu-id="c656e-110">Коллекция [conversation](conversation.md)</span><span class="sxs-lookup"><span data-stu-id="c656e-110">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="c656e-111">Получение списка бесед в этой группе.</span><span class="sxs-lookup"><span data-stu-id="c656e-111">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="c656e-112">Создание</span><span class="sxs-lookup"><span data-stu-id="c656e-112">Create</span></span>](../api/group_post_conversations.md) |[<span data-ttu-id="c656e-113">conversation</span><span class="sxs-lookup"><span data-stu-id="c656e-113">conversation</span></span>](conversation.md)| <span data-ttu-id="c656e-114">Создание беседы путем включения цепочки и записи.</span><span class="sxs-lookup"><span data-stu-id="c656e-114">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="c656e-115">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="c656e-115">Get conversation</span></span>](../api/conversation_get.md) | [<span data-ttu-id="c656e-116">conversation</span><span class="sxs-lookup"><span data-stu-id="c656e-116">conversation</span></span>](conversation.md) |<span data-ttu-id="c656e-117">Считывание свойств и отношений объекта conversation.</span><span class="sxs-lookup"><span data-stu-id="c656e-117">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="c656e-118">Удаление</span><span class="sxs-lookup"><span data-stu-id="c656e-118">Delete</span></span>](../api/conversation_delete.md) | <span data-ttu-id="c656e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c656e-119">None</span></span> |<span data-ttu-id="c656e-120">Удаление объекта conversation.</span><span class="sxs-lookup"><span data-stu-id="c656e-120">Delete conversation object.</span></span> |
|[<span data-ttu-id="c656e-121">Список цепочек беседы</span><span class="sxs-lookup"><span data-stu-id="c656e-121">List conversation threads</span></span>](../api/conversation_list_threads.md) |<span data-ttu-id="c656e-122">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c656e-122">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="c656e-123">Получение всех цепочек в групповой беседе.</span><span class="sxs-lookup"><span data-stu-id="c656e-123">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="c656e-124">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="c656e-124">Create conversation thread</span></span>](../api/conversation_post_threads.md) |<span data-ttu-id="c656e-125">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c656e-125">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="c656e-126">Создание цепочки в указанной беседе.</span><span class="sxs-lookup"><span data-stu-id="c656e-126">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="c656e-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="c656e-127">Properties</span></span>
| <span data-ttu-id="c656e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c656e-128">Property</span></span>     | <span data-ttu-id="c656e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c656e-129">Type</span></span>   |<span data-ttu-id="c656e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c656e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c656e-131">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="c656e-131">hasAttachments</span></span>|<span data-ttu-id="c656e-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656e-132">Boolean</span></span>|<span data-ttu-id="c656e-133">Указывает, содержит ли какая-либо запись в этой беседе хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="c656e-133">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="c656e-134">id</span><span class="sxs-lookup"><span data-stu-id="c656e-134">id</span></span>|<span data-ttu-id="c656e-135">Строка</span><span class="sxs-lookup"><span data-stu-id="c656e-135">String</span></span>|<span data-ttu-id="c656e-p102">Уникальный идентификатор беседы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c656e-p102">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="c656e-138">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="c656e-138">lastDeliveredDateTime</span></span>|<span data-ttu-id="c656e-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c656e-139">DateTimeOffset</span></span>|<span data-ttu-id="c656e-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c656e-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c656e-142">предварительная версия</span><span class="sxs-lookup"><span data-stu-id="c656e-142">preview</span></span>|<span data-ttu-id="c656e-143">Строка</span><span class="sxs-lookup"><span data-stu-id="c656e-143">String</span></span>|<span data-ttu-id="c656e-144">Краткая сводка из текста последней записи в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="c656e-144">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="c656e-145">topic</span><span class="sxs-lookup"><span data-stu-id="c656e-145">topic</span></span>|<span data-ttu-id="c656e-146">Строка</span><span class="sxs-lookup"><span data-stu-id="c656e-146">String</span></span>|<span data-ttu-id="c656e-p104">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="c656e-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="c656e-149">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="c656e-149">uniqueSenders</span></span>|<span data-ttu-id="c656e-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c656e-150">String collection</span></span>|<span data-ttu-id="c656e-151">Все пользователи, которые отправили сообщение в эту беседу.</span><span class="sxs-lookup"><span data-stu-id="c656e-151">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c656e-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="c656e-152">Relationships</span></span>
| <span data-ttu-id="c656e-153">Связь</span><span class="sxs-lookup"><span data-stu-id="c656e-153">Relationship</span></span> | <span data-ttu-id="c656e-154">Тип</span><span class="sxs-lookup"><span data-stu-id="c656e-154">Type</span></span>   |<span data-ttu-id="c656e-155">Описание</span><span class="sxs-lookup"><span data-stu-id="c656e-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c656e-156">threads</span><span class="sxs-lookup"><span data-stu-id="c656e-156">threads</span></span>|<span data-ttu-id="c656e-157">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c656e-157">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="c656e-p105">Коллекция всех цепочек в беседе. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c656e-p105">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c656e-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c656e-162">JSON representation</span></span>

<span data-ttu-id="c656e-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c656e-163">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversation",
  "@odata.annotations": [
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"],

  "threads": [{"@odata.type": "microsoft.graph.conversationThread"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
