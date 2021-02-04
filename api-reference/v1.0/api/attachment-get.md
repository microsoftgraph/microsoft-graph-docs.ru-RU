---
title: Получение вложения
description: 'Чтение свойств и связей объекта, представляющего вложение, которое было добавлено к данным о событии '
localization_priority: Priority
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8ffd1ceec1d3dbdb7e30a059836b11cc8e5a0276
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092640"
---
# <a name="get-attachment"></a><span data-ttu-id="4ade9-103">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="4ade9-103">Get attachment</span></span>

<span data-ttu-id="4ade9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ade9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ade9-105">Чтение свойств, связей или необработанного содержимого вложения, добавленного к пользовательскому [событию](../resources/event.md), [сообщению](../resources/message.md) или групповой [записи](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="4ade9-105">Read the properties, relationships, or raw contents of an attachment that is attached to a user [event](../resources/event.md), [message](../resources/message.md), or group [post](../resources/post.md).</span></span> 

<span data-ttu-id="4ade9-106">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="4ade9-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="4ade9-107">Файл.</span><span class="sxs-lookup"><span data-stu-id="4ade9-107">A file.</span></span> <span data-ttu-id="4ade9-108">На программном уровне это ресурс [fileAttachment](../resources/fileattachment.md).</span><span class="sxs-lookup"><span data-stu-id="4ade9-108">Programmatically, this is a [fileAttachment](../resources/fileattachment.md) resource.</span></span>
* <span data-ttu-id="4ade9-109">Элемент Outlook (контакт, событие или сообщение).</span><span class="sxs-lookup"><span data-stu-id="4ade9-109">An Outlook item (contact, event or message).</span></span> <span data-ttu-id="4ade9-110">На программном уровне вложением элемента является ресурс [itemAttachment](../resources/itemattachment.md).</span><span class="sxs-lookup"><span data-stu-id="4ade9-110">Programmatically, an item attachment is an [itemAttachment](../resources/itemattachment.md) resource.</span></span> <span data-ttu-id="4ade9-111">Вы можете использовать `$expand` для получения других свойств этого элемента.</span><span class="sxs-lookup"><span data-stu-id="4ade9-111">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="4ade9-112">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="4ade9-112">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="4ade9-113">Ссылка на файл, хранящийся в облаке.</span><span class="sxs-lookup"><span data-stu-id="4ade9-113">A link to a file stored in the cloud.</span></span> <span data-ttu-id="4ade9-114">На программном уровне это ресурс [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="4ade9-114">Programmatically, this is a [referenceAttachment](../resources/referenceattachment.md) resource.</span></span>

<span data-ttu-id="4ade9-115">Все эти типы вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="4ade9-115">All these types of attachments are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="4ade9-116">Получение необработанного содержимого вложенного файла или элемента</span><span class="sxs-lookup"><span data-stu-id="4ade9-116">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="4ade9-117">Чтобы получить необработанное содержимое вложенного файла или элемента, вы можете добавить сегмент пути `/$value`.</span><span class="sxs-lookup"><span data-stu-id="4ade9-117">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="4ade9-118">Для вложенного файла тип содержимого определяется исходя из его исходного типа.</span><span class="sxs-lookup"><span data-stu-id="4ade9-118">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="4ade9-119">См. [пример](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) ниже.</span><span class="sxs-lookup"><span data-stu-id="4ade9-119">See an [example](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) below.</span></span>

<span data-ttu-id="4ade9-120">Для вложенного элемента, которое является [контактом ](../resources/contact.md), [событием ](../resources/event.md) и [сообщением](../resources/message.md), возвращаемое необработанное содержимое будет иметь формат MIME.</span><span class="sxs-lookup"><span data-stu-id="4ade9-120">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="4ade9-121">тип вложенного элемента</span><span class="sxs-lookup"><span data-stu-id="4ade9-121">Item attachment type</span></span>  | <span data-ttu-id="4ade9-122">Возвращаемое необработанное содержимое</span><span class="sxs-lookup"><span data-stu-id="4ade9-122">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4ade9-123">**контакт**</span><span class="sxs-lookup"><span data-stu-id="4ade9-123">**contact**</span></span> | <span data-ttu-id="4ade9-124">[vCard](http://www.faqs.org/rfcs/rfc2426.html) в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="4ade9-124">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="4ade9-125">См. [пример](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="4ade9-125">See [example](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="4ade9-126">**событие**</span><span class="sxs-lookup"><span data-stu-id="4ade9-126">**event**</span></span> | <span data-ttu-id="4ade9-127">iCal в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="4ade9-127">iCal MIME format.</span></span> <span data-ttu-id="4ade9-128">См. [пример](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="4ade9-128">See [example](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="4ade9-129">**сообщение**</span><span class="sxs-lookup"><span data-stu-id="4ade9-129">**message**</span></span> | <span data-ttu-id="4ade9-130">Формат MIME.</span><span class="sxs-lookup"><span data-stu-id="4ade9-130">MIME format.</span></span> <span data-ttu-id="4ade9-131">См. [пример](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="4ade9-131">See [example](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="4ade9-132">При попытке получить `$value` вложенной ссылки происходит возврат HTTP 405.</span><span class="sxs-lookup"><span data-stu-id="4ade9-132">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ade9-133">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ade9-133">Permissions</span></span>

<span data-ttu-id="4ade9-134">В зависимости от ресурса (**event**, **message** или **post**), к которому добавлено вложение, и типа запрашиваемого расширения (делегированного или для приложений), разрешение, указанное в следующей таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4ade9-134">Depending on the resource (**event**, **message**, or **post**) that the attachment is attached to and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="4ade9-135">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ade9-135">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4ade9-136">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="4ade9-136">Supported resource</span></span> | <span data-ttu-id="4ade9-137">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ade9-137">Delegated (work or school account)</span></span> | <span data-ttu-id="4ade9-138">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ade9-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ade9-139">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ade9-139">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="4ade9-140">event</span><span class="sxs-lookup"><span data-stu-id="4ade9-140">event</span></span>](../resources/event.md) | <span data-ttu-id="4ade9-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4ade9-141">Calendars.Read</span></span> | <span data-ttu-id="4ade9-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4ade9-142">Calendars.Read</span></span> | <span data-ttu-id="4ade9-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4ade9-143">Calendars.Read</span></span> |
| [<span data-ttu-id="4ade9-144">message</span><span class="sxs-lookup"><span data-stu-id="4ade9-144">message</span></span>](../resources/message.md) | <span data-ttu-id="4ade9-145">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4ade9-145">Mail.Read</span></span> | <span data-ttu-id="4ade9-146">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4ade9-146">Mail.Read</span></span> | <span data-ttu-id="4ade9-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4ade9-147">Mail.Read</span></span> |
| [<span data-ttu-id="4ade9-148">post</span><span class="sxs-lookup"><span data-stu-id="4ade9-148">post</span></span>](../resources/post.md) | <span data-ttu-id="4ade9-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ade9-149">Group.Read.All</span></span> | <span data-ttu-id="4ade9-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4ade9-150">Not supported</span></span> | <span data-ttu-id="4ade9-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4ade9-151">Not supported</span></span> |


<!--
* If accessing attachments in group events or posts: Group.Read.All.
-->

## <a name="http-request"></a><span data-ttu-id="4ade9-152">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ade9-152">HTTP request</span></span>
<span data-ttu-id="4ade9-153">В этом разделе приведен синтаксис запроса HTTP GET для каждой из сущностей ([событие ](../resources/event.md), [сообщение ](../resources/message.md) и [запись](../resources/post.md)), поддерживающих вложения:</span><span class="sxs-lookup"><span data-stu-id="4ade9-153">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), and [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="4ade9-154">Чтобы получить свойства и связи вложения, определите идентификатор вложения для индексирования в коллекции **приложения**, вложенной в заданный экземпляр [события](../resources/event.md), [сообщения](../resources/message.md) или [записи](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="4ade9-154">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="4ade9-155">Если вложением является файл или элемент Outlook (контакт, событие или сообщение), вы можете также получить необработанное содержимое вложения, добавив сегмент пути `/$value` в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="4ade9-155">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="4ade9-156">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ade9-156">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}

GET /me/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}/$value
```

<span data-ttu-id="4ade9-157">Вложения [события](../resources/event.md) в указанном [календаре](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ade9-157">Attachments for an [event](../resources/event.md) in the specified user [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendars/{id}/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}/$value
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
GET /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="4ade9-158">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ade9-158">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}/$value
```
<span data-ttu-id="4ade9-159">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ade9-159">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}/$value
```
<span data-ttu-id="4ade9-160">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ade9-160">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}

GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="4ade9-161">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ade9-161">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}

GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="4ade9-p109">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д. </span><span class="sxs-lookup"><span data-stu-id="4ade9-p109">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}

GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```
<span data-ttu-id="4ade9-164">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="4ade9-164">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}

GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ade9-165">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ade9-165">Optional query parameters</span></span>
<span data-ttu-id="4ade9-166">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4ade9-166">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4ade9-167">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ade9-167">Request headers</span></span>
| <span data-ttu-id="4ade9-168">Имя</span><span class="sxs-lookup"><span data-stu-id="4ade9-168">Name</span></span>       | <span data-ttu-id="4ade9-169">Тип</span><span class="sxs-lookup"><span data-stu-id="4ade9-169">Type</span></span> | <span data-ttu-id="4ade9-170">Описание</span><span class="sxs-lookup"><span data-stu-id="4ade9-170">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4ade9-171">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ade9-171">Authorization</span></span>  | <span data-ttu-id="4ade9-172">string</span><span class="sxs-lookup"><span data-stu-id="4ade9-172">string</span></span>  | <span data-ttu-id="4ade9-p110">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ade9-p110">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ade9-175">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ade9-175">Request body</span></span>
<span data-ttu-id="4ade9-176">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ade9-176">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ade9-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ade9-177">Response</span></span>

<span data-ttu-id="4ade9-178">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4ade9-178">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="4ade9-179">При получении свойств и связей вложения текст ответа включает объект [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="4ade9-179">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span> <span data-ttu-id="4ade9-180">Кроме того, возвращаются свойства этого типа вложения: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="4ade9-180">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

<span data-ttu-id="4ade9-181">При получении необработанного содержимого вложенного файла или элемента, текст ответа содержит необработанное значение вложения.</span><span class="sxs-lookup"><span data-stu-id="4ade9-181">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="4ade9-182">Примеры</span><span class="sxs-lookup"><span data-stu-id="4ade9-182">Examples</span></span> 

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="4ade9-183">Пример 1. Получение свойств вложенного файла</span><span class="sxs-lookup"><span data-stu-id="4ade9-183">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4ade9-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ade9-184">Request</span></span>

<span data-ttu-id="4ade9-185">Ниже приведен пример запроса на получение вложенного файла из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="4ade9-185">Here is an example of the request to get a file attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ade9-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ade9-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment_v1",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="c"></a>[<span data-ttu-id="4ade9-187">C#</span><span class="sxs-lookup"><span data-stu-id="4ade9-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ade9-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ade9-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ade9-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ade9-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ade9-190">Java</span><span class="sxs-lookup"><span data-stu-id="4ade9-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4ade9-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ade9-191">Response</span></span>
<span data-ttu-id="4ade9-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ade9-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_file_attachment_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKjAAA%3D')/attachments/$entity",
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
### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="4ade9-195">Пример 2. Получение свойств вложенного элемента</span><span class="sxs-lookup"><span data-stu-id="4ade9-195">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4ade9-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ade9-196">Request</span></span>

<span data-ttu-id="4ade9-197">В следующем примере показано, как получить вложенный элемент в сообщении.</span><span class="sxs-lookup"><span data-stu-id="4ade9-197">The next example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="4ade9-198">Возвращаются свойства **itemAttachment**.</span><span class="sxs-lookup"><span data-stu-id="4ade9-198">The properties of the **itemAttachment** are returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ade9-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ade9-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_item_attachment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=
```
# <a name="c"></a>[<span data-ttu-id="4ade9-200">C#</span><span class="sxs-lookup"><span data-stu-id="4ade9-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ade9-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ade9-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ade9-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ade9-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ade9-203">Java</span><span class="sxs-lookup"><span data-stu-id="4ade9-203">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4ade9-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ade9-204">Response</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="4ade9-205">Пример 3. Развертывание и изменение свойств элемента, вложенного в сообщение</span><span class="sxs-lookup"><span data-stu-id="4ade9-205">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="4ade9-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ade9-206">Request</span></span>
<span data-ttu-id="4ade9-207">В следующем примере показано, как использовать `$expand` для получения свойств элемента (контакт, событие или сообщение), вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="4ade9-207">The next example shows how to use `$expand` to get the properties of the item (contact, event, or message) that is attached to the message.</span></span> <span data-ttu-id="4ade9-208">В этом примере вложением является сообщением. Свойства вложенного сообщения также возвращаются.</span><span class="sxs-lookup"><span data-stu-id="4ade9-208">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ade9-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ade9-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_item_attachment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```
# <a name="c"></a>[<span data-ttu-id="4ade9-210">C#</span><span class="sxs-lookup"><span data-stu-id="4ade9-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ade9-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ade9-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ade9-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ade9-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ade9-213">Java</span><span class="sxs-lookup"><span data-stu-id="4ade9-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4ade9-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ade9-214">Response</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
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
    ]
  }
}
```



### <a name="example-4-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="4ade9-215">Пример 4. Получение свойств вложенной ссылки</span><span class="sxs-lookup"><span data-stu-id="4ade9-215">Example 4: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4ade9-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ade9-216">Request</span></span>
<span data-ttu-id="4ade9-217">Ниже приведен пример запроса на получение вложенной ссылки из сообщения.</span><span class="sxs-lookup"><span data-stu-id="4ade9-217">Here is an example of the request to get a reference attachment on a message.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ade9-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ade9-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGUzY5QKgAAA=","AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKgAAA=/attachments/AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=
```
# <a name="c"></a>[<span data-ttu-id="4ade9-219">C#</span><span class="sxs-lookup"><span data-stu-id="4ade9-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ade9-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ade9-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ade9-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ade9-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ade9-222">Java</span><span class="sxs-lookup"><span data-stu-id="4ade9-222">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="4ade9-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ade9-223">Response</span></span>
<span data-ttu-id="4ade9-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ade9-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKgAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.referenceAttachment",
    "id": "AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=",
    "lastModifiedDateTime": "2019-04-02T02:58:11Z",
    "name": "Sales Invoice Template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 1060,
    "isInline": true
}
```

### <a name="example-5-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="4ade9-227">Пример 5. Получение необработанного содержимого вложенного файла в сообщении</span><span class="sxs-lookup"><span data-stu-id="4ade9-227">Example 5: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="4ade9-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ade9-228">Request</span></span>

<span data-ttu-id="4ade9-229">Ниже приведен пример запроса на получение необработанного содержимого файла Word, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="4ade9-229">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="4ade9-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ade9-230">Response</span></span>
<span data-ttu-id="4ade9-231">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ade9-231">Here is an example of the response.</span></span> <span data-ttu-id="4ade9-232">Фактический текст ответа содержит необработанные байты вложенного файла, которые кратко описаны ниже.</span><span class="sxs-lookup"><span data-stu-id="4ade9-232">The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="4ade9-233">Пример 6. Получение необработанного содержимого MIME вложенного контакта в сообщении</span><span class="sxs-lookup"><span data-stu-id="4ade9-233">Example 6: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="4ade9-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ade9-234">Request</span></span>

<span data-ttu-id="4ade9-235">Ниже приведен пример запроса на получение необработанного содержимого элемента контакта, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="4ade9-235">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="4ade9-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ade9-236">Response</span></span>
<span data-ttu-id="4ade9-237">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ade9-237">Here is an example of the response.</span></span> 

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


### <a name="example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="4ade9-238">Пример 7. Получение необработанного содержимого MIME вложенного события в сообщении</span><span class="sxs-lookup"><span data-stu-id="4ade9-238">Example 7: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="4ade9-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ade9-239">Request</span></span>

<span data-ttu-id="4ade9-240">Ниже приведен пример запроса на получение необработанного содержимого события, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="4ade9-240">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="4ade9-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ade9-241">Response</span></span>
<span data-ttu-id="4ade9-242">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ade9-242">Here is an example of the response.</span></span> 

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


### <a name="example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="4ade9-243">Пример 8. Получение необработанного содержимого MIME вложенного элемента приглашения на собрание в сообщении</span><span class="sxs-lookup"><span data-stu-id="4ade9-243">Example 8: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="4ade9-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ade9-244">Request</span></span>

<span data-ttu-id="4ade9-245">Ниже приведен пример запроса на получение необработанного содержимого приглашения на собрание (типа [eventMessage](../resources/eventmessage.md)), вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="4ade9-245">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="4ade9-246">Сущность **eventMessage** основана на типе **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="4ade9-246">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="4ade9-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ade9-247">Response</span></span>
<span data-ttu-id="4ade9-248">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ade9-248">Here is an example of the response.</span></span> 

<span data-ttu-id="4ade9-249">В тексте ответа содержится приложение **eventMessage** в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="4ade9-249">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="4ade9-250">Текст **eventMessage** усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="4ade9-250">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="4ade9-251">Полный текст сообщения возвращается от фактического вызова.</span><span class="sxs-lookup"><span data-stu-id="4ade9-251">The full message body is returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: get_and_expand_item_attachment/item:
      Property 'item' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
