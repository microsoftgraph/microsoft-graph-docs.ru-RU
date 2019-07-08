---
title: Список sectionGroups
description: Получение списка объектов sectionGroup.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 6aa1b1a65ef48bbcfcc8412fdd7f3f017e29932c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35435985"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="46a6a-103">Список sectionGroups</span><span class="sxs-lookup"><span data-stu-id="46a6a-103">List sectionGroups</span></span>

<span data-ttu-id="46a6a-104">Получение списка объектов [sectionGroup](../resources/sectiongroup.md) .</span><span class="sxs-lookup"><span data-stu-id="46a6a-104">Retrieve a list of [sectionGroup](../resources/sectiongroup.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="46a6a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46a6a-105">Permissions</span></span>
<span data-ttu-id="46a6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46a6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46a6a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46a6a-108">Permission type</span></span>      | <span data-ttu-id="46a6a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46a6a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46a6a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46a6a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="46a6a-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a6a-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="46a6a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46a6a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46a6a-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46a6a-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="46a6a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46a6a-114">Application</span></span> | <span data-ttu-id="46a6a-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a6a-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46a6a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46a6a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups
GET /groups/{id}/onenote/sectionGroups
GET /sites/{id}/onenote/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="46a6a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="46a6a-117">Optional query parameters</span></span>
<span data-ttu-id="46a6a-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="46a6a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="46a6a-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="46a6a-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="46a6a-120">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `displayName`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="46a6a-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="46a6a-121">Допустимые `expand` значения для групп разделов `sections`: `sectionGroups`, `parentNotebook`, и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="46a6a-121">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46a6a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46a6a-122">Request headers</span></span>
| <span data-ttu-id="46a6a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="46a6a-123">Name</span></span>       | <span data-ttu-id="46a6a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="46a6a-124">Type</span></span> | <span data-ttu-id="46a6a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="46a6a-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="46a6a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="46a6a-126">Authorization</span></span>  | <span data-ttu-id="46a6a-127">string</span><span class="sxs-lookup"><span data-stu-id="46a6a-127">string</span></span>  | <span data-ttu-id="46a6a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46a6a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46a6a-130">Accept</span><span class="sxs-lookup"><span data-stu-id="46a6a-130">Accept</span></span> | <span data-ttu-id="46a6a-131">строка</span><span class="sxs-lookup"><span data-stu-id="46a6a-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="46a6a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46a6a-132">Request body</span></span>
<span data-ttu-id="46a6a-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46a6a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46a6a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="46a6a-134">Response</span></span>

<span data-ttu-id="46a6a-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [sectionGroup](../resources/sectiongroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46a6a-135">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46a6a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="46a6a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46a6a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="46a6a-137">Request</span></span>
<span data-ttu-id="46a6a-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46a6a-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46a6a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="46a6a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46a6a-140">C#</span><span class="sxs-lookup"><span data-stu-id="46a6a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sectiongroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46a6a-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="46a6a-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sectiongroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46a6a-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="46a6a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sectiongroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="46a6a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="46a6a-143">Response</span></span>
<span data-ttu-id="46a6a-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46a6a-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
    {
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
