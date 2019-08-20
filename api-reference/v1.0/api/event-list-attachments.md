---
title: Список вложений
description: Получение списка объектов attachment, вложенных в событие.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 50cc1490643442fa81011a42317aa39b96b4b8d9
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461722"
---
# <a name="list-attachments"></a><span data-ttu-id="8ff01-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="8ff01-103">List attachments</span></span>

<span data-ttu-id="8ff01-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в событие.</span><span class="sxs-lookup"><span data-stu-id="8ff01-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ff01-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ff01-105">Permissions</span></span>
<span data-ttu-id="8ff01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ff01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ff01-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ff01-108">Permission type</span></span>      | <span data-ttu-id="8ff01-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ff01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ff01-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ff01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ff01-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8ff01-111">Calendars.Read</span></span>    |
|<span data-ttu-id="8ff01-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ff01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff01-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8ff01-113">Calendars.Read</span></span>    |
|<span data-ttu-id="8ff01-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ff01-114">Application</span></span> | <span data-ttu-id="8ff01-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8ff01-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ff01-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ff01-116">HTTP request</span></span>
<span data-ttu-id="8ff01-117">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ff01-117">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="8ff01-118">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ff01-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="8ff01-119">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ff01-119">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8ff01-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8ff01-120">Optional query parameters</span></span>
<span data-ttu-id="8ff01-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8ff01-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8ff01-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ff01-122">Request headers</span></span>
| <span data-ttu-id="8ff01-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8ff01-123">Name</span></span>       | <span data-ttu-id="8ff01-124">Тип</span><span class="sxs-lookup"><span data-stu-id="8ff01-124">Type</span></span> | <span data-ttu-id="8ff01-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8ff01-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8ff01-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ff01-126">Authorization</span></span>  | <span data-ttu-id="8ff01-127">string</span><span class="sxs-lookup"><span data-stu-id="8ff01-127">string</span></span>  | <span data-ttu-id="8ff01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ff01-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ff01-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ff01-130">Request body</span></span>
<span data-ttu-id="8ff01-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ff01-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ff01-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ff01-132">Response</span></span>

<span data-ttu-id="8ff01-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ff01-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ff01-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8ff01-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ff01-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ff01-135">Request</span></span>
<span data-ttu-id="8ff01-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ff01-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8ff01-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ff01-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments_v1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ff01-138">C#</span><span class="sxs-lookup"><span data-stu-id="8ff01-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ff01-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ff01-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ff01-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8ff01-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8ff01-141">Java</span><span class="sxs-lookup"><span data-stu-id="8ff01-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8ff01-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ff01-142">Response</span></span>
<span data-ttu-id="8ff01-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ff01-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
