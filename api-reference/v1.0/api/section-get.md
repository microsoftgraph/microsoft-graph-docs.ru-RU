---
title: Получение раздела
description: Получение свойств и связей объекта Оненотесектион.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: bbcd2c5a70e816da8b039b9b2ba81f48640070fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088944"
---
# <a name="get-section"></a><span data-ttu-id="a08db-103">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="a08db-103">Get section</span></span>

<span data-ttu-id="a08db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a08db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a08db-105">Получение свойств и связей объекта [оненотесектион](../resources/section.md) .</span><span class="sxs-lookup"><span data-stu-id="a08db-105">Retrieve the properties and relationships of a [onenoteSection](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a08db-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a08db-106">Permissions</span></span>
<span data-ttu-id="a08db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a08db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a08db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a08db-109">Permission type</span></span>      | <span data-ttu-id="a08db-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a08db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a08db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a08db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a08db-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a08db-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a08db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a08db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a08db-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a08db-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a08db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a08db-115">Application</span></span> | <span data-ttu-id="a08db-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a08db-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a08db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a08db-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a08db-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a08db-118">Optional query parameters</span></span>
<span data-ttu-id="a08db-119">Этот метод поддерживает `select` `expand` [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a08db-119">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a08db-120">Запрос по умолчанию разворачивает `parentNotebook` и выбирает `id` `displayName` свойства, и `self` .</span><span class="sxs-lookup"><span data-stu-id="a08db-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="a08db-121">Допустимые `expand` значения для разделов — `parentNotebook` и `parentSectionGroup` .</span><span class="sxs-lookup"><span data-stu-id="a08db-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a08db-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a08db-122">Request headers</span></span>
| <span data-ttu-id="a08db-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a08db-123">Name</span></span>       | <span data-ttu-id="a08db-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a08db-124">Type</span></span> | <span data-ttu-id="a08db-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a08db-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a08db-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a08db-126">Authorization</span></span>  | <span data-ttu-id="a08db-127">string</span><span class="sxs-lookup"><span data-stu-id="a08db-127">string</span></span>  | <span data-ttu-id="a08db-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a08db-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a08db-130">Accept</span><span class="sxs-lookup"><span data-stu-id="a08db-130">Accept</span></span> | <span data-ttu-id="a08db-131">строка</span><span class="sxs-lookup"><span data-stu-id="a08db-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a08db-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a08db-132">Request body</span></span>
<span data-ttu-id="a08db-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a08db-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a08db-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a08db-134">Response</span></span>

<span data-ttu-id="a08db-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [оненотесектион](../resources/section.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a08db-135">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a08db-136">Пример</span><span class="sxs-lookup"><span data-stu-id="a08db-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a08db-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a08db-137">Request</span></span>
<span data-ttu-id="a08db-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a08db-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a08db-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a08db-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
# <a name="c"></a>[<span data-ttu-id="a08db-140">C#</span><span class="sxs-lookup"><span data-stu-id="a08db-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-section-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a08db-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a08db-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-section-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a08db-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a08db-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-section-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a08db-143">Java</span><span class="sxs-lookup"><span data-stu-id="a08db-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-section-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a08db-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a08db-144">Response</span></span>
<span data-ttu-id="a08db-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a08db-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

