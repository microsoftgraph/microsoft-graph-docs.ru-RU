---
title: Тип ресурса Post
description: Представляет отдельный элемент Post в сущности conversationThread.
author: dkershaw10
ms.openlocfilehash: dcbf62d5415273ebd805fc930c746282519f386a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340042"
---
# <a name="post-resource-type"></a><span data-ttu-id="02c67-103">Тип ресурса Post</span><span class="sxs-lookup"><span data-stu-id="02c67-103">post resource type</span></span>
<span data-ttu-id="02c67-104">Представляет отдельный элемент Post в сущности [conversationThread](conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="02c67-104">Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="02c67-105">Хотя явно создать экземпляр post невозможно, он будет создан в результате выполнения любого из указанных ниже действий.</span><span class="sxs-lookup"><span data-stu-id="02c67-105">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- <span data-ttu-id="02c67-106">[Добавление ответа к существующей публикации](../api/post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="02c67-106">[Reply to an existing post](../api/post-reply.md)</span></span> 
- <span data-ttu-id="02c67-107">[Добавление ответа к существующей цепочке](../api/conversationthread-reply.md).</span><span class="sxs-lookup"><span data-stu-id="02c67-107">[Reply to an existing thread](../api/conversationthread-reply.md)</span></span> 
- <span data-ttu-id="02c67-108">[Создание цепочки в новой беседе](../api/group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="02c67-108">[Create a thread in a new conversation](../api/group-post-threads.md)</span></span>
- [<span data-ttu-id="02c67-109">Создание беседы</span><span class="sxs-lookup"><span data-stu-id="02c67-109">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="02c67-110">С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="02c67-110">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="02c67-111">Методы</span><span class="sxs-lookup"><span data-stu-id="02c67-111">Methods</span></span>

| <span data-ttu-id="02c67-112">Метод</span><span class="sxs-lookup"><span data-stu-id="02c67-112">Method</span></span>       | <span data-ttu-id="02c67-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="02c67-113">Return Type</span></span>  |<span data-ttu-id="02c67-114">Описание</span><span class="sxs-lookup"><span data-stu-id="02c67-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02c67-115">Вывод списка публикаций</span><span class="sxs-lookup"><span data-stu-id="02c67-115">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="02c67-116">post</span><span class="sxs-lookup"><span data-stu-id="02c67-116">post</span></span>](post.md) |<span data-ttu-id="02c67-117">Получение публикаций из указанной цепочки.</span><span class="sxs-lookup"><span data-stu-id="02c67-117">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="02c67-118">Получение публикации</span><span class="sxs-lookup"><span data-stu-id="02c67-118">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="02c67-119">post</span><span class="sxs-lookup"><span data-stu-id="02c67-119">post</span></span>](post.md) |<span data-ttu-id="02c67-120">Получение свойств и связей публикации в указанной цепочке.</span><span class="sxs-lookup"><span data-stu-id="02c67-120">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="02c67-121">Ответ</span><span class="sxs-lookup"><span data-stu-id="02c67-121">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="02c67-122">Нет</span><span class="sxs-lookup"><span data-stu-id="02c67-122">None</span></span>|<span data-ttu-id="02c67-123">Ответ на публикацию и добавление новой публикации в указанную цепочку беседы группы.</span><span class="sxs-lookup"><span data-stu-id="02c67-123">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="02c67-124">Переадресация</span><span class="sxs-lookup"><span data-stu-id="02c67-124">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="02c67-125">Нет</span><span class="sxs-lookup"><span data-stu-id="02c67-125">None</span></span>|<span data-ttu-id="02c67-126">Переадресация публикации получателю.</span><span class="sxs-lookup"><span data-stu-id="02c67-126">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="02c67-127">**Вложения**</span><span class="sxs-lookup"><span data-stu-id="02c67-127">**Attachments**</span></span>| | |
|[<span data-ttu-id="02c67-128">Список вложений</span><span class="sxs-lookup"><span data-stu-id="02c67-128">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="02c67-129">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="02c67-129">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="02c67-130">Получает все вложения для экземпляра post.</span><span class="sxs-lookup"><span data-stu-id="02c67-130">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="02c67-131">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="02c67-131">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="02c67-132">attachment</span><span class="sxs-lookup"><span data-stu-id="02c67-132">attachment</span></span>](attachment.md)| <span data-ttu-id="02c67-133">Добавление вложения в публикацию.</span><span class="sxs-lookup"><span data-stu-id="02c67-133">Add an attachment to a post.</span></span> |
|<span data-ttu-id="02c67-134">**Открытые расширения**</span><span class="sxs-lookup"><span data-stu-id="02c67-134">**Open extensions**</span></span>| | |
|[<span data-ttu-id="02c67-135">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="02c67-135">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="02c67-136">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="02c67-136">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="02c67-137">Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="02c67-137">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="02c67-138">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="02c67-138">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="02c67-139">Коллекция [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="02c67-139">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="02c67-140">Получение объектов открытого расширения, которые определяются по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="02c67-140">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="02c67-141">**Расширения схемы**</span><span class="sxs-lookup"><span data-stu-id="02c67-141">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="02c67-142">Добавление значений расширений для схемы</span><span class="sxs-lookup"><span data-stu-id="02c67-142">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="02c67-143">Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="02c67-143">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="02c67-144">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="02c67-144">**Extended properties**</span></span>| | |
|[<span data-ttu-id="02c67-145">Создание однозначного расширенного свойства</span><span class="sxs-lookup"><span data-stu-id="02c67-145">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="02c67-146">post</span><span class="sxs-lookup"><span data-stu-id="02c67-146">post</span></span>](post.md)  |<span data-ttu-id="02c67-147">Создание одного или нескольких расширенных свойств с одним значением в новой или существующей публикации.</span><span class="sxs-lookup"><span data-stu-id="02c67-147">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="02c67-148">Получение публикации с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="02c67-148">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="02c67-149">post</span><span class="sxs-lookup"><span data-stu-id="02c67-149">post</span></span>](post.md) | <span data-ttu-id="02c67-150">Получение публикаций, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="02c67-150">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="02c67-151">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="02c67-151">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="02c67-152">post</span><span class="sxs-lookup"><span data-stu-id="02c67-152">post</span></span>](post.md) | <span data-ttu-id="02c67-153">Создание одного или нескольких расширенных свойств с несколькими значениями в новой или существующей публикации.</span><span class="sxs-lookup"><span data-stu-id="02c67-153">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="02c67-154">Получение публикации с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="02c67-154">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="02c67-155">post</span><span class="sxs-lookup"><span data-stu-id="02c67-155">post</span></span>](post.md) | <span data-ttu-id="02c67-156">Получение публикации, которая содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="02c67-156">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="02c67-157">Свойства</span><span class="sxs-lookup"><span data-stu-id="02c67-157">Properties</span></span>
| <span data-ttu-id="02c67-158">Свойство</span><span class="sxs-lookup"><span data-stu-id="02c67-158">Property</span></span>     | <span data-ttu-id="02c67-159">Тип</span><span class="sxs-lookup"><span data-stu-id="02c67-159">Type</span></span>   |<span data-ttu-id="02c67-160">Описание</span><span class="sxs-lookup"><span data-stu-id="02c67-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02c67-161">Основной текст</span><span class="sxs-lookup"><span data-stu-id="02c67-161">body</span></span>|[<span data-ttu-id="02c67-162">itemBody</span><span class="sxs-lookup"><span data-stu-id="02c67-162">itemBody</span></span>](itembody.md)|<span data-ttu-id="02c67-p101">Содержимое публикации. Это свойство используется по умолчанию. Это свойство может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="02c67-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="02c67-166">categories</span><span class="sxs-lookup"><span data-stu-id="02c67-166">categories</span></span>|<span data-ttu-id="02c67-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="02c67-167">String collection</span></span>|<span data-ttu-id="02c67-168">Категории, сопоставленные с публикацией.</span><span class="sxs-lookup"><span data-stu-id="02c67-168">The categories associated with the post.</span></span>|
|<span data-ttu-id="02c67-169">changeKey</span><span class="sxs-lookup"><span data-stu-id="02c67-169">changeKey</span></span>|<span data-ttu-id="02c67-170">Строка</span><span class="sxs-lookup"><span data-stu-id="02c67-170">String</span></span>|<span data-ttu-id="02c67-p102">Указывает версию публикации. При каждом изменении публикации также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="02c67-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="02c67-174">conversationId</span><span class="sxs-lookup"><span data-stu-id="02c67-174">conversationId</span></span>|<span data-ttu-id="02c67-175">Строка</span><span class="sxs-lookup"><span data-stu-id="02c67-175">String</span></span>|<span data-ttu-id="02c67-p103">Уникальный идентификатор беседы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="02c67-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="02c67-178">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="02c67-178">conversationThreadId</span></span>|<span data-ttu-id="02c67-179">Строка</span><span class="sxs-lookup"><span data-stu-id="02c67-179">String</span></span>|<span data-ttu-id="02c67-p104">Уникальный идентификатор цепочки беседы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="02c67-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="02c67-182">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02c67-182">createdDateTime</span></span>|<span data-ttu-id="02c67-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02c67-183">DateTimeOffset</span></span>|<span data-ttu-id="02c67-p105">Указывает, когда была создана публикация. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="02c67-p105">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="02c67-187">from</span><span class="sxs-lookup"><span data-stu-id="02c67-187">from</span></span>|[<span data-ttu-id="02c67-188">recipient</span><span class="sxs-lookup"><span data-stu-id="02c67-188">recipient</span></span>](recipient.md)|<span data-ttu-id="02c67-p106">Используется в сценариях делегированного доступа. Указывает, кто опубликовал сообщение от имени другого пользователя. Это свойство используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="02c67-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="02c67-192">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="02c67-192">hasAttachments</span></span>|<span data-ttu-id="02c67-193">Логический</span><span class="sxs-lookup"><span data-stu-id="02c67-193">Boolean</span></span>|<span data-ttu-id="02c67-p107">Указывает, есть ли в публикации хотя бы одно вложение. Это свойство используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="02c67-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="02c67-196">id</span><span class="sxs-lookup"><span data-stu-id="02c67-196">id</span></span>|<span data-ttu-id="02c67-197">Строка</span><span class="sxs-lookup"><span data-stu-id="02c67-197">String</span></span>| <span data-ttu-id="02c67-198">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="02c67-198">Read-only.</span></span>|
|<span data-ttu-id="02c67-199">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02c67-199">lastModifiedDateTime</span></span>|<span data-ttu-id="02c67-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02c67-200">DateTimeOffset</span></span>|<span data-ttu-id="02c67-p108">Указывает дату и время последнего изменения публикации. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="02c67-p108">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="02c67-204">newParticipants</span><span class="sxs-lookup"><span data-stu-id="02c67-204">newParticipants</span></span>|<span data-ttu-id="02c67-205">Коллекция объектов [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="02c67-205">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="02c67-206">Участники беседы, которые были добавлены в цепочку в рамках этой публикации.</span><span class="sxs-lookup"><span data-stu-id="02c67-206">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="02c67-207">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="02c67-207">receivedDateTime</span></span>|<span data-ttu-id="02c67-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02c67-208">DateTimeOffset</span></span>|<span data-ttu-id="02c67-p109">Указывает, когда была получена публикация. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="02c67-p109">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="02c67-212">sender</span><span class="sxs-lookup"><span data-stu-id="02c67-212">sender</span></span>|[<span data-ttu-id="02c67-213">recipient</span><span class="sxs-lookup"><span data-stu-id="02c67-213">recipient</span></span>](recipient.md)|<span data-ttu-id="02c67-p110">Содержит электронный адрес отправителя. Если получатель не указан, то в качестве значения Sender используется адрес пользователя, прошедшего проверку подлинности. Это свойство используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="02c67-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02c67-217">Связи</span><span class="sxs-lookup"><span data-stu-id="02c67-217">Relationships</span></span>
| <span data-ttu-id="02c67-218">Связь</span><span class="sxs-lookup"><span data-stu-id="02c67-218">Relationship</span></span> | <span data-ttu-id="02c67-219">Тип</span><span class="sxs-lookup"><span data-stu-id="02c67-219">Type</span></span>   |<span data-ttu-id="02c67-220">Описание</span><span class="sxs-lookup"><span data-stu-id="02c67-220">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02c67-221">attachments</span><span class="sxs-lookup"><span data-stu-id="02c67-221">attachments</span></span>|<span data-ttu-id="02c67-222">Коллекция объектов [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="02c67-222">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="02c67-p111">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="02c67-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="02c67-225">extensions</span><span class="sxs-lookup"><span data-stu-id="02c67-225">extensions</span></span>|<span data-ttu-id="02c67-226">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="02c67-226">[Extension](extension.md) collection</span></span>|<span data-ttu-id="02c67-p112">Коллекция открытых расширений, определенных для публикации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="02c67-p112">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="02c67-230">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="02c67-230">inReplyTo</span></span>|[<span data-ttu-id="02c67-231">post</span><span class="sxs-lookup"><span data-stu-id="02c67-231">post</span></span>](post.md)| <span data-ttu-id="02c67-232">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="02c67-232">Read-only.</span></span>|
|<span data-ttu-id="02c67-233">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="02c67-233">multiValueExtendedProperties</span></span>|<span data-ttu-id="02c67-234">Коллекция объектов [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="02c67-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="02c67-p113">Коллекция расширенных свойств с несколькими значениями, определенных для публикации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="02c67-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="02c67-238">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="02c67-238">singleValueExtendedProperties</span></span>|<span data-ttu-id="02c67-239">Коллекция объектов [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="02c67-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="02c67-p114">Коллекция расширенных свойств с одним значением, определенных для публикации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="02c67-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02c67-243">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02c67-243">JSON representation</span></span>

<span data-ttu-id="02c67-244">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02c67-244">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="02c67-245">См. также</span><span class="sxs-lookup"><span data-stu-id="02c67-245">See also</span></span>

- [<span data-ttu-id="02c67-246">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="02c67-246">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="02c67-247">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="02c67-247">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="02c67-248">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="02c67-248">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
