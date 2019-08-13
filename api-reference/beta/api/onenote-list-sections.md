---
title: Вывод списка разделов
description: Получение списка объектов Section.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 1b45e73ab852f79845d0008c6c936115ed873c64
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342618"
---
# <a name="list-sections"></a><span data-ttu-id="8f4a9-103">Вывод списка разделов</span><span class="sxs-lookup"><span data-stu-id="8f4a9-103">List sections</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f4a9-104">Получение списка объектов [section](../resources/onenotesection.md) .</span><span class="sxs-lookup"><span data-stu-id="8f4a9-104">Retrieve a list of [section](../resources/onenotesection.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f4a9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f4a9-105">Permissions</span></span>
<span data-ttu-id="8f4a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f4a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f4a9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f4a9-108">Permission type</span></span>      | <span data-ttu-id="8f4a9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f4a9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f4a9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f4a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f4a9-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4a9-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f4a9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f4a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f4a9-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4a9-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="8f4a9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f4a9-114">Application</span></span> | <span data-ttu-id="8f4a9-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4a9-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f4a9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f4a9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections
GET /users/{id | userPrincipalName}/onenote/sections
GET /groups/{id}/onenote/sections
GET /sites/{id}/onenote/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8f4a9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f4a9-117">Optional query parameters</span></span>
<span data-ttu-id="8f4a9-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8f4a9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="8f4a9-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="8f4a9-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="8f4a9-120">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `displayName`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="8f4a9-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="8f4a9-121">Допустимые `expand` значения для разделов `parentNotebook` — `parentSectionGroup`и.</span><span class="sxs-lookup"><span data-stu-id="8f4a9-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f4a9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f4a9-122">Request headers</span></span>
| <span data-ttu-id="8f4a9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8f4a9-123">Name</span></span>       | <span data-ttu-id="8f4a9-124">Тип</span><span class="sxs-lookup"><span data-stu-id="8f4a9-124">Type</span></span> | <span data-ttu-id="8f4a9-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8f4a9-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8f4a9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f4a9-126">Authorization</span></span>  | <span data-ttu-id="8f4a9-127">string</span><span class="sxs-lookup"><span data-stu-id="8f4a9-127">string</span></span>  | <span data-ttu-id="8f4a9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f4a9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f4a9-130">Accept</span><span class="sxs-lookup"><span data-stu-id="8f4a9-130">Accept</span></span> | <span data-ttu-id="8f4a9-131">строка</span><span class="sxs-lookup"><span data-stu-id="8f4a9-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="8f4a9-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f4a9-132">Request body</span></span>
<span data-ttu-id="8f4a9-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f4a9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f4a9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f4a9-134">Response</span></span>

<span data-ttu-id="8f4a9-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [оненотесектион](../resources/onenotesection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f4a9-135">If successful, this method returns a `200 OK` response code and collection of [onenoteSection](../resources/onenotesection.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8f4a9-136">Пример</span><span class="sxs-lookup"><span data-stu-id="8f4a9-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f4a9-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f4a9-137">Request</span></span>
<span data-ttu-id="8f4a9-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f4a9-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f4a9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f4a9-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "onenote_get_sections"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f4a9-140">C#</span><span class="sxs-lookup"><span data-stu-id="8f4a9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/onenote-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f4a9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f4a9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/onenote-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f4a9-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8f4a9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/onenote-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f4a9-143">Java</span><span class="sxs-lookup"><span data-stu-id="8f4a9-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/onenote-get-sections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8f4a9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f4a9-144">Response</span></span>
<span data-ttu-id="8f4a9-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f4a9-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "isDefault": true,
      "pagesUrl": "pagesUrl-value",
      "displayName": "name-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
