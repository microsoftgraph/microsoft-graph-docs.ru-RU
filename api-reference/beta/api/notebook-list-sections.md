---
title: Вывод списка разделов
description: Получение списка объектов Section из указанной записной книжки.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 757b0dca13ad209f6ae9ea737e2ce02f2441f7f2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342742"
---
# <a name="list-sections"></a><span data-ttu-id="626aa-103">Вывод списка разделов</span><span class="sxs-lookup"><span data-stu-id="626aa-103">List sections</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="626aa-104">Получение списка объектов [section](../resources/onenotesection.md) из указанной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="626aa-104">Retrieve a list of [section](../resources/onenotesection.md) objects from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="626aa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="626aa-105">Permissions</span></span>
<span data-ttu-id="626aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="626aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="626aa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="626aa-108">Permission type</span></span>      | <span data-ttu-id="626aa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="626aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="626aa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="626aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="626aa-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="626aa-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="626aa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="626aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="626aa-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="626aa-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="626aa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="626aa-114">Application</span></span> | <span data-ttu-id="626aa-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="626aa-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="626aa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="626aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sections
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
GET /groups/{id}/onenote/notebooks/{id}/sections
GET /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="626aa-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="626aa-117">Optional query parameters</span></span>
<span data-ttu-id="626aa-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="626aa-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="626aa-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="626aa-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="626aa-120">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `displayName`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="626aa-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="626aa-121">Допустимые `expand` значения для разделов `parentNotebook` — `parentSectionGroup`и.</span><span class="sxs-lookup"><span data-stu-id="626aa-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="626aa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="626aa-122">Request headers</span></span>
| <span data-ttu-id="626aa-123">Имя</span><span class="sxs-lookup"><span data-stu-id="626aa-123">Name</span></span>       | <span data-ttu-id="626aa-124">Тип</span><span class="sxs-lookup"><span data-stu-id="626aa-124">Type</span></span> | <span data-ttu-id="626aa-125">Описание</span><span class="sxs-lookup"><span data-stu-id="626aa-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="626aa-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="626aa-126">Authorization</span></span>  | <span data-ttu-id="626aa-127">string</span><span class="sxs-lookup"><span data-stu-id="626aa-127">string</span></span>  | <span data-ttu-id="626aa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="626aa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="626aa-130">Accept</span><span class="sxs-lookup"><span data-stu-id="626aa-130">Accept</span></span> | <span data-ttu-id="626aa-131">строка</span><span class="sxs-lookup"><span data-stu-id="626aa-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="626aa-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="626aa-132">Request body</span></span>
<span data-ttu-id="626aa-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="626aa-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="626aa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="626aa-134">Response</span></span>

<span data-ttu-id="626aa-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [оненотесектион](../resources/onenotesection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="626aa-135">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/onenotesection.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="626aa-136">Пример</span><span class="sxs-lookup"><span data-stu-id="626aa-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="626aa-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="626aa-137">Request</span></span>
<span data-ttu-id="626aa-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="626aa-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="626aa-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="626aa-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_get_sections"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="626aa-140">C#</span><span class="sxs-lookup"><span data-stu-id="626aa-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="626aa-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="626aa-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="626aa-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="626aa-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="626aa-143">Java</span><span class="sxs-lookup"><span data-stu-id="626aa-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-get-sections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="626aa-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="626aa-144">Response</span></span>
<span data-ttu-id="626aa-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="626aa-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
