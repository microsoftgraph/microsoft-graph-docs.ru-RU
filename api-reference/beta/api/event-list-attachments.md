---
title: Список вложений
description: Получение списка объектов attachment, вложенных в событие.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: acfcbd41c07cd9e308e6ad1d705c8590298e04f3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042557"
---
# <a name="list-attachments"></a><span data-ttu-id="0e6ce-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="0e6ce-103">List attachments</span></span>

<span data-ttu-id="0e6ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e6ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e6ce-105">Получение списка объектов [attachment](../resources/attachment.md), вложенных в событие.</span><span class="sxs-lookup"><span data-stu-id="0e6ce-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e6ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e6ce-106">Permissions</span></span>

<span data-ttu-id="0e6ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e6ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e6ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e6ce-109">Permission type</span></span>      | <span data-ttu-id="0e6ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e6ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e6ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e6ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e6ce-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0e6ce-112">Calendars.Read</span></span>    |
|<span data-ttu-id="0e6ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e6ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e6ce-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0e6ce-114">Calendars.Read</span></span>    |
|<span data-ttu-id="0e6ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e6ce-115">Application</span></span> | <span data-ttu-id="0e6ce-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0e6ce-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e6ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e6ce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="0e6ce-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0e6ce-118">Optional query parameters</span></span>

<span data-ttu-id="0e6ce-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0e6ce-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="0e6ce-120">В частности, параметр запроса можно включить все вложения событий в линию с остальными свойствами `$expand` события.</span><span class="sxs-lookup"><span data-stu-id="0e6ce-120">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="0e6ce-121">Например:</span><span class="sxs-lookup"><span data-stu-id="0e6ce-121">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="0e6ce-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e6ce-122">Request headers</span></span>

| <span data-ttu-id="0e6ce-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0e6ce-123">Name</span></span>       | <span data-ttu-id="0e6ce-124">Тип</span><span class="sxs-lookup"><span data-stu-id="0e6ce-124">Type</span></span> | <span data-ttu-id="0e6ce-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0e6ce-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0e6ce-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e6ce-126">Authorization</span></span>  | <span data-ttu-id="0e6ce-127">string</span><span class="sxs-lookup"><span data-stu-id="0e6ce-127">string</span></span>  | <span data-ttu-id="0e6ce-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e6ce-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e6ce-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e6ce-130">Request body</span></span>

<span data-ttu-id="0e6ce-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e6ce-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e6ce-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e6ce-132">Response</span></span>

<span data-ttu-id="0e6ce-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e6ce-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e6ce-134">Пример</span><span class="sxs-lookup"><span data-stu-id="0e6ce-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e6ce-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e6ce-135">Request</span></span>

<span data-ttu-id="0e6ce-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e6ce-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e6ce-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e6ce-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments_beta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="0e6ce-138">C#</span><span class="sxs-lookup"><span data-stu-id="0e6ce-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e6ce-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e6ce-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e6ce-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e6ce-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e6ce-141">Java</span><span class="sxs-lookup"><span data-stu-id="0e6ce-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-attachments-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0e6ce-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e6ce-142">Response</span></span>

<span data-ttu-id="0e6ce-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0e6ce-143">Here is an example of the response.</span></span> <span data-ttu-id="0e6ce-144">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0e6ce-144">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "event_get_attachments_beta",
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
      "@odata.type":"#microsoft.graph.fileAttachment",
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
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
