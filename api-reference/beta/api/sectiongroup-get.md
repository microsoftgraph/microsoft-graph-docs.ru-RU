---
title: Получение sectionGroup
description: Получение свойств и связей объекта sectionGroup.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: f6088369e43c4267aa3ed4bbac431843c5f7de0e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722512"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="2f582-103">Получение sectionGroup</span><span class="sxs-lookup"><span data-stu-id="2f582-103">Get sectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f582-104">Получение свойств и связей объекта [sectionGroup](../resources/sectiongroup.md) .</span><span class="sxs-lookup"><span data-stu-id="2f582-104">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f582-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f582-105">Permissions</span></span>
<span data-ttu-id="2f582-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f582-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f582-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f582-108">Permission type</span></span>      | <span data-ttu-id="2f582-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f582-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f582-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f582-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2f582-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f582-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="2f582-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f582-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f582-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f582-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="2f582-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f582-114">Application</span></span> | <span data-ttu-id="2f582-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f582-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f582-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f582-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2f582-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f582-117">Optional query parameters</span></span>
<span data-ttu-id="2f582-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2f582-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="2f582-119">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `name`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="2f582-119">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="2f582-120">Допустимые `expand` значения для групп разделов `parentNotebook` — `parentSectionGroup`и.</span><span class="sxs-lookup"><span data-stu-id="2f582-120">Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f582-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f582-121">Request headers</span></span>
| <span data-ttu-id="2f582-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2f582-122">Name</span></span>       | <span data-ttu-id="2f582-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2f582-123">Type</span></span> | <span data-ttu-id="2f582-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2f582-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2f582-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f582-125">Authorization</span></span>  | <span data-ttu-id="2f582-126">string</span><span class="sxs-lookup"><span data-stu-id="2f582-126">string</span></span>  | <span data-ttu-id="2f582-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f582-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f582-129">Accept</span><span class="sxs-lookup"><span data-stu-id="2f582-129">Accept</span></span> | <span data-ttu-id="2f582-130">строка</span><span class="sxs-lookup"><span data-stu-id="2f582-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="2f582-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f582-131">Request body</span></span>
<span data-ttu-id="2f582-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f582-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f582-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f582-133">Response</span></span>

<span data-ttu-id="2f582-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f582-134">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2f582-135">Пример</span><span class="sxs-lookup"><span data-stu-id="2f582-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f582-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f582-136">Request</span></span>
<span data-ttu-id="2f582-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f582-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2f582-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f582-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2f582-139">C#</span><span class="sxs-lookup"><span data-stu-id="2f582-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f582-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f582-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2f582-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2f582-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2f582-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f582-142">Response</span></span>
<span data-ttu-id="2f582-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f582-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
