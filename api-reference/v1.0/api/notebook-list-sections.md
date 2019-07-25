---
title: Вывод списка разделов
description: Получение списка объектов Оненотесектион из указанной записной книжки.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 9b0f348014633fc3b5a403c0f9c128018a35cf3e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892740"
---
# <a name="list-sections"></a><span data-ttu-id="88011-103">Вывод списка разделов</span><span class="sxs-lookup"><span data-stu-id="88011-103">List sections</span></span>

<span data-ttu-id="88011-104">Получение списка объектов [оненотесектион](../resources/section.md) из указанной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="88011-104">Retrieve a list of [onenoteSection](../resources/section.md) objects from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="88011-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88011-105">Permissions</span></span>
<span data-ttu-id="88011-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88011-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88011-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88011-108">Permission type</span></span>      | <span data-ttu-id="88011-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88011-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88011-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88011-110">Delegated (work or school account)</span></span> | <span data-ttu-id="88011-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88011-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="88011-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88011-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88011-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88011-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="88011-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88011-114">Application</span></span> | <span data-ttu-id="88011-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88011-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88011-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88011-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sections
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
GET /groups/{id}/onenote/notebooks/{id}/sections
GET /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88011-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="88011-117">Optional query parameters</span></span>
<span data-ttu-id="88011-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="88011-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="88011-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="88011-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="88011-120">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `displayName`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="88011-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="88011-121">Допустимые `expand` значения для разделов `parentNotebook` — `parentSectionGroup`и.</span><span class="sxs-lookup"><span data-stu-id="88011-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="88011-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88011-122">Request headers</span></span>
| <span data-ttu-id="88011-123">Имя</span><span class="sxs-lookup"><span data-stu-id="88011-123">Name</span></span>       | <span data-ttu-id="88011-124">Тип</span><span class="sxs-lookup"><span data-stu-id="88011-124">Type</span></span> | <span data-ttu-id="88011-125">Описание</span><span class="sxs-lookup"><span data-stu-id="88011-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="88011-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="88011-126">Authorization</span></span>  | <span data-ttu-id="88011-127">string</span><span class="sxs-lookup"><span data-stu-id="88011-127">string</span></span>  | <span data-ttu-id="88011-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88011-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88011-130">Accept</span><span class="sxs-lookup"><span data-stu-id="88011-130">Accept</span></span> | <span data-ttu-id="88011-131">строка</span><span class="sxs-lookup"><span data-stu-id="88011-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="88011-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88011-132">Request body</span></span>
<span data-ttu-id="88011-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88011-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88011-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="88011-134">Response</span></span>

<span data-ttu-id="88011-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [оненотесектион](../resources/section.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88011-135">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88011-136">Пример</span><span class="sxs-lookup"><span data-stu-id="88011-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88011-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="88011-137">Request</span></span>
<span data-ttu-id="88011-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88011-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="88011-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="88011-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_get_sections"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="88011-140">C#</span><span class="sxs-lookup"><span data-stu-id="88011-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88011-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="88011-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="88011-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="88011-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="88011-143">Java</span><span class="sxs-lookup"><span data-stu-id="88011-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-get-sections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="88011-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="88011-144">Response</span></span>
<span data-ttu-id="88011-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88011-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
