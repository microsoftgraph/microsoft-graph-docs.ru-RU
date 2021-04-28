---
title: Список вложений
description: Получение списка объектов attachment, вложенных в событие.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e324d67cd6e7c57d3a936a0ec6d6e9ace3ec5df0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039589"
---
# <a name="list-attachments"></a><span data-ttu-id="672f1-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="672f1-103">List attachments</span></span>

<span data-ttu-id="672f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="672f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="672f1-105">Получение списка объектов [attachment](../resources/attachment.md), вложенных в событие.</span><span class="sxs-lookup"><span data-stu-id="672f1-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="672f1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="672f1-106">Permissions</span></span>
<span data-ttu-id="672f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="672f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="672f1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="672f1-109">Permission type</span></span>      | <span data-ttu-id="672f1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="672f1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="672f1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="672f1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="672f1-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="672f1-112">Calendars.Read</span></span>    |
|<span data-ttu-id="672f1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="672f1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="672f1-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="672f1-114">Calendars.Read</span></span>    |
|<span data-ttu-id="672f1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="672f1-115">Application</span></span> | <span data-ttu-id="672f1-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="672f1-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="672f1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="672f1-117">HTTP request</span></span>
<span data-ttu-id="672f1-118">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="672f1-118">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->

<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments
GET /users/{id | userPrincipalName}/events/{id}/attachments

GET /me/calendar/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
GET /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="672f1-119">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="672f1-119">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="672f1-120">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="672f1-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="672f1-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="672f1-121">Optional query parameters</span></span>
<span data-ttu-id="672f1-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="672f1-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="672f1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="672f1-123">Request headers</span></span>
| <span data-ttu-id="672f1-124">Имя</span><span class="sxs-lookup"><span data-stu-id="672f1-124">Name</span></span>       | <span data-ttu-id="672f1-125">Тип</span><span class="sxs-lookup"><span data-stu-id="672f1-125">Type</span></span> | <span data-ttu-id="672f1-126">Описание</span><span class="sxs-lookup"><span data-stu-id="672f1-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="672f1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="672f1-127">Authorization</span></span>  | <span data-ttu-id="672f1-128">string</span><span class="sxs-lookup"><span data-stu-id="672f1-128">string</span></span>  | <span data-ttu-id="672f1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="672f1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="672f1-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="672f1-131">Request body</span></span>
<span data-ttu-id="672f1-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="672f1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="672f1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="672f1-133">Response</span></span>

<span data-ttu-id="672f1-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="672f1-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="672f1-135">Пример</span><span class="sxs-lookup"><span data-stu-id="672f1-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="672f1-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="672f1-136">Request</span></span>
<span data-ttu-id="672f1-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="672f1-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="672f1-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="672f1-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments_v1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="672f1-139">C#</span><span class="sxs-lookup"><span data-stu-id="672f1-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="672f1-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="672f1-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="672f1-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="672f1-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="672f1-142">Java</span><span class="sxs-lookup"><span data-stu-id="672f1-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="672f1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="672f1-143">Response</span></span>
<span data-ttu-id="672f1-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="672f1-144">Here is an example of the response.</span></span> <span data-ttu-id="672f1-145">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="672f1-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "event_get_attachments_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
