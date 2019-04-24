---
title: Обновление объекта eventMessage
description: Обновление свойств объекта eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 160fbf70f243174265fc6e4e54feabb8042bd450
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463968"
---
# <a name="update-eventmessage"></a><span data-ttu-id="ea9f6-103">Обновление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="ea9f6-103">Update eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea9f6-104">Обновление свойств объекта [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="ea9f6-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea9f6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea9f6-105">Permissions</span></span>
<span data-ttu-id="ea9f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea9f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea9f6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea9f6-108">Permission type</span></span>      | <span data-ttu-id="ea9f6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea9f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea9f6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea9f6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea9f6-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea9f6-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ea9f6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea9f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea9f6-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea9f6-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ea9f6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea9f6-114">Application</span></span> | <span data-ttu-id="ea9f6-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea9f6-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea9f6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea9f6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ea9f6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea9f6-117">Request headers</span></span>
| <span data-ttu-id="ea9f6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ea9f6-118">Name</span></span>       | <span data-ttu-id="ea9f6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ea9f6-119">Type</span></span> | <span data-ttu-id="ea9f6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ea9f6-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ea9f6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea9f6-121">Authorization</span></span>  | <span data-ttu-id="ea9f6-122">string</span><span class="sxs-lookup"><span data-stu-id="ea9f6-122">string</span></span>  | <span data-ttu-id="ea9f6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea9f6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea9f6-125">Content-Type</span></span> | <span data-ttu-id="ea9f6-126">string</span><span class="sxs-lookup"><span data-stu-id="ea9f6-126">string</span></span>  | <span data-ttu-id="ea9f6-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="ea9f6-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea9f6-129">Request body</span></span>
<span data-ttu-id="ea9f6-p104">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="ea9f6-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea9f6-134">Property</span></span>     | <span data-ttu-id="ea9f6-135">Тип</span><span class="sxs-lookup"><span data-stu-id="ea9f6-135">Type</span></span>   |<span data-ttu-id="ea9f6-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ea9f6-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea9f6-137">categories</span><span class="sxs-lookup"><span data-stu-id="ea9f6-137">categories</span></span>|<span data-ttu-id="ea9f6-138">String</span><span class="sxs-lookup"><span data-stu-id="ea9f6-138">String</span></span>|<span data-ttu-id="ea9f6-139">Категории, связанные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="ea9f6-140">importance</span><span class="sxs-lookup"><span data-stu-id="ea9f6-140">importance</span></span>|<span data-ttu-id="ea9f6-141">String</span><span class="sxs-lookup"><span data-stu-id="ea9f6-141">String</span></span>|<span data-ttu-id="ea9f6-p105">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="ea9f6-144">isAllDay</span><span class="sxs-lookup"><span data-stu-id="ea9f6-144">isAllDay</span></span> |<span data-ttu-id="ea9f6-145">Логический</span><span class="sxs-lookup"><span data-stu-id="ea9f6-145">Boolean</span></span>|<span data-ttu-id="ea9f6-146">Указывает, продолжается ли событие за весь день.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-146">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="ea9f6-147">Для настройки этого свойства необходимо также настроить свойства **startDateTime** и **endDateTime** события.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-147">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="ea9f6-148">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ea9f6-148">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="ea9f6-149">Логический</span><span class="sxs-lookup"><span data-stu-id="ea9f6-149">Boolean</span></span>|<span data-ttu-id="ea9f6-150">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-150">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="ea9f6-151">isRead</span><span class="sxs-lookup"><span data-stu-id="ea9f6-151">isRead</span></span>|<span data-ttu-id="ea9f6-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea9f6-152">Boolean</span></span>|<span data-ttu-id="ea9f6-153">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-153">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="ea9f6-154">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ea9f6-154">isReadReceiptRequested</span></span>|<span data-ttu-id="ea9f6-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea9f6-155">Boolean</span></span>|<span data-ttu-id="ea9f6-156">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-156">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="ea9f6-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea9f6-157">Response</span></span>

<span data-ttu-id="ea9f6-158">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-158">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea9f6-159">Пример</span><span class="sxs-lookup"><span data-stu-id="ea9f6-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea9f6-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea9f6-160">Request</span></span>
<span data-ttu-id="ea9f6-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-161">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ea9f6-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea9f6-162">Response</span></span>
<span data-ttu-id="ea9f6-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea9f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/eventmessage-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
