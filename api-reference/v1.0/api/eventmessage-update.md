---
title: Обновление объекта eventMessage
description: Обновление свойств объекта eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b06df63d9a5dfd4e837fd682089823482d1a2118
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454981"
---
# <a name="update-eventmessage"></a><span data-ttu-id="4c357-103">Обновление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="4c357-103">Update eventMessage</span></span>

<span data-ttu-id="4c357-104">Обновление свойств объекта [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="4c357-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4c357-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c357-105">Permissions</span></span>
<span data-ttu-id="4c357-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c357-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c357-108">Permission type</span></span>      | <span data-ttu-id="4c357-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c357-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c357-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c357-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c357-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c357-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4c357-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c357-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c357-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c357-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4c357-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c357-114">Application</span></span> | <span data-ttu-id="4c357-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c357-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c357-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c357-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4c357-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c357-117">Request headers</span></span>
| <span data-ttu-id="4c357-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4c357-118">Name</span></span>       | <span data-ttu-id="4c357-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4c357-119">Type</span></span> | <span data-ttu-id="4c357-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4c357-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4c357-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c357-121">Authorization</span></span>  | <span data-ttu-id="4c357-122">string</span><span class="sxs-lookup"><span data-stu-id="4c357-122">string</span></span>  | <span data-ttu-id="4c357-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c357-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c357-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c357-125">Content-Type</span></span> | <span data-ttu-id="4c357-126">string</span><span class="sxs-lookup"><span data-stu-id="4c357-126">string</span></span>  | <span data-ttu-id="4c357-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c357-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="4c357-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c357-129">Request body</span></span>
<span data-ttu-id="4c357-p104">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="4c357-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="4c357-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c357-134">Property</span></span>     | <span data-ttu-id="4c357-135">Тип</span><span class="sxs-lookup"><span data-stu-id="4c357-135">Type</span></span>   |<span data-ttu-id="4c357-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4c357-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c357-137">categories</span><span class="sxs-lookup"><span data-stu-id="4c357-137">categories</span></span>|<span data-ttu-id="4c357-138">String</span><span class="sxs-lookup"><span data-stu-id="4c357-138">String</span></span>|<span data-ttu-id="4c357-139">Категории, связанные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="4c357-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="4c357-140">importance</span><span class="sxs-lookup"><span data-stu-id="4c357-140">importance</span></span>|<span data-ttu-id="4c357-141">String</span><span class="sxs-lookup"><span data-stu-id="4c357-141">String</span></span>|<span data-ttu-id="4c357-142">Важность сообщения.</span><span class="sxs-lookup"><span data-stu-id="4c357-142">The importance of the message.</span></span> <span data-ttu-id="4c357-143">Допустимые значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="4c357-143">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="4c357-144">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="4c357-144">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="4c357-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c357-145">Boolean</span></span>|<span data-ttu-id="4c357-146">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="4c357-146">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="4c357-147">isRead</span><span class="sxs-lookup"><span data-stu-id="4c357-147">isRead</span></span>|<span data-ttu-id="4c357-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c357-148">Boolean</span></span>|<span data-ttu-id="4c357-149">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="4c357-149">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="4c357-150">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="4c357-150">isReadReceiptRequested</span></span>|<span data-ttu-id="4c357-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c357-151">Boolean</span></span>|<span data-ttu-id="4c357-152">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="4c357-152">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="4c357-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c357-153">Response</span></span>

<span data-ttu-id="4c357-154">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c357-154">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c357-155">Пример</span><span class="sxs-lookup"><span data-stu-id="4c357-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c357-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c357-156">Request</span></span>
<span data-ttu-id="4c357-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c357-157">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4c357-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c357-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c357-159">C#</span><span class="sxs-lookup"><span data-stu-id="4c357-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c357-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c357-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c357-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4c357-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4c357-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c357-162">Response</span></span>
<span data-ttu-id="4c357-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c357-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
