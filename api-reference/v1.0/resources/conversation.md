# <a name="conversation-resource-type"></a><span data-ttu-id="94414-101">Тип ресурса conversation</span><span class="sxs-lookup"><span data-stu-id="94414-101">conversation resource type</span></span>

<span data-ttu-id="94414-p101">Беседа — коллекция [цепочек](conversationthread.md), содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.</span><span class="sxs-lookup"><span data-stu-id="94414-p101">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

## <a name="methods"></a><span data-ttu-id="94414-104">Методы</span><span class="sxs-lookup"><span data-stu-id="94414-104">Methods</span></span>

| <span data-ttu-id="94414-105">Метод</span><span class="sxs-lookup"><span data-stu-id="94414-105">Method</span></span>       | <span data-ttu-id="94414-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="94414-106">Return Type</span></span>  |<span data-ttu-id="94414-107">Описание</span><span class="sxs-lookup"><span data-stu-id="94414-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94414-108">Список бесед</span><span class="sxs-lookup"><span data-stu-id="94414-108">List conversations</span></span>](../api/group_list_conversations.md) | <span data-ttu-id="94414-109">Коллекция [conversation](conversation.md)</span><span class="sxs-lookup"><span data-stu-id="94414-109">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="94414-110">Получение списка бесед в этой группе.</span><span class="sxs-lookup"><span data-stu-id="94414-110">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="94414-111">Создание</span><span class="sxs-lookup"><span data-stu-id="94414-111">Create</span></span>](../api/group_post_conversations.md) |[<span data-ttu-id="94414-112">conversation</span><span class="sxs-lookup"><span data-stu-id="94414-112">conversation</span></span>](conversation.md)| <span data-ttu-id="94414-113">Создание беседы путем включения цепочки и записи.</span><span class="sxs-lookup"><span data-stu-id="94414-113">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="94414-114">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="94414-114">Get conversation</span></span>](../api/conversation_get.md) | [<span data-ttu-id="94414-115">conversation</span><span class="sxs-lookup"><span data-stu-id="94414-115">conversation</span></span>](conversation.md) |<span data-ttu-id="94414-116">Считывание свойств и отношений объекта conversation.</span><span class="sxs-lookup"><span data-stu-id="94414-116">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="94414-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="94414-117">Delete</span></span>](../api/conversation_delete.md) | <span data-ttu-id="94414-118">Нет</span><span class="sxs-lookup"><span data-stu-id="94414-118">None</span></span> |<span data-ttu-id="94414-119">Удаление объекта conversation.</span><span class="sxs-lookup"><span data-stu-id="94414-119">Delete conversation object.</span></span> |
|[<span data-ttu-id="94414-120">Список цепочек беседы</span><span class="sxs-lookup"><span data-stu-id="94414-120">List conversation threads</span></span>](../api/conversation_list_threads.md) |<span data-ttu-id="94414-121">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="94414-121">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="94414-122">Получение всех цепочек в групповой беседе.</span><span class="sxs-lookup"><span data-stu-id="94414-122">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="94414-123">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="94414-123">Create conversation thread</span></span>](../api/conversation_post_threads.md) |<span data-ttu-id="94414-124">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="94414-124">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="94414-125">Создание цепочки в указанной беседе.</span><span class="sxs-lookup"><span data-stu-id="94414-125">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="94414-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="94414-126">Properties</span></span>
| <span data-ttu-id="94414-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="94414-127">Property</span></span>     | <span data-ttu-id="94414-128">Тип</span><span class="sxs-lookup"><span data-stu-id="94414-128">Type</span></span>   |<span data-ttu-id="94414-129">Описание</span><span class="sxs-lookup"><span data-stu-id="94414-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94414-130">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="94414-130">hasAttachments</span></span>|<span data-ttu-id="94414-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="94414-131">Boolean</span></span>|<span data-ttu-id="94414-132">Указывает, содержит ли какая-либо запись в этой беседе хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="94414-132">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="94414-133">id</span><span class="sxs-lookup"><span data-stu-id="94414-133">id</span></span>|<span data-ttu-id="94414-134">String</span><span class="sxs-lookup"><span data-stu-id="94414-134">String</span></span>|<span data-ttu-id="94414-p102">Уникальный идентификатор беседы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94414-p102">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="94414-137">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="94414-137">lastDeliveredDateTime</span></span>|<span data-ttu-id="94414-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94414-138">DateTimeOffset</span></span>|<span data-ttu-id="94414-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="94414-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="94414-141">preview</span><span class="sxs-lookup"><span data-stu-id="94414-141">preview</span></span>|<span data-ttu-id="94414-142">String</span><span class="sxs-lookup"><span data-stu-id="94414-142">String</span></span>|<span data-ttu-id="94414-143">Краткая сводка из текста последней записи в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="94414-143">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="94414-144">topic</span><span class="sxs-lookup"><span data-stu-id="94414-144">topic</span></span>|<span data-ttu-id="94414-145">String</span><span class="sxs-lookup"><span data-stu-id="94414-145">String</span></span>|<span data-ttu-id="94414-p104">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="94414-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="94414-148">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="94414-148">uniqueSenders</span></span>|<span data-ttu-id="94414-149">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="94414-149">String collection</span></span>|<span data-ttu-id="94414-150">Все пользователи, которые отправили сообщение в эту беседу.</span><span class="sxs-lookup"><span data-stu-id="94414-150">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94414-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="94414-151">Relationships</span></span>
| <span data-ttu-id="94414-152">Связь</span><span class="sxs-lookup"><span data-stu-id="94414-152">Relationship</span></span> | <span data-ttu-id="94414-153">Тип</span><span class="sxs-lookup"><span data-stu-id="94414-153">Type</span></span>   |<span data-ttu-id="94414-154">Описание</span><span class="sxs-lookup"><span data-stu-id="94414-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94414-155">threads</span><span class="sxs-lookup"><span data-stu-id="94414-155">threads</span></span>|<span data-ttu-id="94414-156">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="94414-156">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="94414-p105">Коллекция всех цепочек в беседе. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="94414-p105">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94414-161">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="94414-161">JSON representation</span></span>

<span data-ttu-id="94414-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94414-162">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
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
