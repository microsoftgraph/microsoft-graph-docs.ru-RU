---
title: Обновление объекта eventMessage
description: Обновление свойств объекта eventMessage.
ms.openlocfilehash: 3d81977c815737ae96839c6fc883692bf2555597
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075286"
---
# <a name="update-eventmessage"></a><span data-ttu-id="c5f2a-103">Обновление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="c5f2a-103">Update eventMessage</span></span>

> <span data-ttu-id="c5f2a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5f2a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5f2a-106">Обновление свойств объекта [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="c5f2a-106">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5f2a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5f2a-107">Permissions</span></span>
<span data-ttu-id="c5f2a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5f2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f2a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5f2a-110">Permission type</span></span>      | <span data-ttu-id="c5f2a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5f2a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5f2a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5f2a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c5f2a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5f2a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c5f2a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5f2a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5f2a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5f2a-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c5f2a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5f2a-116">Application</span></span> | <span data-ttu-id="c5f2a-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5f2a-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5f2a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5f2a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c5f2a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5f2a-119">Request headers</span></span>
| <span data-ttu-id="c5f2a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c5f2a-120">Name</span></span>       | <span data-ttu-id="c5f2a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f2a-121">Type</span></span> | <span data-ttu-id="c5f2a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c5f2a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c5f2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5f2a-123">Authorization</span></span>  | <span data-ttu-id="c5f2a-124">string</span><span class="sxs-lookup"><span data-stu-id="c5f2a-124">string</span></span>  | <span data-ttu-id="c5f2a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5f2a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5f2a-127">Content-Type</span></span> | <span data-ttu-id="c5f2a-128">string</span><span class="sxs-lookup"><span data-stu-id="c5f2a-128">string</span></span>  | <span data-ttu-id="c5f2a-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="c5f2a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5f2a-131">Request body</span></span>
<span data-ttu-id="c5f2a-p105">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="c5f2a-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5f2a-136">Property</span></span>     | <span data-ttu-id="c5f2a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f2a-137">Type</span></span>   |<span data-ttu-id="c5f2a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="c5f2a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5f2a-139">categories</span><span class="sxs-lookup"><span data-stu-id="c5f2a-139">categories</span></span>|<span data-ttu-id="c5f2a-140">String</span><span class="sxs-lookup"><span data-stu-id="c5f2a-140">String</span></span>|<span data-ttu-id="c5f2a-141">Категории, связанные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="c5f2a-142">importance</span><span class="sxs-lookup"><span data-stu-id="c5f2a-142">importance</span></span>|<span data-ttu-id="c5f2a-143">String</span><span class="sxs-lookup"><span data-stu-id="c5f2a-143">String</span></span>|<span data-ttu-id="c5f2a-p106">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-p106">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="c5f2a-146">isAllDay</span><span class="sxs-lookup"><span data-stu-id="c5f2a-146">isAllDay</span></span> |<span data-ttu-id="c5f2a-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5f2a-147">Boolean</span></span>|<span data-ttu-id="c5f2a-148">Указывает, является ли событие длится весь день.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-148">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="c5f2a-149">Изменяет значения этого свойства требует настройки свойств **startDateTime** и **endDateTime** , а также события.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-149">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="c5f2a-150">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="c5f2a-150">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="c5f2a-151">Логический</span><span class="sxs-lookup"><span data-stu-id="c5f2a-151">Boolean</span></span>|<span data-ttu-id="c5f2a-152">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-152">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="c5f2a-153">isRead</span><span class="sxs-lookup"><span data-stu-id="c5f2a-153">isRead</span></span>|<span data-ttu-id="c5f2a-154">Логический</span><span class="sxs-lookup"><span data-stu-id="c5f2a-154">Boolean</span></span>|<span data-ttu-id="c5f2a-155">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-155">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="c5f2a-156">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="c5f2a-156">isReadReceiptRequested</span></span>|<span data-ttu-id="c5f2a-157">Логический</span><span class="sxs-lookup"><span data-stu-id="c5f2a-157">Boolean</span></span>|<span data-ttu-id="c5f2a-158">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-158">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="c5f2a-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5f2a-159">Response</span></span>

<span data-ttu-id="c5f2a-160">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-160">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5f2a-161">Пример</span><span class="sxs-lookup"><span data-stu-id="c5f2a-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5f2a-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5f2a-162">Request</span></span>
<span data-ttu-id="c5f2a-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5f2a-163">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c5f2a-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5f2a-164">Response</span></span>
<span data-ttu-id="c5f2a-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c5f2a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
