---
title: Обновление объекта eventMessage
description: Обновление свойств объекта eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f0566c75cf3849d87e9433f4c5f70038c4c10087
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422378"
---
# <a name="update-eventmessage"></a><span data-ttu-id="3c8c2-103">Обновление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="3c8c2-103">Update eventMessage</span></span>

<span data-ttu-id="3c8c2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3c8c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c8c2-105">Обновление свойств объекта [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="3c8c2-105">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c8c2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c8c2-106">Permissions</span></span>
<span data-ttu-id="3c8c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c8c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c8c2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c8c2-109">Permission type</span></span>      | <span data-ttu-id="3c8c2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c8c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c8c2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c8c2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c8c2-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c8c2-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3c8c2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c8c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c8c2-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c8c2-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3c8c2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c8c2-115">Application</span></span> | <span data-ttu-id="3c8c2-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c8c2-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c8c2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c8c2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3c8c2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c8c2-118">Request headers</span></span>
| <span data-ttu-id="3c8c2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3c8c2-119">Name</span></span>       | <span data-ttu-id="3c8c2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3c8c2-120">Type</span></span> | <span data-ttu-id="3c8c2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3c8c2-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3c8c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c8c2-122">Authorization</span></span>  | <span data-ttu-id="3c8c2-123">string</span><span class="sxs-lookup"><span data-stu-id="3c8c2-123">string</span></span>  | <span data-ttu-id="3c8c2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c8c2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c8c2-126">Content-Type</span></span> | <span data-ttu-id="3c8c2-127">string</span><span class="sxs-lookup"><span data-stu-id="3c8c2-127">string</span></span>  | <span data-ttu-id="3c8c2-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="3c8c2-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c8c2-130">Request body</span></span>
<span data-ttu-id="3c8c2-p104">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="3c8c2-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c8c2-135">Property</span></span>     | <span data-ttu-id="3c8c2-136">Тип</span><span class="sxs-lookup"><span data-stu-id="3c8c2-136">Type</span></span>   |<span data-ttu-id="3c8c2-137">Описание</span><span class="sxs-lookup"><span data-stu-id="3c8c2-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c8c2-138">categories</span><span class="sxs-lookup"><span data-stu-id="3c8c2-138">categories</span></span>|<span data-ttu-id="3c8c2-139">String</span><span class="sxs-lookup"><span data-stu-id="3c8c2-139">String</span></span>|<span data-ttu-id="3c8c2-140">Категории, связанные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-140">The categories associated with the message.</span></span>|
|<span data-ttu-id="3c8c2-141">importance</span><span class="sxs-lookup"><span data-stu-id="3c8c2-141">importance</span></span>|<span data-ttu-id="3c8c2-142">String</span><span class="sxs-lookup"><span data-stu-id="3c8c2-142">String</span></span>|<span data-ttu-id="3c8c2-p105">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="3c8c2-145">isAllDay</span><span class="sxs-lookup"><span data-stu-id="3c8c2-145">isAllDay</span></span> |<span data-ttu-id="3c8c2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c8c2-146">Boolean</span></span>|<span data-ttu-id="3c8c2-147">Указывает, продолжается ли событие за весь день.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-147">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="3c8c2-148">Для настройки этого свойства необходимо также настроить свойства **startDateTime** и **endDateTime** события.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-148">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="3c8c2-149">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="3c8c2-149">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="3c8c2-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c8c2-150">Boolean</span></span>|<span data-ttu-id="3c8c2-151">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-151">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="3c8c2-152">isRead</span><span class="sxs-lookup"><span data-stu-id="3c8c2-152">isRead</span></span>|<span data-ttu-id="3c8c2-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c8c2-153">Boolean</span></span>|<span data-ttu-id="3c8c2-154">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-154">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="3c8c2-155">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="3c8c2-155">isReadReceiptRequested</span></span>|<span data-ttu-id="3c8c2-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c8c2-156">Boolean</span></span>|<span data-ttu-id="3c8c2-157">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-157">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="3c8c2-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c8c2-158">Response</span></span>

<span data-ttu-id="3c8c2-159">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-159">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c8c2-160">Пример</span><span class="sxs-lookup"><span data-stu-id="3c8c2-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c8c2-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c8c2-161">Request</span></span>
<span data-ttu-id="3c8c2-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c8c2-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c8c2-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3c8c2-164">C#</span><span class="sxs-lookup"><span data-stu-id="3c8c2-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c8c2-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c8c2-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c8c2-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c8c2-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c8c2-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c8c2-167">Response</span></span>
<span data-ttu-id="3c8c2-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c8c2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
