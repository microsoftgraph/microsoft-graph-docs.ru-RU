---
title: Обновление объекта eventMessage
description: Обновление свойств объекта eventMessage.
ms.openlocfilehash: 2bad679d4e460705c1716bd682c9e1afb0acc22b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025374"
---
# <a name="update-eventmessage"></a><span data-ttu-id="412d4-103">Обновление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="412d4-103">Update eventMessage</span></span>

<span data-ttu-id="412d4-104">Обновление свойств объекта [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="412d4-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="412d4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="412d4-105">Permissions</span></span>
<span data-ttu-id="412d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="412d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="412d4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="412d4-108">Permission type</span></span>      | <span data-ttu-id="412d4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="412d4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="412d4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="412d4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="412d4-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="412d4-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="412d4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="412d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="412d4-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="412d4-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="412d4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="412d4-114">Application</span></span> | <span data-ttu-id="412d4-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="412d4-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="412d4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="412d4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="412d4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="412d4-117">Request headers</span></span>
| <span data-ttu-id="412d4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="412d4-118">Name</span></span>       | <span data-ttu-id="412d4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="412d4-119">Type</span></span> | <span data-ttu-id="412d4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="412d4-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="412d4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="412d4-121">Authorization</span></span>  | <span data-ttu-id="412d4-122">string</span><span class="sxs-lookup"><span data-stu-id="412d4-122">string</span></span>  | <span data-ttu-id="412d4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="412d4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="412d4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="412d4-125">Content-Type</span></span> | <span data-ttu-id="412d4-126">string</span><span class="sxs-lookup"><span data-stu-id="412d4-126">string</span></span>  | <span data-ttu-id="412d4-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="412d4-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="412d4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="412d4-129">Request body</span></span>
<span data-ttu-id="412d4-p104">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="412d4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="412d4-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="412d4-134">Property</span></span>     | <span data-ttu-id="412d4-135">Тип</span><span class="sxs-lookup"><span data-stu-id="412d4-135">Type</span></span>   |<span data-ttu-id="412d4-136">Описание</span><span class="sxs-lookup"><span data-stu-id="412d4-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="412d4-137">categories</span><span class="sxs-lookup"><span data-stu-id="412d4-137">categories</span></span>|<span data-ttu-id="412d4-138">String</span><span class="sxs-lookup"><span data-stu-id="412d4-138">String</span></span>|<span data-ttu-id="412d4-139">Категории, связанные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="412d4-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="412d4-140">importance</span><span class="sxs-lookup"><span data-stu-id="412d4-140">importance</span></span>|<span data-ttu-id="412d4-141">String</span><span class="sxs-lookup"><span data-stu-id="412d4-141">String</span></span>|<span data-ttu-id="412d4-142">Важность сообщения.</span><span class="sxs-lookup"><span data-stu-id="412d4-142">The importance of the message.</span></span> <span data-ttu-id="412d4-143">Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="412d4-143">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="412d4-144">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="412d4-144">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="412d4-145">Логический</span><span class="sxs-lookup"><span data-stu-id="412d4-145">Boolean</span></span>|<span data-ttu-id="412d4-146">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="412d4-146">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="412d4-147">isRead</span><span class="sxs-lookup"><span data-stu-id="412d4-147">isRead</span></span>|<span data-ttu-id="412d4-148">Логический</span><span class="sxs-lookup"><span data-stu-id="412d4-148">Boolean</span></span>|<span data-ttu-id="412d4-149">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="412d4-149">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="412d4-150">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="412d4-150">isReadReceiptRequested</span></span>|<span data-ttu-id="412d4-151">Логический</span><span class="sxs-lookup"><span data-stu-id="412d4-151">Boolean</span></span>|<span data-ttu-id="412d4-152">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="412d4-152">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="412d4-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="412d4-153">Response</span></span>

<span data-ttu-id="412d4-154">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="412d4-154">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="412d4-155">Пример</span><span class="sxs-lookup"><span data-stu-id="412d4-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="412d4-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="412d4-156">Request</span></span>
<span data-ttu-id="412d4-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="412d4-157">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="412d4-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="412d4-158">Response</span></span>
<span data-ttu-id="412d4-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="412d4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
