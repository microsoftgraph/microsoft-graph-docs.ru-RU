# <a name="conversationthread-resource-type"></a><span data-ttu-id="5574f-101">Тип ресурса conversationThread</span><span class="sxs-lookup"><span data-stu-id="5574f-101">conversationThread resource type</span></span>
<span data-ttu-id="5574f-102">conversationThread — это коллекция экземпляров [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="5574f-102">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="5574f-p101">Коллекция получателей последней записи — это все получатели для цепочки. Коллекция получателей для цепочки может увеличиваться. При удалении получателя из цепочки создается новая цепочка.</span><span class="sxs-lookup"><span data-stu-id="5574f-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="5574f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5574f-106">Methods</span></span>

| <span data-ttu-id="5574f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5574f-107">Method</span></span>       | <span data-ttu-id="5574f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5574f-108">Return Type</span></span>  |<span data-ttu-id="5574f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5574f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5574f-110">Список цепочек бесед</span><span class="sxs-lookup"><span data-stu-id="5574f-110">List threads</span></span>](../api/group_list_threads.md) | <span data-ttu-id="5574f-111">Коллекция [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="5574f-111">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="5574f-112">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="5574f-112">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="5574f-113">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="5574f-113">Create thread</span></span>](../api/group_post_threads.md) | [<span data-ttu-id="5574f-114">conversationThread</span><span class="sxs-lookup"><span data-stu-id="5574f-114">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="5574f-p102">Создание беседы путем создания цепочки. В группе создаются беседа, цепочка беседы и запись.</span><span class="sxs-lookup"><span data-stu-id="5574f-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="5574f-117">Получение conversationThread</span><span class="sxs-lookup"><span data-stu-id="5574f-117">Get conversationThread</span></span>](../api/conversationthread_get.md) | [<span data-ttu-id="5574f-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="5574f-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="5574f-119">Получение определенной цепочки, принадлежащей группе.</span><span class="sxs-lookup"><span data-stu-id="5574f-119">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="5574f-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="5574f-120">Update</span></span>](../api/conversationthread_update.md) | [<span data-ttu-id="5574f-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="5574f-121">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="5574f-122">Обновление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="5574f-122">Update conversationThread object.</span></span> |
|[<span data-ttu-id="5574f-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="5574f-123">Delete</span></span>](../api/conversationthread_delete.md) | <span data-ttu-id="5574f-124">Нет</span><span class="sxs-lookup"><span data-stu-id="5574f-124">None</span></span> |<span data-ttu-id="5574f-125">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="5574f-125">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="5574f-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="5574f-126">Reply</span></span>](../api/conversationthread_reply.md)|<span data-ttu-id="5574f-127">Нет</span><span class="sxs-lookup"><span data-stu-id="5574f-127">None</span></span>|<span data-ttu-id="5574f-128">Создание ответа для этой цепочки с помощью создания сущности Post.</span><span class="sxs-lookup"><span data-stu-id="5574f-128">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="5574f-129">Список сущностей Post</span><span class="sxs-lookup"><span data-stu-id="5574f-129">List Posts</span></span>](../api/conversationthread_list_posts.md) |<span data-ttu-id="5574f-130">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="5574f-130">[post](post.md) collection</span></span>| <span data-ttu-id="5574f-131">Получение записей для указанной цепочки.</span><span class="sxs-lookup"><span data-stu-id="5574f-131">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="5574f-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="5574f-132">Properties</span></span>
| <span data-ttu-id="5574f-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="5574f-133">Property</span></span>     | <span data-ttu-id="5574f-134">Тип</span><span class="sxs-lookup"><span data-stu-id="5574f-134">Type</span></span>   |<span data-ttu-id="5574f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5574f-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5574f-136">id</span><span class="sxs-lookup"><span data-stu-id="5574f-136">id</span></span>|<span data-ttu-id="5574f-137">String</span><span class="sxs-lookup"><span data-stu-id="5574f-137">String</span></span>| <span data-ttu-id="5574f-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5574f-138">Read-only.</span></span>|
|<span data-ttu-id="5574f-139">toRecipients</span><span class="sxs-lookup"><span data-stu-id="5574f-139">toRecipients</span></span>|<span data-ttu-id="5574f-140">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="5574f-140">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="5574f-141">Получатели в поле "Кому" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="5574f-141">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="5574f-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="5574f-142">ccRecipients</span></span>|<span data-ttu-id="5574f-143">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="5574f-143">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="5574f-144">Получатели в поле "Копия" для цепочки.</span><span class="sxs-lookup"><span data-stu-id="5574f-144">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="5574f-145">topic</span><span class="sxs-lookup"><span data-stu-id="5574f-145">topic</span></span>|<span data-ttu-id="5574f-146">String</span><span class="sxs-lookup"><span data-stu-id="5574f-146">String</span></span>|<span data-ttu-id="5574f-p103">Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="5574f-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="5574f-149">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="5574f-149">hasAttachments</span></span>|<span data-ttu-id="5574f-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="5574f-150">Boolean</span></span>|<span data-ttu-id="5574f-151">Указывает, содержит ли какая-либо запись в этой цепочке хотя бы одно вложение.</span><span class="sxs-lookup"><span data-stu-id="5574f-151">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="5574f-152">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="5574f-152">lastDeliveredDateTime</span></span>|<span data-ttu-id="5574f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5574f-153">DateTimeOffset</span></span>|<span data-ttu-id="5574f-p104">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5574f-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5574f-156">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="5574f-156">uniqueSenders</span></span>|<span data-ttu-id="5574f-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5574f-157">String collection</span></span>|<span data-ttu-id="5574f-158">Все пользователи, которые отправили сообщение в эту цепочку.</span><span class="sxs-lookup"><span data-stu-id="5574f-158">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="5574f-159">preview</span><span class="sxs-lookup"><span data-stu-id="5574f-159">preview</span></span>|<span data-ttu-id="5574f-160">String</span><span class="sxs-lookup"><span data-stu-id="5574f-160">String</span></span>|<span data-ttu-id="5574f-161">Краткая сводка из текста последней записи в этой беседе.</span><span class="sxs-lookup"><span data-stu-id="5574f-161">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="5574f-162">isLocked</span><span class="sxs-lookup"><span data-stu-id="5574f-162">isLocked</span></span>|<span data-ttu-id="5574f-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="5574f-163">Boolean</span></span>|<span data-ttu-id="5574f-164">Указывает, заблокирована ли цепочка.</span><span class="sxs-lookup"><span data-stu-id="5574f-164">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5574f-165">Отношения</span><span class="sxs-lookup"><span data-stu-id="5574f-165">Relationships</span></span>
| <span data-ttu-id="5574f-166">Связь</span><span class="sxs-lookup"><span data-stu-id="5574f-166">Relationship</span></span> | <span data-ttu-id="5574f-167">Тип</span><span class="sxs-lookup"><span data-stu-id="5574f-167">Type</span></span>   |<span data-ttu-id="5574f-168">Описание</span><span class="sxs-lookup"><span data-stu-id="5574f-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5574f-169">posts</span><span class="sxs-lookup"><span data-stu-id="5574f-169">posts</span></span>|<span data-ttu-id="5574f-170">Коллекция [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="5574f-170">[post](post.md) collection</span></span>| <span data-ttu-id="5574f-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5574f-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5574f-173">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5574f-173">JSON representation</span></span>

<span data-ttu-id="5574f-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5574f-174">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread"
}-->

```json
{
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": true,
  "id": "string (identifier)",
  "isLocked": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
