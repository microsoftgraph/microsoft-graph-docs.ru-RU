---
title: Список вложений
description: Получение списка объектов attachment, вложенных в данные о событии.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: d05bb4194a60346b97e6be368d6790fdebf8e12b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854707"
---
# <a name="list-attachments"></a><span data-ttu-id="f2cf5-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="f2cf5-103">List attachments</span></span>

> <span data-ttu-id="f2cf5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2cf5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2cf5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2cf5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2cf5-106">Получение списка объектов [attachment](../resources/attachment.md), вложенных в данные о событии.</span><span class="sxs-lookup"><span data-stu-id="f2cf5-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2cf5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2cf5-107">Permissions</span></span>

<span data-ttu-id="f2cf5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2cf5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2cf5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2cf5-110">Permission type</span></span>      | <span data-ttu-id="f2cf5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2cf5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2cf5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2cf5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2cf5-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2cf5-113">Calendars.Read</span></span>    |
|<span data-ttu-id="f2cf5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2cf5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2cf5-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2cf5-115">Calendars.Read</span></span>    |
|<span data-ttu-id="f2cf5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2cf5-116">Application</span></span> | <span data-ttu-id="f2cf5-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2cf5-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2cf5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2cf5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="f2cf5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2cf5-119">Optional query parameters</span></span>

<span data-ttu-id="f2cf5-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f2cf5-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f2cf5-121">В частности, можно использовать `$expand` параметр для включения всех встроенных вложений событий с помощью rest свойства событий запроса.</span><span class="sxs-lookup"><span data-stu-id="f2cf5-121">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="f2cf5-122">Пример:</span><span class="sxs-lookup"><span data-stu-id="f2cf5-122">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="f2cf5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2cf5-123">Request headers</span></span>

| <span data-ttu-id="f2cf5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f2cf5-124">Name</span></span>       | <span data-ttu-id="f2cf5-125">Тип</span><span class="sxs-lookup"><span data-stu-id="f2cf5-125">Type</span></span> | <span data-ttu-id="f2cf5-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f2cf5-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f2cf5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2cf5-127">Authorization</span></span>  | <span data-ttu-id="f2cf5-128">string</span><span class="sxs-lookup"><span data-stu-id="f2cf5-128">string</span></span>  | <span data-ttu-id="f2cf5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2cf5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2cf5-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f2cf5-131">Request body</span></span>

<span data-ttu-id="f2cf5-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2cf5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2cf5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2cf5-133">Response</span></span>

<span data-ttu-id="f2cf5-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2cf5-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2cf5-135">Пример</span><span class="sxs-lookup"><span data-stu-id="f2cf5-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2cf5-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2cf5-136">Request</span></span>

<span data-ttu-id="f2cf5-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2cf5-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="f2cf5-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2cf5-138">Response</span></span>

<span data-ttu-id="f2cf5-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f2cf5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
