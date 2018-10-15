# <a name="post-resource-type"></a><span data-ttu-id="5cbd0-101">Тип ресурса Post</span><span class="sxs-lookup"><span data-stu-id="5cbd0-101">post resource type</span></span>
<span data-ttu-id="5cbd0-102">Представляет отдельный элемент Post в сущности [conversationThread](conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="5cbd0-102">Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="5cbd0-103">Хотя явно создать экземпляр post невозможно, он будет создан в результате выполнения любого из указанных ниже действий.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-103">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- <span data-ttu-id="5cbd0-104">[[Добавление ответа к существующей публикации](../api/post_reply.md).](../api/post_reply.md)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-104">[Reply to an existing post](../api/post_reply.md)</span></span> 
- <span data-ttu-id="5cbd0-105">[[Добавление ответа к существующей цепочке](../api/conversationthread_reply.md).](../api/conversationthread_reply.md)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-105">[Reply to an existing thread](../api/conversationthread_reply.md)</span></span> 
- <span data-ttu-id="5cbd0-106">[[Создание цепочки в новой беседе](../api/group_post_threads.md).](../api/group_post_threads.md)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-106">[Create a thread in a new conversation](../api/group_post_threads.md)</span></span>
- [<span data-ttu-id="5cbd0-107">Создание беседы</span><span class="sxs-lookup"><span data-stu-id="5cbd0-107">Create a new conversation</span></span>](../api/group_post_conversations.md)

<span data-ttu-id="5cbd0-108">С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](../../../concepts/extensibility_overview.md).</span><span class="sxs-lookup"><span data-stu-id="5cbd0-108">This resource lets you add your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5cbd0-109">Методы</span><span class="sxs-lookup"><span data-stu-id="5cbd0-109">Methods</span></span>

| <span data-ttu-id="5cbd0-110">Метод</span><span class="sxs-lookup"><span data-stu-id="5cbd0-110">Method</span></span>       | <span data-ttu-id="5cbd0-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5cbd0-111">Return Type</span></span>  |<span data-ttu-id="5cbd0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5cbd0-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5cbd0-113">Вывод списка публикаций</span><span class="sxs-lookup"><span data-stu-id="5cbd0-113">List posts</span></span>](../api/conversationthread_list_posts.md) | [<span data-ttu-id="5cbd0-114">post</span><span class="sxs-lookup"><span data-stu-id="5cbd0-114">post</span></span>](post.md) |<span data-ttu-id="5cbd0-115">Получение публикаций из указанной цепочки.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-115">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="5cbd0-116">Получение публикации</span><span class="sxs-lookup"><span data-stu-id="5cbd0-116">Get post</span></span>](../api/post_get.md) | [<span data-ttu-id="5cbd0-117">post</span><span class="sxs-lookup"><span data-stu-id="5cbd0-117">post</span></span>](post.md) |<span data-ttu-id="5cbd0-118">Получение свойств и связей публикации в указанной цепочке.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-118">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="5cbd0-119">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cbd0-119">Reply</span></span>](../api/post_reply.md)|<span data-ttu-id="5cbd0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5cbd0-120">None</span></span>|<span data-ttu-id="5cbd0-121">Ответ на публикацию и добавление новой публикации в указанную цепочку беседы группы.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-121">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="5cbd0-122">Переадресация</span><span class="sxs-lookup"><span data-stu-id="5cbd0-122">Forward</span></span>](../api/post_forward.md)|<span data-ttu-id="5cbd0-123">Нет</span><span class="sxs-lookup"><span data-stu-id="5cbd0-123">None</span></span>|<span data-ttu-id="5cbd0-124">Переадресация публикации получателю.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-124">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="5cbd0-125">**Вложения**</span><span class="sxs-lookup"><span data-stu-id="5cbd0-125">**Attachments**</span></span>| | |
|[<span data-ttu-id="5cbd0-126">Список вложений</span><span class="sxs-lookup"><span data-stu-id="5cbd0-126">List attachments</span></span>](../api/post_list_attachments.md) |<span data-ttu-id="5cbd0-127">Коллекция [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-127">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="5cbd0-128">Получает все вложения для экземпляра post.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-128">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="5cbd0-129">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="5cbd0-129">Add attachment</span></span>](../api/post_post_attachments.md) |[<span data-ttu-id="5cbd0-130">attachment</span><span class="sxs-lookup"><span data-stu-id="5cbd0-130">attachment</span></span>](attachment.md)| <span data-ttu-id="5cbd0-131">Добавление вложения в публикацию.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-131">Add an attachment to a post.</span></span> |
|<span data-ttu-id="5cbd0-132">**Открытые расширения**</span><span class="sxs-lookup"><span data-stu-id="5cbd0-132">**Open extensions**</span></span>| | |
|[<span data-ttu-id="5cbd0-133">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="5cbd0-133">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="5cbd0-134">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="5cbd0-134">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="5cbd0-135">Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-135">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="5cbd0-136">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="5cbd0-136">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="5cbd0-137">Коллекция [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-137">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="5cbd0-138">Получение объектов открытого расширения, которые определяются по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-138">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="5cbd0-139">**Расширения схемы**</span><span class="sxs-lookup"><span data-stu-id="5cbd0-139">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="5cbd0-140">Добавление значений расширений для схемы</span><span class="sxs-lookup"><span data-stu-id="5cbd0-140">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="5cbd0-141">Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-141">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="5cbd0-142">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="5cbd0-142">**Extended properties**</span></span>| | |
|[<span data-ttu-id="5cbd0-143">Создание однозначного расширенного свойства</span><span class="sxs-lookup"><span data-stu-id="5cbd0-143">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="5cbd0-144">post</span><span class="sxs-lookup"><span data-stu-id="5cbd0-144">post</span></span>](post.md)  |<span data-ttu-id="5cbd0-145">Создание одного или нескольких расширенных свойств с одним значением в новой или существующей публикации.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-145">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="5cbd0-146">Получение публикации с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="5cbd0-146">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="5cbd0-147">post</span><span class="sxs-lookup"><span data-stu-id="5cbd0-147">post</span></span>](post.md) | <span data-ttu-id="5cbd0-148">Получение публикаций, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-148">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="5cbd0-149">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="5cbd0-149">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="5cbd0-150">post</span><span class="sxs-lookup"><span data-stu-id="5cbd0-150">post</span></span>](post.md) | <span data-ttu-id="5cbd0-151">Создание одного или нескольких расширенных свойств с несколькими значениями в новой или существующей публикации.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-151">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="5cbd0-152">Получение публикации с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="5cbd0-152">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="5cbd0-153">post</span><span class="sxs-lookup"><span data-stu-id="5cbd0-153">post</span></span>](post.md) | <span data-ttu-id="5cbd0-154">Получение публикации, которая содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-154">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="5cbd0-155">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cbd0-155">Properties</span></span>
| <span data-ttu-id="5cbd0-156">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cbd0-156">Property</span></span>     | <span data-ttu-id="5cbd0-157">Тип</span><span class="sxs-lookup"><span data-stu-id="5cbd0-157">Type</span></span>   |<span data-ttu-id="5cbd0-158">Описание</span><span class="sxs-lookup"><span data-stu-id="5cbd0-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cbd0-159">body</span><span class="sxs-lookup"><span data-stu-id="5cbd0-159">body</span></span>|[<span data-ttu-id="5cbd0-160">itemBody</span><span class="sxs-lookup"><span data-stu-id="5cbd0-160">itemBody</span></span>](itembody.md)|<span data-ttu-id="5cbd0-p101">Содержимое публикации. Это свойство используется по умолчанию. Это свойство может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="5cbd0-164">categories</span><span class="sxs-lookup"><span data-stu-id="5cbd0-164">categories</span></span>|<span data-ttu-id="5cbd0-165">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5cbd0-165">String collection</span></span>|<span data-ttu-id="5cbd0-166">Категории, сопоставленные с публикацией.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-166">The categories associated with the post.</span></span>|
|<span data-ttu-id="5cbd0-167">changeKey</span><span class="sxs-lookup"><span data-stu-id="5cbd0-167">changeKey</span></span>|<span data-ttu-id="5cbd0-168">String (строка)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-168">String</span></span>|<span data-ttu-id="5cbd0-p102">Указывает версию публикации. При каждом изменении публикации также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="5cbd0-172">conversationId</span><span class="sxs-lookup"><span data-stu-id="5cbd0-172">conversationId</span></span>|<span data-ttu-id="5cbd0-173">String (строка)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-173">String</span></span>|<span data-ttu-id="5cbd0-p103">Уникальный идентификатор беседы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="5cbd0-176">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="5cbd0-176">conversationThreadId</span></span>|<span data-ttu-id="5cbd0-177">String (строка)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-177">String</span></span>|<span data-ttu-id="5cbd0-p104">Уникальный идентификатор цепочки беседы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="5cbd0-180">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5cbd0-180">createdDateTime</span></span>|<span data-ttu-id="5cbd0-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cbd0-181">DateTimeOffset</span></span>|<span data-ttu-id="5cbd0-p105">Указывает, когда была создана публикация. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p105">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5cbd0-185">from</span><span class="sxs-lookup"><span data-stu-id="5cbd0-185">from</span></span>|[<span data-ttu-id="5cbd0-186">recipient</span><span class="sxs-lookup"><span data-stu-id="5cbd0-186">recipient</span></span>](recipient.md)|<span data-ttu-id="5cbd0-p106">Используется в сценариях делегированного доступа. Указывает, кто опубликовал сообщение от имени другого пользователя. Это свойство используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="5cbd0-190">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="5cbd0-190">hasAttachments</span></span>|<span data-ttu-id="5cbd0-191">Логический</span><span class="sxs-lookup"><span data-stu-id="5cbd0-191">Boolean</span></span>|<span data-ttu-id="5cbd0-p107">Указывает, есть ли в публикации хотя бы одно вложение. Это свойство используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="5cbd0-194">id</span><span class="sxs-lookup"><span data-stu-id="5cbd0-194">id</span></span>|<span data-ttu-id="5cbd0-195">String (строка)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-195">String</span></span>| <span data-ttu-id="5cbd0-196">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-196">Read-only.</span></span>|
|<span data-ttu-id="5cbd0-197">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cbd0-197">lastModifiedDateTime</span></span>|<span data-ttu-id="5cbd0-198">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cbd0-198">DateTimeOffset</span></span>|<span data-ttu-id="5cbd0-p108">Указывает дату и время последнего изменения публикации. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p108">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5cbd0-202">newParticipants</span><span class="sxs-lookup"><span data-stu-id="5cbd0-202">newParticipants</span></span>|<span data-ttu-id="5cbd0-203">Коллекция объектов [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-203">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="5cbd0-204">Участники беседы, которые были добавлены в цепочку в рамках этой публикации.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-204">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="5cbd0-205">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cbd0-205">receivedDateTime</span></span>|<span data-ttu-id="5cbd0-206">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cbd0-206">DateTimeOffset</span></span>|<span data-ttu-id="5cbd0-p109">Указывает, когда была получена публикация. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p109">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5cbd0-210">sender</span><span class="sxs-lookup"><span data-stu-id="5cbd0-210">sender</span></span>|[<span data-ttu-id="5cbd0-211">recipient</span><span class="sxs-lookup"><span data-stu-id="5cbd0-211">recipient</span></span>](recipient.md)|<span data-ttu-id="5cbd0-p110">Содержит электронный адрес отправителя. Если получатель не указан, то в качестве значения Sender используется адрес пользователя, прошедшего проверку подлинности. Это свойство используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cbd0-215">Связи</span><span class="sxs-lookup"><span data-stu-id="5cbd0-215">Relationships</span></span>
| <span data-ttu-id="5cbd0-216">Связь</span><span class="sxs-lookup"><span data-stu-id="5cbd0-216">Relationship</span></span> | <span data-ttu-id="5cbd0-217">Тип</span><span class="sxs-lookup"><span data-stu-id="5cbd0-217">Type</span></span>   |<span data-ttu-id="5cbd0-218">Описание</span><span class="sxs-lookup"><span data-stu-id="5cbd0-218">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cbd0-219">attachments</span><span class="sxs-lookup"><span data-stu-id="5cbd0-219">attachments</span></span>|<span data-ttu-id="5cbd0-220">Коллекция объектов [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-220">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="5cbd0-p111">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="5cbd0-223">extensions</span><span class="sxs-lookup"><span data-stu-id="5cbd0-223">extensions</span></span>|<span data-ttu-id="5cbd0-224">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-224">[Extension](extension.md) collection</span></span>|<span data-ttu-id="5cbd0-p112">Коллекция открытых расширений, определенных для публикации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p112">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="5cbd0-228">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="5cbd0-228">inReplyTo</span></span>|[<span data-ttu-id="5cbd0-229">post</span><span class="sxs-lookup"><span data-stu-id="5cbd0-229">post</span></span>](post.md)| <span data-ttu-id="5cbd0-230">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-230">Read-only.</span></span>|
|<span data-ttu-id="5cbd0-231">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="5cbd0-231">multiValueExtendedProperties</span></span>|<span data-ttu-id="5cbd0-232">Коллекция объектов [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-232">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="5cbd0-p113">Коллекция расширенных свойств с несколькими значениями, определенных для публикации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="5cbd0-236">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="5cbd0-236">singleValueExtendedProperties</span></span>|<span data-ttu-id="5cbd0-237">Коллекция объектов [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="5cbd0-237">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="5cbd0-p114">Коллекция расширенных свойств с одним значением, определенных для публикации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5cbd0-241">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cbd0-241">JSON representation</span></span>

<span data-ttu-id="5cbd0-242">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cbd0-242">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.post",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "inReplyTo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a><span data-ttu-id="5cbd0-243">См. также</span><span class="sxs-lookup"><span data-stu-id="5cbd0-243">See also</span></span>

- [<span data-ttu-id="5cbd0-244">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="5cbd0-244">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="5cbd0-245">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="5cbd0-245">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="5cbd0-246">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="5cbd0-246">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
