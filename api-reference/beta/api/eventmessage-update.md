---
title: Обновление объекта eventMessage
description: Обновление свойств объекта eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b7c22cfee9ad7378166ac619a770894b110c510f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325057"
---
# <a name="update-eventmessage"></a><span data-ttu-id="008cd-103">Обновление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="008cd-103">Update eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="008cd-104">Обновление свойств объекта [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="008cd-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="008cd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="008cd-105">Permissions</span></span>
<span data-ttu-id="008cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="008cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="008cd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="008cd-108">Permission type</span></span>      | <span data-ttu-id="008cd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="008cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="008cd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="008cd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="008cd-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="008cd-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="008cd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="008cd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="008cd-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="008cd-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="008cd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="008cd-114">Application</span></span> | <span data-ttu-id="008cd-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="008cd-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="008cd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="008cd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="008cd-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="008cd-117">Request headers</span></span>
| <span data-ttu-id="008cd-118">Имя</span><span class="sxs-lookup"><span data-stu-id="008cd-118">Name</span></span>       | <span data-ttu-id="008cd-119">Тип</span><span class="sxs-lookup"><span data-stu-id="008cd-119">Type</span></span> | <span data-ttu-id="008cd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="008cd-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="008cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="008cd-121">Authorization</span></span>  | <span data-ttu-id="008cd-122">string</span><span class="sxs-lookup"><span data-stu-id="008cd-122">string</span></span>  | <span data-ttu-id="008cd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="008cd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="008cd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="008cd-125">Content-Type</span></span> | <span data-ttu-id="008cd-126">string</span><span class="sxs-lookup"><span data-stu-id="008cd-126">string</span></span>  | <span data-ttu-id="008cd-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="008cd-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="008cd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="008cd-129">Request body</span></span>
<span data-ttu-id="008cd-p104">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="008cd-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="008cd-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="008cd-134">Property</span></span>     | <span data-ttu-id="008cd-135">Тип</span><span class="sxs-lookup"><span data-stu-id="008cd-135">Type</span></span>   |<span data-ttu-id="008cd-136">Описание</span><span class="sxs-lookup"><span data-stu-id="008cd-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="008cd-137">categories</span><span class="sxs-lookup"><span data-stu-id="008cd-137">categories</span></span>|<span data-ttu-id="008cd-138">String</span><span class="sxs-lookup"><span data-stu-id="008cd-138">String</span></span>|<span data-ttu-id="008cd-139">Категории, связанные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="008cd-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="008cd-140">importance</span><span class="sxs-lookup"><span data-stu-id="008cd-140">importance</span></span>|<span data-ttu-id="008cd-141">String</span><span class="sxs-lookup"><span data-stu-id="008cd-141">String</span></span>|<span data-ttu-id="008cd-p105">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="008cd-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="008cd-144">isAllDay</span><span class="sxs-lookup"><span data-stu-id="008cd-144">isAllDay</span></span> |<span data-ttu-id="008cd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="008cd-145">Boolean</span></span>|<span data-ttu-id="008cd-146">Указывает, продолжается ли событие за весь день.</span><span class="sxs-lookup"><span data-stu-id="008cd-146">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="008cd-147">Для настройки этого свойства необходимо также настроить свойства **startDateTime** и **endDateTime** события.</span><span class="sxs-lookup"><span data-stu-id="008cd-147">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="008cd-148">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="008cd-148">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="008cd-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="008cd-149">Boolean</span></span>|<span data-ttu-id="008cd-150">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="008cd-150">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="008cd-151">isRead</span><span class="sxs-lookup"><span data-stu-id="008cd-151">isRead</span></span>|<span data-ttu-id="008cd-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="008cd-152">Boolean</span></span>|<span data-ttu-id="008cd-153">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="008cd-153">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="008cd-154">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="008cd-154">isReadReceiptRequested</span></span>|<span data-ttu-id="008cd-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="008cd-155">Boolean</span></span>|<span data-ttu-id="008cd-156">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="008cd-156">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="008cd-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="008cd-157">Response</span></span>

<span data-ttu-id="008cd-158">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="008cd-158">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="008cd-159">Пример</span><span class="sxs-lookup"><span data-stu-id="008cd-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="008cd-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="008cd-160">Request</span></span>
<span data-ttu-id="008cd-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="008cd-161">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="008cd-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="008cd-162">Response</span></span>
<span data-ttu-id="008cd-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="008cd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
