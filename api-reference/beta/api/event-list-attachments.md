---
title: Список вложений
description: Получение списка объектов attachment, вложенных в данные о событии.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cf092595f558d3aa1529023029ce84c6f2a4cb87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524011"
---
# <a name="list-attachments"></a><span data-ttu-id="d5738-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="d5738-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5738-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в данные о событии.</span><span class="sxs-lookup"><span data-stu-id="d5738-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5738-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5738-105">Permissions</span></span>

<span data-ttu-id="d5738-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5738-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5738-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5738-108">Permission type</span></span>      | <span data-ttu-id="d5738-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5738-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5738-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5738-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d5738-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d5738-111">Calendars.Read</span></span>    |
|<span data-ttu-id="d5738-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5738-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5738-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d5738-113">Calendars.Read</span></span>    |
|<span data-ttu-id="d5738-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5738-114">Application</span></span> | <span data-ttu-id="d5738-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d5738-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5738-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5738-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="d5738-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d5738-117">Optional query parameters</span></span>

<span data-ttu-id="d5738-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d5738-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d5738-119">В частности, можно использовать `$expand` параметр для включения всех встроенных вложений событий с помощью rest свойства событий запроса.</span><span class="sxs-lookup"><span data-stu-id="d5738-119">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="d5738-120">Пример:</span><span class="sxs-lookup"><span data-stu-id="d5738-120">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="d5738-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5738-121">Request headers</span></span>

| <span data-ttu-id="d5738-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d5738-122">Name</span></span>       | <span data-ttu-id="d5738-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d5738-123">Type</span></span> | <span data-ttu-id="d5738-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d5738-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d5738-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5738-125">Authorization</span></span>  | <span data-ttu-id="d5738-126">string</span><span class="sxs-lookup"><span data-stu-id="d5738-126">string</span></span>  | <span data-ttu-id="d5738-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5738-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5738-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5738-129">Request body</span></span>

<span data-ttu-id="d5738-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5738-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5738-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5738-131">Response</span></span>

<span data-ttu-id="d5738-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5738-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5738-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d5738-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5738-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5738-134">Request</span></span>

<span data-ttu-id="d5738-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5738-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="d5738-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5738-136">Response</span></span>

<span data-ttu-id="d5738-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d5738-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-list-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
