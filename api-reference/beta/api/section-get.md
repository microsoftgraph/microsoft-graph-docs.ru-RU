---
title: Получение раздела
description: Получение свойств и связей объекта Section.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 054d0988de977668db16c78d8d44c393dc5059b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453704"
---
# <a name="get-section"></a><span data-ttu-id="b3a8c-103">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="b3a8c-103">Get section</span></span>

<span data-ttu-id="b3a8c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b3a8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3a8c-105">Получение свойств и связей объекта [section](../resources/onenotesection.md) .</span><span class="sxs-lookup"><span data-stu-id="b3a8c-105">Retrieve the properties and relationships of a [section](../resources/onenotesection.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3a8c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3a8c-106">Permissions</span></span>
<span data-ttu-id="b3a8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3a8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3a8c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3a8c-109">Permission type</span></span>      | <span data-ttu-id="b3a8c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3a8c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3a8c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3a8c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3a8c-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3a8c-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3a8c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3a8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3a8c-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3a8c-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b3a8c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3a8c-115">Application</span></span> | <span data-ttu-id="b3a8c-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3a8c-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3a8c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3a8c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3a8c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b3a8c-118">Optional query parameters</span></span>
<span data-ttu-id="b3a8c-119">Этот метод поддерживает `select` `expand` [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b3a8c-119">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b3a8c-120">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `displayName`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="b3a8c-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="b3a8c-121">Допустимые `expand` значения для разделов `parentNotebook` — `parentSectionGroup`и.</span><span class="sxs-lookup"><span data-stu-id="b3a8c-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3a8c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3a8c-122">Request headers</span></span>
| <span data-ttu-id="b3a8c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b3a8c-123">Name</span></span>       | <span data-ttu-id="b3a8c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="b3a8c-124">Type</span></span> | <span data-ttu-id="b3a8c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b3a8c-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b3a8c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3a8c-126">Authorization</span></span>  | <span data-ttu-id="b3a8c-127">string</span><span class="sxs-lookup"><span data-stu-id="b3a8c-127">string</span></span>  | <span data-ttu-id="b3a8c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3a8c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3a8c-130">Accept</span><span class="sxs-lookup"><span data-stu-id="b3a8c-130">Accept</span></span> | <span data-ttu-id="b3a8c-131">строка</span><span class="sxs-lookup"><span data-stu-id="b3a8c-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b3a8c-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3a8c-132">Request body</span></span>
<span data-ttu-id="b3a8c-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3a8c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3a8c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3a8c-134">Response</span></span>

<span data-ttu-id="b3a8c-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [оненотесектион](../resources/onenotesection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3a8c-135">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/onenotesection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3a8c-136">Пример</span><span class="sxs-lookup"><span data-stu-id="b3a8c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3a8c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3a8c-137">Request</span></span>
<span data-ttu-id="b3a8c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3a8c-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3a8c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3a8c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}
```
# <a name="c"></a>[<span data-ttu-id="b3a8c-140">C#</span><span class="sxs-lookup"><span data-stu-id="b3a8c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-section-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3a8c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3a8c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-section-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3a8c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3a8c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-section-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b3a8c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3a8c-143">Response</span></span>
<span data-ttu-id="b3a8c-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3a8c-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
