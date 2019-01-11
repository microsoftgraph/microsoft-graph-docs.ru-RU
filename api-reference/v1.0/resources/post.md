---
title: Тип ресурса Post
description: Представляет отдельный элемент Post в сущности conversationThread.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 585d823a7a3e4b6814f06c1613cac66a82a93e65
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851193"
---
# <a name="post-resource-type"></a><span data-ttu-id="134f4-103">Тип ресурса Post</span><span class="sxs-lookup"><span data-stu-id="134f4-103">post resource type</span></span>
<span data-ttu-id="134f4-104">Представляет отдельный элемент Post в сущности [conversationThread](conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="134f4-104">Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="134f4-105">Хотя явно создать экземпляр post невозможно, он будет создан в результате выполнения любого из указанных ниже действий.</span><span class="sxs-lookup"><span data-stu-id="134f4-105">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- <span data-ttu-id="134f4-106">[Добавление ответа к существующей публикации](../api/post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="134f4-106">[Reply to an existing post](../api/post-reply.md)</span></span> 
- <span data-ttu-id="134f4-107">[Добавление ответа к существующей цепочке](../api/conversationthread-reply.md).</span><span class="sxs-lookup"><span data-stu-id="134f4-107">[Reply to an existing thread](../api/conversationthread-reply.md)</span></span> 
- <span data-ttu-id="134f4-108">[Создание цепочки в новой беседе](../api/group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="134f4-108">[Create a thread in a new conversation](../api/group-post-threads.md)</span></span>
- [<span data-ttu-id="134f4-109">Создание беседы</span><span class="sxs-lookup"><span data-stu-id="134f4-109">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="134f4-110">С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="134f4-110">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="134f4-111">Методы</span><span class="sxs-lookup"><span data-stu-id="134f4-111">Methods</span></span>

| <span data-ttu-id="134f4-112">Метод</span><span class="sxs-lookup"><span data-stu-id="134f4-112">Method</span></span>       | <span data-ttu-id="134f4-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="134f4-113">Return Type</span></span>  |<span data-ttu-id="134f4-114">Описание</span><span class="sxs-lookup"><span data-stu-id="134f4-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="134f4-115">Вывод списка публикаций</span><span class="sxs-lookup"><span data-stu-id="134f4-115">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="134f4-116">post</span><span class="sxs-lookup"><span data-stu-id="134f4-116">post</span></span>](post.md) |<span data-ttu-id="134f4-117">Получение публикаций из указанной цепочки.</span><span class="sxs-lookup"><span data-stu-id="134f4-117">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="134f4-118">Получение публикации</span><span class="sxs-lookup"><span data-stu-id="134f4-118">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="134f4-119">post</span><span class="sxs-lookup"><span data-stu-id="134f4-119">post</span></span>](post.md) |<span data-ttu-id="134f4-120">Получение свойств и связей публикации в указанной цепочке.</span><span class="sxs-lookup"><span data-stu-id="134f4-120">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="134f4-121">Ответ</span><span class="sxs-lookup"><span data-stu-id="134f4-121">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="134f4-122">Нет</span><span class="sxs-lookup"><span data-stu-id="134f4-122">None</span></span>|<span data-ttu-id="134f4-123">Ответ на публикацию и добавление новой публикации в указанную цепочку беседы группы.</span><span class="sxs-lookup"><span data-stu-id="134f4-123">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="134f4-124">Переадресация</span><span class="sxs-lookup"><span data-stu-id="134f4-124">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="134f4-125">Нет</span><span class="sxs-lookup"><span data-stu-id="134f4-125">None</span></span>|<span data-ttu-id="134f4-126">Переадресация публикации получателю.</span><span class="sxs-lookup"><span data-stu-id="134f4-126">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="134f4-127">**Вложения**</span><span class="sxs-lookup"><span data-stu-id="134f4-127">**Attachments**</span></span>| | |
|[<span data-ttu-id="134f4-128">Список вложений</span><span class="sxs-lookup"><span data-stu-id="134f4-128">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="134f4-129">Коллекция [attachment](attachment.md) </span><span class="sxs-lookup"><span data-stu-id="134f4-129">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="134f4-130">Получает все вложения для экземпляра post.</span><span class="sxs-lookup"><span data-stu-id="134f4-130">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="134f4-131">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="134f4-131">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="134f4-132">attachment</span><span class="sxs-lookup"><span data-stu-id="134f4-132">attachment</span></span>](attachment.md)| <span data-ttu-id="134f4-133">Добавление вложения в публикацию.</span><span class="sxs-lookup"><span data-stu-id="134f4-133">Add an attachment to a post.</span></span> |
|<span data-ttu-id="134f4-134">**Открытые расширения**</span><span class="sxs-lookup"><span data-stu-id="134f4-134">**Open extensions**</span></span>| | |
|[<span data-ttu-id="134f4-135">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="134f4-135">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="134f4-136">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="134f4-136">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="134f4-137">Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="134f4-137">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="134f4-138">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="134f4-138">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="134f4-139">Коллекция [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="134f4-139">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="134f4-140">Получение объектов открытого расширения, которые определяются по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="134f4-140">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="134f4-141">**Расширения схемы**</span><span class="sxs-lookup"><span data-stu-id="134f4-141">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="134f4-142">Добавление значений расширений для схемы</span><span class="sxs-lookup"><span data-stu-id="134f4-142">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="134f4-143">Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="134f4-143">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="134f4-144">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="134f4-144">**Extended properties**</span></span>| | |
|[<span data-ttu-id="134f4-145">Создание однозначного расширенного свойства</span><span class="sxs-lookup"><span data-stu-id="134f4-145">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="134f4-146">post</span><span class="sxs-lookup"><span data-stu-id="134f4-146">post</span></span>](post.md)  |<span data-ttu-id="134f4-147">Создание одного или нескольких расширенных свойств с одним значением в новой или существующей публикации.</span><span class="sxs-lookup"><span data-stu-id="134f4-147">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="134f4-148">Получение публикации с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="134f4-148">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="134f4-149">post</span><span class="sxs-lookup"><span data-stu-id="134f4-149">post</span></span>](post.md) | <span data-ttu-id="134f4-150">Получение публикаций, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="134f4-150">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="134f4-151">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="134f4-151">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="134f4-152">post</span><span class="sxs-lookup"><span data-stu-id="134f4-152">post</span></span>](post.md) | <span data-ttu-id="134f4-153">Создание одного или нескольких расширенных свойств с несколькими значениями в новой или существующей публикации.</span><span class="sxs-lookup"><span data-stu-id="134f4-153">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="134f4-154">Получение публикации с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="134f4-154">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="134f4-155">post</span><span class="sxs-lookup"><span data-stu-id="134f4-155">post</span></span>](post.md) | <span data-ttu-id="134f4-156">Получение публикации, которая содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="134f4-156">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="134f4-157">Свойства</span><span class="sxs-lookup"><span data-stu-id="134f4-157">Properties</span></span>
| <span data-ttu-id="134f4-158">Свойство</span><span class="sxs-lookup"><span data-stu-id="134f4-158">Property</span></span>     | <span data-ttu-id="134f4-159">Тип</span><span class="sxs-lookup"><span data-stu-id="134f4-159">Type</span></span>   |<span data-ttu-id="134f4-160">Описание</span><span class="sxs-lookup"><span data-stu-id="134f4-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="134f4-161">Основной текст</span><span class="sxs-lookup"><span data-stu-id="134f4-161">body</span></span>|[<span data-ttu-id="134f4-162">itemBody</span><span class="sxs-lookup"><span data-stu-id="134f4-162">itemBody</span></span>](itembody.md)|<span data-ttu-id="134f4-p101">Содержимое публикации. Это свойство используется по умолчанию. Это свойство может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="134f4-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="134f4-166">categories</span><span class="sxs-lookup"><span data-stu-id="134f4-166">categories</span></span>|<span data-ttu-id="134f4-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="134f4-167">String collection</span></span>|<span data-ttu-id="134f4-168">Категории, сопоставленные с публикацией.</span><span class="sxs-lookup"><span data-stu-id="134f4-168">The categories associated with the post.</span></span>|
|<span data-ttu-id="134f4-169">changeKey</span><span class="sxs-lookup"><span data-stu-id="134f4-169">changeKey</span></span>|<span data-ttu-id="134f4-170">Строка</span><span class="sxs-lookup"><span data-stu-id="134f4-170">String</span></span>|<span data-ttu-id="134f4-p102">Указывает версию публикации. При каждом изменении публикации также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="134f4-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="134f4-174">conversationId</span><span class="sxs-lookup"><span data-stu-id="134f4-174">conversationId</span></span>|<span data-ttu-id="134f4-175">Строка</span><span class="sxs-lookup"><span data-stu-id="134f4-175">String</span></span>|<span data-ttu-id="134f4-p103">Уникальный идентификатор беседы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="134f4-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="134f4-178">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="134f4-178">conversationThreadId</span></span>|<span data-ttu-id="134f4-179">Строка</span><span class="sxs-lookup"><span data-stu-id="134f4-179">String</span></span>|<span data-ttu-id="134f4-p104">Уникальный идентификатор цепочки беседы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="134f4-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="134f4-182">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="134f4-182">createdDateTime</span></span>|<span data-ttu-id="134f4-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="134f4-183">DateTimeOffset</span></span>|<span data-ttu-id="134f4-p105">Указывает, когда была создана публикация. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="134f4-p105">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="134f4-187">from</span><span class="sxs-lookup"><span data-stu-id="134f4-187">from</span></span>|[<span data-ttu-id="134f4-188">recipient</span><span class="sxs-lookup"><span data-stu-id="134f4-188">recipient</span></span>](recipient.md)|<span data-ttu-id="134f4-p106">Используется в сценариях делегированного доступа. Указывает, кто опубликовал сообщение от имени другого пользователя. Это свойство используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="134f4-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="134f4-192">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="134f4-192">hasAttachments</span></span>|<span data-ttu-id="134f4-193">Логический</span><span class="sxs-lookup"><span data-stu-id="134f4-193">Boolean</span></span>|<span data-ttu-id="134f4-p107">Указывает, есть ли в публикации хотя бы одно вложение. Это свойство используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="134f4-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="134f4-196">id</span><span class="sxs-lookup"><span data-stu-id="134f4-196">id</span></span>|<span data-ttu-id="134f4-197">Строка</span><span class="sxs-lookup"><span data-stu-id="134f4-197">String</span></span>| <span data-ttu-id="134f4-198">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="134f4-198">Read-only.</span></span>|
|<span data-ttu-id="134f4-199">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="134f4-199">lastModifiedDateTime</span></span>|<span data-ttu-id="134f4-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="134f4-200">DateTimeOffset</span></span>|<span data-ttu-id="134f4-p108">Указывает дату и время последнего изменения публикации. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="134f4-p108">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="134f4-204">newParticipants</span><span class="sxs-lookup"><span data-stu-id="134f4-204">newParticipants</span></span>|<span data-ttu-id="134f4-205">Коллекция объектов [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="134f4-205">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="134f4-206">Участники беседы, которые были добавлены в цепочку в рамках этой публикации.</span><span class="sxs-lookup"><span data-stu-id="134f4-206">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="134f4-207">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="134f4-207">receivedDateTime</span></span>|<span data-ttu-id="134f4-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="134f4-208">DateTimeOffset</span></span>|<span data-ttu-id="134f4-p109">Указывает, когда была получена публикация. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="134f4-p109">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="134f4-212">sender</span><span class="sxs-lookup"><span data-stu-id="134f4-212">sender</span></span>|[<span data-ttu-id="134f4-213">recipient</span><span class="sxs-lookup"><span data-stu-id="134f4-213">recipient</span></span>](recipient.md)|<span data-ttu-id="134f4-p110">Содержит электронный адрес отправителя. Если получатель не указан, то в качестве значения Sender используется адрес пользователя, прошедшего проверку подлинности. Это свойство используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="134f4-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="134f4-217">Связи</span><span class="sxs-lookup"><span data-stu-id="134f4-217">Relationships</span></span>
| <span data-ttu-id="134f4-218">Связь</span><span class="sxs-lookup"><span data-stu-id="134f4-218">Relationship</span></span> | <span data-ttu-id="134f4-219">Тип</span><span class="sxs-lookup"><span data-stu-id="134f4-219">Type</span></span>   |<span data-ttu-id="134f4-220">Описание</span><span class="sxs-lookup"><span data-stu-id="134f4-220">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="134f4-221">attachments</span><span class="sxs-lookup"><span data-stu-id="134f4-221">attachments</span></span>|<span data-ttu-id="134f4-222">Коллекция объектов [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="134f4-222">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="134f4-p111">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="134f4-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="134f4-225">extensions</span><span class="sxs-lookup"><span data-stu-id="134f4-225">extensions</span></span>|<span data-ttu-id="134f4-226">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="134f4-226">[Extension](extension.md) collection</span></span>|<span data-ttu-id="134f4-p112">Коллекция открытых расширений, определенных для публикации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="134f4-p112">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="134f4-230">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="134f4-230">inReplyTo</span></span>|[<span data-ttu-id="134f4-231">post</span><span class="sxs-lookup"><span data-stu-id="134f4-231">post</span></span>](post.md)| <span data-ttu-id="134f4-232">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="134f4-232">Read-only.</span></span>|
|<span data-ttu-id="134f4-233">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="134f4-233">multiValueExtendedProperties</span></span>|<span data-ttu-id="134f4-234">Коллекция объектов [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="134f4-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="134f4-p113">Коллекция расширенных свойств с несколькими значениями, определенных для публикации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="134f4-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="134f4-238">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="134f4-238">singleValueExtendedProperties</span></span>|<span data-ttu-id="134f4-239">Коллекция объектов [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="134f4-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="134f4-p114">Коллекция расширенных свойств с одним значением, определенных для публикации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="134f4-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="134f4-243">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="134f4-243">JSON representation</span></span>

<span data-ttu-id="134f4-244">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="134f4-244">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="134f4-245">См. также</span><span class="sxs-lookup"><span data-stu-id="134f4-245">See also</span></span>

- [<span data-ttu-id="134f4-246">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="134f4-246">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="134f4-247">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="134f4-247">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="134f4-248">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="134f4-248">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
