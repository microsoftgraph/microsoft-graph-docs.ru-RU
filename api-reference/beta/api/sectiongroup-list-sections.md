---
title: Вывод списка разделов
description: Получение списка объектов Section из указанной группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: cb15fe0a5f50cf3b433ca7941437084802520b0b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976842"
---
# <a name="list-sections"></a><span data-ttu-id="ab14d-103">Вывод списка разделов</span><span class="sxs-lookup"><span data-stu-id="ab14d-103">List sections</span></span>

<span data-ttu-id="ab14d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab14d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab14d-105">Получение списка объектов [оненотесектион](../resources/onenotesection.md) из указанной группы разделов.</span><span class="sxs-lookup"><span data-stu-id="ab14d-105">Retrieve a list of [onenoteSection](../resources/onenotesection.md) objects from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab14d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab14d-106">Permissions</span></span>
<span data-ttu-id="ab14d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab14d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab14d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab14d-109">Permission type</span></span>      | <span data-ttu-id="ab14d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab14d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab14d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab14d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ab14d-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab14d-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab14d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab14d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab14d-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab14d-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ab14d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab14d-115">Application</span></span> | <span data-ttu-id="ab14d-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab14d-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab14d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab14d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sections
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
GET /groups/{id}/onenote/sectionGroups/{id}/sections
GET /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ab14d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ab14d-118">Optional query parameters</span></span>
<span data-ttu-id="ab14d-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ab14d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="ab14d-120">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="ab14d-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="ab14d-121">Запрос по умолчанию разворачивает `parentNotebook` и выбирает `id` `displayName` свойства, и `self` .</span><span class="sxs-lookup"><span data-stu-id="ab14d-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="ab14d-122">Допустимые `expand` значения для разделов — `parentNotebook` и `parentSectionGroup` .</span><span class="sxs-lookup"><span data-stu-id="ab14d-122">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ab14d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab14d-123">Request headers</span></span>
| <span data-ttu-id="ab14d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ab14d-124">Name</span></span>       | <span data-ttu-id="ab14d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="ab14d-125">Type</span></span> | <span data-ttu-id="ab14d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ab14d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ab14d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab14d-127">Authorization</span></span>  | <span data-ttu-id="ab14d-128">string</span><span class="sxs-lookup"><span data-stu-id="ab14d-128">string</span></span>  | <span data-ttu-id="ab14d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab14d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab14d-131">Accept</span><span class="sxs-lookup"><span data-stu-id="ab14d-131">Accept</span></span> | <span data-ttu-id="ab14d-132">строка</span><span class="sxs-lookup"><span data-stu-id="ab14d-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ab14d-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab14d-133">Request body</span></span>
<span data-ttu-id="ab14d-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab14d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab14d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab14d-135">Response</span></span>

<span data-ttu-id="ab14d-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [оненотесектион](../resources/onenotesection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab14d-136">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/onenotesection.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab14d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="ab14d-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab14d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab14d-138">Request</span></span>
<span data-ttu-id="ab14d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab14d-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab14d-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab14d-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sectiongroup_get_sections"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sections
```
# <a name="c"></a>[<span data-ttu-id="ab14d-141">C#</span><span class="sxs-lookup"><span data-stu-id="ab14d-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sectiongroup-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab14d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab14d-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sectiongroup-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab14d-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab14d-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sectiongroup-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab14d-144">Java</span><span class="sxs-lookup"><span data-stu-id="ab14d-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sectiongroup-get-sections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ab14d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab14d-145">Response</span></span>
<span data-ttu-id="ab14d-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab14d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
