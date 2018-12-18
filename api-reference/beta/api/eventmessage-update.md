---
title: Обновление объекта eventMessage
description: Обновление свойств объекта eventMessage.
author: angelgolfer-ms
ms.openlocfilehash: 922f17528b864c8cdfae39a4df475a0a61f40103
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302473"
---
# <a name="update-eventmessage"></a><span data-ttu-id="214e6-103">Обновление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="214e6-103">Update eventMessage</span></span>

> <span data-ttu-id="214e6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="214e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="214e6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="214e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="214e6-106">Обновление свойств объекта [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="214e6-106">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="214e6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="214e6-107">Permissions</span></span>
<span data-ttu-id="214e6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="214e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="214e6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="214e6-110">Permission type</span></span>      | <span data-ttu-id="214e6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="214e6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="214e6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="214e6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="214e6-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="214e6-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="214e6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="214e6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="214e6-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="214e6-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="214e6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="214e6-116">Application</span></span> | <span data-ttu-id="214e6-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="214e6-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="214e6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="214e6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="214e6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="214e6-119">Request headers</span></span>
| <span data-ttu-id="214e6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="214e6-120">Name</span></span>       | <span data-ttu-id="214e6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="214e6-121">Type</span></span> | <span data-ttu-id="214e6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="214e6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="214e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="214e6-123">Authorization</span></span>  | <span data-ttu-id="214e6-124">string</span><span class="sxs-lookup"><span data-stu-id="214e6-124">string</span></span>  | <span data-ttu-id="214e6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="214e6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="214e6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="214e6-127">Content-Type</span></span> | <span data-ttu-id="214e6-128">string</span><span class="sxs-lookup"><span data-stu-id="214e6-128">string</span></span>  | <span data-ttu-id="214e6-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="214e6-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="214e6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="214e6-131">Request body</span></span>
<span data-ttu-id="214e6-p105">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="214e6-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="214e6-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="214e6-136">Property</span></span>     | <span data-ttu-id="214e6-137">Тип</span><span class="sxs-lookup"><span data-stu-id="214e6-137">Type</span></span>   |<span data-ttu-id="214e6-138">Описание</span><span class="sxs-lookup"><span data-stu-id="214e6-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="214e6-139">categories</span><span class="sxs-lookup"><span data-stu-id="214e6-139">categories</span></span>|<span data-ttu-id="214e6-140">String</span><span class="sxs-lookup"><span data-stu-id="214e6-140">String</span></span>|<span data-ttu-id="214e6-141">Категории, связанные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="214e6-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="214e6-142">importance</span><span class="sxs-lookup"><span data-stu-id="214e6-142">importance</span></span>|<span data-ttu-id="214e6-143">String</span><span class="sxs-lookup"><span data-stu-id="214e6-143">String</span></span>|<span data-ttu-id="214e6-p106">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="214e6-p106">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="214e6-146">isAllDay</span><span class="sxs-lookup"><span data-stu-id="214e6-146">isAllDay</span></span> |<span data-ttu-id="214e6-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="214e6-147">Boolean</span></span>|<span data-ttu-id="214e6-148">Указывает, является ли событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="214e6-148">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="214e6-149">Изменяет значения этого свойства требует настройки свойств **startDateTime** и **endDateTime** , а также события.</span><span class="sxs-lookup"><span data-stu-id="214e6-149">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="214e6-150">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="214e6-150">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="214e6-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="214e6-151">Boolean</span></span>|<span data-ttu-id="214e6-152">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="214e6-152">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="214e6-153">isRead</span><span class="sxs-lookup"><span data-stu-id="214e6-153">isRead</span></span>|<span data-ttu-id="214e6-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="214e6-154">Boolean</span></span>|<span data-ttu-id="214e6-155">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="214e6-155">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="214e6-156">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="214e6-156">isReadReceiptRequested</span></span>|<span data-ttu-id="214e6-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="214e6-157">Boolean</span></span>|<span data-ttu-id="214e6-158">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="214e6-158">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="214e6-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="214e6-159">Response</span></span>

<span data-ttu-id="214e6-160">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="214e6-160">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="214e6-161">Пример</span><span class="sxs-lookup"><span data-stu-id="214e6-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="214e6-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="214e6-162">Request</span></span>
<span data-ttu-id="214e6-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="214e6-163">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
##### <a name="response"></a><span data-ttu-id="214e6-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="214e6-164">Response</span></span>
<span data-ttu-id="214e6-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="214e6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
