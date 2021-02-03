---
title: Получение вложения
description: Чтение свойств и связей вложения, вложенного в событие, сообщение, задачу Outlook или публикацию.
localization_priority: Normal
doc_type: apiPageType
author: svpsiva
ms.prod: outlook
ms.openlocfilehash: 5676615011806a5dbe07297080c06b976d945f11
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092409"
---
# <a name="get-attachment"></a><span data-ttu-id="3701c-103">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="3701c-103">Get attachment</span></span>

<span data-ttu-id="3701c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3701c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="3701c-105">Чтение свойств, связей или необработанных содержимого вложения, вложенного в событие [пользователя,](../resources/event.md) [сообщение,](../resources/message.md) [задачу Outlook](../resources/outlooktask.md)или групповую [публикацию.](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="3701c-105">Read the properties, relationships, or raw contents of an attachment that is attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md).</span></span> 

<span data-ttu-id="3701c-106">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="3701c-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="3701c-107">Файл.</span><span class="sxs-lookup"><span data-stu-id="3701c-107">A file.</span></span> <span data-ttu-id="3701c-108">Программным образом это ресурс [fileAttachment.](../resources/fileattachment.md)</span><span class="sxs-lookup"><span data-stu-id="3701c-108">Programmatically, this is a [fileAttachment](../resources/fileattachment.md) resource.</span></span>
* <span data-ttu-id="3701c-109">Элемент Outlook (контакт, событие или сообщение).</span><span class="sxs-lookup"><span data-stu-id="3701c-109">An Outlook item (contact, event or message).</span></span> <span data-ttu-id="3701c-110">Программным образом вложение элемента является [ресурсом itemAttachment.](../resources/itemattachment.md)</span><span class="sxs-lookup"><span data-stu-id="3701c-110">Programmatically, an item attachment is an [itemAttachment](../resources/itemattachment.md) resource.</span></span> <span data-ttu-id="3701c-111">Вы можете использовать `$expand` для получения других свойств этого элемента.</span><span class="sxs-lookup"><span data-stu-id="3701c-111">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="3701c-112">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="3701c-112">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="3701c-113">Ссылка на файл, хранимый в облаке.</span><span class="sxs-lookup"><span data-stu-id="3701c-113">A link to a file stored in the cloud.</span></span> <span data-ttu-id="3701c-114">Программным образом это ресурс [referenceAttachment.](../resources/referenceattachment.md)</span><span class="sxs-lookup"><span data-stu-id="3701c-114">Programmatically, this is a [referenceAttachment](../resources/referenceattachment.md) resource.</span></span>

<span data-ttu-id="3701c-115">Все эти типы вложений являются производными от ресурса [attachment.](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="3701c-115">All these types of attachments are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="3701c-116">Получение необработанного содержимого вложенного файла или элемента</span><span class="sxs-lookup"><span data-stu-id="3701c-116">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="3701c-117">Чтобы получить необработанное содержимое вложенного файла или элемента, вы можете добавить сегмент пути `/$value`.</span><span class="sxs-lookup"><span data-stu-id="3701c-117">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="3701c-118">Для вложенного файла тип содержимого определяется исходя из его исходного типа.</span><span class="sxs-lookup"><span data-stu-id="3701c-118">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="3701c-119">См. [пример](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) ниже.</span><span class="sxs-lookup"><span data-stu-id="3701c-119">See an [example](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) below.</span></span>

<span data-ttu-id="3701c-120">Для вложенного элемента, которое является [контактом ](../resources/contact.md), [событием ](../resources/event.md) и [сообщением](../resources/message.md), возвращаемое необработанное содержимое будет иметь формат MIME.</span><span class="sxs-lookup"><span data-stu-id="3701c-120">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="3701c-121">тип вложенного элемента</span><span class="sxs-lookup"><span data-stu-id="3701c-121">Item attachment type</span></span>  | <span data-ttu-id="3701c-122">Возвращаемое необработанное содержимое</span><span class="sxs-lookup"><span data-stu-id="3701c-122">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3701c-123">**контакт**</span><span class="sxs-lookup"><span data-stu-id="3701c-123">**contact**</span></span> | <span data-ttu-id="3701c-124">[vCard](http://www.faqs.org/rfcs/rfc2426.html) в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="3701c-124">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="3701c-125">См. [пример](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="3701c-125">See [example](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="3701c-126">**событие**</span><span class="sxs-lookup"><span data-stu-id="3701c-126">**event**</span></span> | <span data-ttu-id="3701c-127">iCal в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="3701c-127">iCal MIME format.</span></span> <span data-ttu-id="3701c-128">См. [пример](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="3701c-128">See [example](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="3701c-129">**сообщение**</span><span class="sxs-lookup"><span data-stu-id="3701c-129">**message**</span></span> | <span data-ttu-id="3701c-130">Формат MIME.</span><span class="sxs-lookup"><span data-stu-id="3701c-130">MIME format.</span></span> <span data-ttu-id="3701c-131">См. [пример](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="3701c-131">See [example](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="3701c-132">При попытке получить `$value` вложенной ссылки происходит возврат HTTP 405.</span><span class="sxs-lookup"><span data-stu-id="3701c-132">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="3701c-133">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3701c-133">Permissions</span></span>

<span data-ttu-id="3701c-134">В зависимости от ресурса **(события,** **сообщения,**  **outlookTask** или post), к который вложено вложение, и типа запрашиваемого разрешения (делегирование или приложение), разрешение, указанное в следующей таблице, является наименее привилегированным для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3701c-134">Depending on the resource (**event**, **message**, **outlookTask**, or **post**) that the attachment is attached to and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="3701c-135">Чтобы узнать больше, в том [числе](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) с осторожностью перед выбором более привилегированных разрешений, найди следующие разрешения в [разрешениях.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="3701c-135">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3701c-136">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="3701c-136">Supported resource</span></span> | <span data-ttu-id="3701c-137">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3701c-137">Delegated (work or school account)</span></span> | <span data-ttu-id="3701c-138">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3701c-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3701c-139">Приложение</span><span class="sxs-lookup"><span data-stu-id="3701c-139">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="3701c-140">event</span><span class="sxs-lookup"><span data-stu-id="3701c-140">event</span></span>](../resources/event.md) | <span data-ttu-id="3701c-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3701c-141">Calendars.Read</span></span> | <span data-ttu-id="3701c-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3701c-142">Calendars.Read</span></span> | <span data-ttu-id="3701c-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3701c-143">Calendars.Read</span></span> |
| [<span data-ttu-id="3701c-144">message</span><span class="sxs-lookup"><span data-stu-id="3701c-144">message</span></span>](../resources/message.md) | <span data-ttu-id="3701c-145">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3701c-145">Mail.Read</span></span> | <span data-ttu-id="3701c-146">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3701c-146">Mail.Read</span></span> | <span data-ttu-id="3701c-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3701c-147">Mail.Read</span></span> |
| [<span data-ttu-id="3701c-148">outlookTask</span><span class="sxs-lookup"><span data-stu-id="3701c-148">outlookTask</span></span>](../resources/outlooktask.md) |  <span data-ttu-id="3701c-149">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="3701c-149">Tasks.Read</span></span> | <span data-ttu-id="3701c-150">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="3701c-150">Tasks.Read</span></span> | <span data-ttu-id="3701c-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3701c-151">Not supported</span></span> |
| [<span data-ttu-id="3701c-152">post</span><span class="sxs-lookup"><span data-stu-id="3701c-152">post</span></span>](../resources/post.md) | <span data-ttu-id="3701c-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3701c-153">Group.Read.All</span></span> | <span data-ttu-id="3701c-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3701c-154">Not supported</span></span> | <span data-ttu-id="3701c-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3701c-155">Not supported</span></span> |


<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="3701c-156">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3701c-156">HTTP request</span></span>

<span data-ttu-id="3701c-157">В этом разделе показан синтаксис http GET-запроса для каждой сущности[(событие,](../resources/event.md) [сообщение,](../resources/message.md) [задача Outlook](../resources/outlooktask.md)и [публикация),](../resources/post.md)которые поддерживают вложения:</span><span class="sxs-lookup"><span data-stu-id="3701c-157">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), and [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="3701c-158">Чтобы получить свойства и связи вложения, укажите ИД  вложения для индексации в коллекции вложений, присоединенный к указанному событию, [](../resources/event.md)сообщению, [](../resources/message.md)задаче [Outlook](../resources/outlooktask.md)или экземпляру [post.](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="3701c-158">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="3701c-159">Если вложением является файл или элемент Outlook (контакт, событие или сообщение), вы можете также получить необработанное содержимое вложения, добавив сегмент пути `/$value` в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="3701c-159">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="3701c-160">Вложение [события:](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="3701c-160">An attachment of an [event](../resources/event.md):</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
GET /me/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}/$value
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="3701c-161">Вложение сообщения [в](../resources/message.md) почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="3701c-161">An attachment of a [message](../resources/message.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="3701c-162">Вложение сообщения [в](../resources/message.md) почтовом ящике пользователя верхнего уровня: [](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="3701c-162">An attachment of a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="3701c-163">Вложение [сообщения, которое](../resources/message.md) содержится в папке [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="3701c-163">An attachment of a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="3701c-164">В предыдущем примере показан один уровень вложенности, но сообщение может быть расположено в потомок потомка и так далее.</span><span class="sxs-lookup"><span data-stu-id="3701c-164">The preceding example shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>

<span data-ttu-id="3701c-165">Вложение задачи [Outlook:](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="3701c-165">An attachment of an [Outlook task](../resources/outlooktask.md):</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments/{id}
GET /users/{id}/outlook/tasks/{id}/attachments/{id}
GET /me/outlook/tasks/{id}/attachments/{id}/$value
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

<span data-ttu-id="3701c-166">Вложение post [в](../resources/post.md) [потоке,](../resources/conversationthread.md) принадлежащем [беседе](../resources/conversation.md) группы:</span><span class="sxs-lookup"><span data-stu-id="3701c-166">An attachment of a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3701c-167">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3701c-167">Optional query parameters</span></span>

<span data-ttu-id="3701c-168">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3701c-168">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3701c-169">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3701c-169">Request headers</span></span>

| <span data-ttu-id="3701c-170">Имя</span><span class="sxs-lookup"><span data-stu-id="3701c-170">Name</span></span>       | <span data-ttu-id="3701c-171">Тип</span><span class="sxs-lookup"><span data-stu-id="3701c-171">Type</span></span> | <span data-ttu-id="3701c-172">Описание</span><span class="sxs-lookup"><span data-stu-id="3701c-172">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3701c-173">Authorization</span><span class="sxs-lookup"><span data-stu-id="3701c-173">Authorization</span></span>  | <span data-ttu-id="3701c-174">string</span><span class="sxs-lookup"><span data-stu-id="3701c-174">string</span></span>  | <span data-ttu-id="3701c-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3701c-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3701c-177">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3701c-177">Request body</span></span>

<span data-ttu-id="3701c-178">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3701c-178">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3701c-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="3701c-179">Response</span></span>

<span data-ttu-id="3701c-180">В случае успеха метод GET возвращает `200 OK` код отклика.</span><span class="sxs-lookup"><span data-stu-id="3701c-180">If successful, the GET method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="3701c-181">При получении свойств и связей вложения текст ответа включает объект [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="3701c-181">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span>
<span data-ttu-id="3701c-182">Кроме того, возвращаются свойства этого типа вложения: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="3701c-182">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

<span data-ttu-id="3701c-183">При получении необработанного содержимого вложенного файла или элемента, текст ответа содержит необработанное значение вложения.</span><span class="sxs-lookup"><span data-stu-id="3701c-183">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="3701c-184">Примеры</span><span class="sxs-lookup"><span data-stu-id="3701c-184">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="3701c-185">Пример 1. Получение свойств вложенного файла</span><span class="sxs-lookup"><span data-stu-id="3701c-185">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="3701c-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="3701c-186">Request</span></span>

<span data-ttu-id="3701c-187">Вот пример запроса на просмотр свойств вложенного файла в сообщении.</span><span class="sxs-lookup"><span data-stu-id="3701c-187">Here is an example of the request to get the properties of a file attachment on a message.</span></span>

# <a name="http"></a>[<span data-ttu-id="3701c-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="3701c-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment_beta",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="c"></a>[<span data-ttu-id="3701c-189">C#</span><span class="sxs-lookup"><span data-stu-id="3701c-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3701c-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3701c-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3701c-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3701c-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3701c-192">Java</span><span class="sxs-lookup"><span data-stu-id="3701c-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3701c-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="3701c-193">Response</span></span>

<span data-ttu-id="3701c-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3701c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_file_attachment_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKjAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "id": "AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=",
    "lastModifiedDateTime": "2019-04-02T03:41:29Z",
    "name": "Draft sales invoice template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 13068,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "UEsDBBQABgAIAAAAIQ4AAAAA"
}
```

### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="3701c-197">Пример 2. Получение свойств вложенного элемента</span><span class="sxs-lookup"><span data-stu-id="3701c-197">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="3701c-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="3701c-198">Request</span></span>

<span data-ttu-id="3701c-199">В следующем примере показано, как получить вложенный элемент в сообщении.</span><span class="sxs-lookup"><span data-stu-id="3701c-199">The next example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="3701c-200">Возвращаются свойства **itemAttachment**.</span><span class="sxs-lookup"><span data-stu-id="3701c-200">The properties of the **itemAttachment** are returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="3701c-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="3701c-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```
# <a name="c"></a>[<span data-ttu-id="3701c-202">C#</span><span class="sxs-lookup"><span data-stu-id="3701c-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3701c-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3701c-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3701c-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3701c-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3701c-205">Java</span><span class="sxs-lookup"><span data-stu-id="3701c-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3701c-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="3701c-206">Response</span></span>
<span data-ttu-id="3701c-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3701c-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1M-CJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="3701c-210">Пример 3. Развертывание и изменение свойств элемента, вложенного в сообщение</span><span class="sxs-lookup"><span data-stu-id="3701c-210">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="3701c-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="3701c-211">Request</span></span>

<span data-ttu-id="3701c-212">В следующем примере показано, как использовать `$expand` для получения свойств элемента (контакт, событие или сообщение), вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="3701c-212">The next example shows how to use `$expand` to get the properties of the item (contact, event, or message) that is attached to the message.</span></span> <span data-ttu-id="3701c-213">В этом примере вложением является сообщением. Свойства вложенного сообщения также возвращаются.</span><span class="sxs-lookup"><span data-stu-id="3701c-213">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="3701c-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="3701c-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```
# <a name="c"></a>[<span data-ttu-id="3701c-215">C#</span><span class="sxs-lookup"><span data-stu-id="3701c-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3701c-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3701c-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3701c-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3701c-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3701c-218">Java</span><span class="sxs-lookup"><span data-stu-id="3701c-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3701c-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="3701c-219">Response</span></span>
<span data-ttu-id="3701c-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3701c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_and_expand_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
  "item":{
    "@odata.type":"#microsoft.graph.message",
    "id":"",
    "createdDateTime":"2017-07-21T00:20:41Z",
    "lastModifiedDateTime":"2017-07-21T00:20:34Z",
    "receivedDateTime":"2017-07-21T00:19:55Z",
    "sentDateTime":"2017-07-21T00:19:52Z",
    "hasAttachments":false,
    "internetMessageId":"<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
    "subject":"Reminder - please bring laptop",
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "conversationIndex":"AQHTAbcSwb41IIwGp0qstrYSZH+U7Q==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "body":{
      "contentType":"html",
      "content":"<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
    },
    "sender":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "from":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "toRecipients":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients":[
      {
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.onmicrosoft.com"
        }
      }
    ],
    "flag":{
      "flagStatus":"notFlagged"
    }
  }
}
```

### <a name="example-4-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="3701c-223">Пример 4. Получение свойств вложенной ссылки</span><span class="sxs-lookup"><span data-stu-id="3701c-223">Example 4: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="3701c-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="3701c-224">Request</span></span>

<span data-ttu-id="3701c-225">Ниже приведен пример запроса на получение вложенной ссылки из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="3701c-225">Here is an example of the request to get a reference attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="3701c-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="3701c-226">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGE1M88AADUv0uAAAG=","AAMkAGE1Mg72tgf7hJp0PICVGCc0g="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```
# <a name="c"></a>[<span data-ttu-id="3701c-227">C#</span><span class="sxs-lookup"><span data-stu-id="3701c-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3701c-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3701c-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3701c-229">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3701c-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3701c-230">Java</span><span class="sxs-lookup"><span data-stu-id="3701c-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3701c-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="3701c-231">Response</span></span>
<span data-ttu-id="3701c-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3701c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_reference_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```


### <a name="example-5-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="3701c-235">Пример 5. Получение необработанного содержимого вложенного файла в сообщении</span><span class="sxs-lookup"><span data-stu-id="3701c-235">Example 5: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="3701c-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="3701c-236">Request</span></span>

<span data-ttu-id="3701c-237">Ниже приведен пример запроса на получение необработанного содержимого файла Word, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="3701c-237">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="3701c-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="3701c-238">Response</span></span>
<span data-ttu-id="3701c-239">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3701c-239">Here is an example of the response.</span></span> <span data-ttu-id="3701c-240">Фактический текст ответа содержит необработанные байты вложенного файла, которые кратко описаны ниже.</span><span class="sxs-lookup"><span data-stu-id="3701c-240">The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="3701c-241">Пример 6. Получение необработанного содержимого MIME вложенного контакта в сообщении</span><span class="sxs-lookup"><span data-stu-id="3701c-241">Example 6: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="3701c-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="3701c-242">Request</span></span>

<span data-ttu-id="3701c-243">Ниже приведен пример запроса на получение необработанного содержимого элемента контакта, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="3701c-243">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="3701c-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="3701c-244">Response</span></span>
<span data-ttu-id="3701c-245">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3701c-245">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCARD
PROFILE:VCARD
VERSION:3.0
MAILER:Microsoft Exchange
PRODID:Microsoft Exchange
FN:Alex Wilbur
N:Wilbur;Alex;;;
NOTE:Sunday\, June 10\, 2012 5:44 PM:\nGutter\, window cleaning\, pressure 
 washing\, roof debris blowing\n
ORG:Contoso;
CLASS:PUBLIC
ADR;TYPE=WORK,PREF:;;4567 Main St;Buffalo;NY;98052;United States of America
LABEL;TYPE=WORK,PREF:4567 Main St\nBuffalo\, NY 98052
ADR;TYPE=HOME:;;;;;;
ADR;TYPE=POSTAL:;;;;;;
TEL;TYPE=WORK:(425) 555-0100
TITLE:
X-MS-IMADDRESS:
REV;VALUE=DATE-TIME:2019-04-09T02:13:31,161Z
END:VCARD
```


### <a name="example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="3701c-246">Пример 7. Получение необработанного содержимого MIME вложенного события в сообщении</span><span class="sxs-lookup"><span data-stu-id="3701c-246">Example 7: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="3701c-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="3701c-247">Request</span></span>

<span data-ttu-id="3701c-248">Ниже приведен пример запроса на получение необработанного содержимого события, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="3701c-248">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="3701c-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="3701c-249">Response</span></span>
<span data-ttu-id="3701c-250">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3701c-250">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCALENDAR
METHOD:PUBLISH
PRODID:Microsoft Exchange Server 2010
VERSION:2.0
BEGIN:VTIMEZONE
TZID:Pacific Standard Time
BEGIN:STANDARD
DTSTART:16010101T020000
TZOFFSETFROM:-0700
TZOFFSETTO:-0800
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=1SU;BYMONTH=11
END:STANDARD
BEGIN:DAYLIGHT
DTSTART:16010101T020000
TZOFFSETFROM:-0800
TZOFFSETTO:-0700
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=2SU;BYMONTH=3
END:DAYLIGHT
END:VTIMEZONE
BEGIN:VEVENT
ORGANIZER;CN=Adele Vance:MAILTO:adelev@contoso.com
ATTENDEE;ROLE=REQ-PARTICIPANT;PARTSTAT=NEEDS-ACTION;RSVP=TRUE;CN=Adele Vance:MAILTO:adelev@contoso.com
DESCRIPTION;LANGUAGE=en-US:\n
UID:040000008200
SUMMARY;LANGUAGE=en-US:Review Megan's docs
DTSTART;TZID=Pacific Standard Time:20190409T140000
DTEND;TZID=Pacific Standard Time:20190409T160000
CLASS:PUBLIC
PRIORITY:5
DTSTAMP:20190409T211833Z
TRANSP:OPAQUE
STATUS:CONFIRMED
SEQUENCE:0
LOCATION;LANGUAGE=en-US:
X-MICROSOFT-CDO-APPT-SEQUENCE:0
X-MICROSOFT-CDO-OWNERAPPTID:0
X-MICROSOFT-CDO-BUSYSTATUS:BUSY
X-MICROSOFT-CDO-INTENDEDSTATUS:BUSY
X-MICROSOFT-CDO-ALLDAYEVENT:FALSE
X-MICROSOFT-CDO-IMPORTANCE:1
X-MICROSOFT-CDO-INSTTYPE:0
X-MICROSOFT-DONOTFORWARDMEETING:FALSE
X-MICROSOFT-DISALLOW-COUNTER:FALSE
X-MICROSOFT-LOCATIONS:[]
BEGIN:VALARM
DESCRIPTION:REMINDER
TRIGGER;RELATED=START:-PT15M
ACTION:DISPLAY
END:VALARM
END:VEVENT
END:VCALENDAR
```


### <a name="example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="3701c-251">Пример 8. Получение необработанного содержимого MIME вложенного элемента приглашения на собрание в сообщении</span><span class="sxs-lookup"><span data-stu-id="3701c-251">Example 8: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="3701c-252">Запрос</span><span class="sxs-lookup"><span data-stu-id="3701c-252">Request</span></span>

<span data-ttu-id="3701c-253">Ниже приведен пример запроса на получение необработанного содержимого приглашения на собрание (типа [eventMessage](../resources/eventmessage.md)), вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="3701c-253">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="3701c-254">Сущность **eventMessage** основана на типе **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="3701c-254">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="3701c-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="3701c-255">Response</span></span>
<span data-ttu-id="3701c-256">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3701c-256">Here is an example of the response.</span></span> 

<span data-ttu-id="3701c-257">В тексте ответа содержится приложение **eventMessage** в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="3701c-257">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="3701c-258">Текст **eventMessage** усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="3701c-258">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="3701c-259">Полный текст сообщения возвращается от фактического вызова.</span><span class="sxs-lookup"><span data-stu-id="3701c-259">The full message body is returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

From: Megan Bowen <MeganB@contoso.OnMicrosoft.com>
To: Adele Vance <AdeleV@contoso.OnMicrosoft.com>
Subject: Let's go for lunch
Thread-Topic: Let's go for lunch
Thread-Index: AdTPqxOmg4AXoJV960a1j5NrJCHYjA==
X-MS-Exchange-MessageSentRepresentingType: 1
Date: Thu, 28 Feb 2019 21:17:58 +0000
Message-ID:
    <CY4PR2201MB1046E9C83FC42478EF4EE283C9750@CY4PR2201MB1046.namprd22.prod.outlook.com>
Content-Language: en-US
X-MS-Has-Attach:
X-MS-Exchange-Organization-SCL: -1
X-MS-TNEF-Correlator:
X-MS-Exchange-Organization-RecordReviewCfmType: 0
Content-Type: multipart/alternative;
    boundary="_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_"
MIME-Version: 1.0

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/plain; charset="us-ascii"

Does mid month work for you?

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/html; charset="us-ascii"

<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=us-ascii">
</head>
<body>
Does mid month work for you?
</body>
</html>

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/calendar; charset="utf-8"; method=REQUEST
Content-Transfer-Encoding: base64

QkVHSU46VkNBTEVOREFSDQpNRVRIT0Q6UkVRVUVTVA0KUFJPRElEOk1pY3Jvc29mdCBFeGNoYW5n


--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_--
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
