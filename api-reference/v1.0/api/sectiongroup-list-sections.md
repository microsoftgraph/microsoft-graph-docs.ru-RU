---
title: Вывод списка разделов
description: Получение списка объектов Оненотесектион из указанной группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: ddfd23b4513374180332f8f5a6077ac6bc62868d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509887"
---
# <a name="list-sections"></a><span data-ttu-id="c7aed-103">Вывод списка разделов</span><span class="sxs-lookup"><span data-stu-id="c7aed-103">List sections</span></span>

<span data-ttu-id="c7aed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7aed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7aed-105">Получение списка объектов [оненотесектион](../resources/section.md) из указанной группы разделов.</span><span class="sxs-lookup"><span data-stu-id="c7aed-105">Retrieve a list of [onenoteSection](../resources/section.md) objects from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7aed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7aed-106">Permissions</span></span>
<span data-ttu-id="c7aed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7aed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7aed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7aed-109">Permission type</span></span>      | <span data-ttu-id="c7aed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7aed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7aed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7aed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7aed-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7aed-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7aed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7aed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7aed-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7aed-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c7aed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7aed-115">Application</span></span> | <span data-ttu-id="c7aed-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7aed-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7aed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7aed-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sections
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
GET /groups/{id}/onenote/sectionGroups/{id}/sections
GET /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c7aed-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7aed-118">Optional query parameters</span></span>
<span data-ttu-id="c7aed-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c7aed-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c7aed-120">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="c7aed-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="c7aed-121">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `displayName`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="c7aed-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="c7aed-122">Допустимые `expand` значения для разделов `parentNotebook` — `parentSectionGroup`и.</span><span class="sxs-lookup"><span data-stu-id="c7aed-122">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="c7aed-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7aed-123">Request headers</span></span>
| <span data-ttu-id="c7aed-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c7aed-124">Name</span></span>       | <span data-ttu-id="c7aed-125">Тип</span><span class="sxs-lookup"><span data-stu-id="c7aed-125">Type</span></span> | <span data-ttu-id="c7aed-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c7aed-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c7aed-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7aed-127">Authorization</span></span>  | <span data-ttu-id="c7aed-128">string</span><span class="sxs-lookup"><span data-stu-id="c7aed-128">string</span></span>  | <span data-ttu-id="c7aed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7aed-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7aed-131">Accept</span><span class="sxs-lookup"><span data-stu-id="c7aed-131">Accept</span></span> | <span data-ttu-id="c7aed-132">строка</span><span class="sxs-lookup"><span data-stu-id="c7aed-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c7aed-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7aed-133">Request body</span></span>
<span data-ttu-id="c7aed-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7aed-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7aed-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7aed-135">Response</span></span>

<span data-ttu-id="c7aed-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [оненотесектион](../resources/section.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7aed-136">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7aed-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c7aed-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7aed-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7aed-138">Request</span></span>
<span data-ttu-id="c7aed-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7aed-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7aed-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7aed-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sectionsgroup_get_sections"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
```
# <a name="c"></a>[<span data-ttu-id="c7aed-141">C#</span><span class="sxs-lookup"><span data-stu-id="c7aed-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sectionsgroup-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7aed-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7aed-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sectionsgroup-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7aed-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7aed-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sectionsgroup-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7aed-144">Java</span><span class="sxs-lookup"><span data-stu-id="c7aed-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sectionsgroup-get-sections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c7aed-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7aed-145">Response</span></span>
<span data-ttu-id="c7aed-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7aed-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
