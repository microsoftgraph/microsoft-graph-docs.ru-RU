---
title: Список вложений
description: Получение списка объектов attachment, вложенных в данные о событии.
author: angelgolfer-ms
ms.openlocfilehash: 051ab6fa9b2064ea62606f5d01de540600ed66c2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333875"
---
# <a name="list-attachments"></a><span data-ttu-id="c558f-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="c558f-103">List attachments</span></span>

> <span data-ttu-id="c558f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c558f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c558f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c558f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c558f-106">Получение списка объектов [attachment](../resources/attachment.md), вложенных в данные о событии.</span><span class="sxs-lookup"><span data-stu-id="c558f-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="c558f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c558f-107">Permissions</span></span>
<span data-ttu-id="c558f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c558f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c558f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c558f-110">Permission type</span></span>      | <span data-ttu-id="c558f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c558f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c558f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c558f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c558f-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c558f-113">Calendars.Read</span></span>    |
|<span data-ttu-id="c558f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c558f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c558f-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c558f-115">Calendars.Read</span></span>    |
|<span data-ttu-id="c558f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c558f-116">Application</span></span> | <span data-ttu-id="c558f-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c558f-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c558f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c558f-118">HTTP request</span></span>
<span data-ttu-id="c558f-119">Вложения для [событий](../resources/event.md) в списке пользователя по умолчанию [календаря](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="c558f-119">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="c558f-120">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c558f-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="c558f-121">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="c558f-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c558f-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c558f-122">Optional query parameters</span></span>
<span data-ttu-id="c558f-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c558f-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c558f-124">В частности, можно использовать $разверните параметр запроса для включения всех встроенных вложений событий с помощью rest свойства событий.</span><span class="sxs-lookup"><span data-stu-id="c558f-124">In particular, you can use the $expand query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="c558f-125">Пример:</span><span class="sxs-lookup"><span data-stu-id="c558f-125">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```


## <a name="request-headers"></a><span data-ttu-id="c558f-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c558f-126">Request headers</span></span>
| <span data-ttu-id="c558f-127">Имя</span><span class="sxs-lookup"><span data-stu-id="c558f-127">Name</span></span>       | <span data-ttu-id="c558f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c558f-128">Type</span></span> | <span data-ttu-id="c558f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c558f-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c558f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="c558f-130">Authorization</span></span>  | <span data-ttu-id="c558f-131">string</span><span class="sxs-lookup"><span data-stu-id="c558f-131">string</span></span>  | <span data-ttu-id="c558f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c558f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c558f-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c558f-134">Request body</span></span>
<span data-ttu-id="c558f-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c558f-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c558f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c558f-136">Response</span></span>

<span data-ttu-id="c558f-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c558f-137">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c558f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c558f-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c558f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c558f-139">Request</span></span>
<span data-ttu-id="c558f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c558f-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="c558f-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c558f-141">Response</span></span>
<span data-ttu-id="c558f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c558f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
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
  "tocPath": ""
}-->