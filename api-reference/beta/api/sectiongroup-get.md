---
title: Получение sectionGroup
description: Получение свойств и связей объекта sectionGroup.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: e2cd1dd261809ee01ea193c41dacf9d197076a13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453674"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="93e9f-103">Получение sectionGroup</span><span class="sxs-lookup"><span data-stu-id="93e9f-103">Get sectionGroup</span></span>

<span data-ttu-id="93e9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93e9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93e9f-105">Получение свойств и связей объекта [sectionGroup](../resources/sectiongroup.md) .</span><span class="sxs-lookup"><span data-stu-id="93e9f-105">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="93e9f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93e9f-106">Permissions</span></span>
<span data-ttu-id="93e9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93e9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93e9f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93e9f-109">Permission type</span></span>      | <span data-ttu-id="93e9f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93e9f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93e9f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93e9f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93e9f-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93e9f-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="93e9f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93e9f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93e9f-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93e9f-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="93e9f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93e9f-115">Application</span></span> | <span data-ttu-id="93e9f-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93e9f-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93e9f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93e9f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93e9f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="93e9f-118">Optional query parameters</span></span>
<span data-ttu-id="93e9f-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="93e9f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="93e9f-120">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `name`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="93e9f-120">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="93e9f-121">Допустимые `expand` значения для групп разделов `parentNotebook` — `parentSectionGroup`и.</span><span class="sxs-lookup"><span data-stu-id="93e9f-121">Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93e9f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93e9f-122">Request headers</span></span>
| <span data-ttu-id="93e9f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="93e9f-123">Name</span></span>       | <span data-ttu-id="93e9f-124">Тип</span><span class="sxs-lookup"><span data-stu-id="93e9f-124">Type</span></span> | <span data-ttu-id="93e9f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="93e9f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="93e9f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="93e9f-126">Authorization</span></span>  | <span data-ttu-id="93e9f-127">string</span><span class="sxs-lookup"><span data-stu-id="93e9f-127">string</span></span>  | <span data-ttu-id="93e9f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93e9f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93e9f-130">Accept</span><span class="sxs-lookup"><span data-stu-id="93e9f-130">Accept</span></span> | <span data-ttu-id="93e9f-131">строка</span><span class="sxs-lookup"><span data-stu-id="93e9f-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="93e9f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93e9f-132">Request body</span></span>
<span data-ttu-id="93e9f-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93e9f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93e9f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="93e9f-134">Response</span></span>

<span data-ttu-id="93e9f-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="93e9f-135">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93e9f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="93e9f-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93e9f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="93e9f-137">Request</span></span>
<span data-ttu-id="93e9f-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93e9f-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93e9f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="93e9f-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="93e9f-140">C#</span><span class="sxs-lookup"><span data-stu-id="93e9f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sectiongroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93e9f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93e9f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sectiongroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93e9f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93e9f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sectiongroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="93e9f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="93e9f-143">Response</span></span>
<span data-ttu-id="93e9f-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93e9f-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
