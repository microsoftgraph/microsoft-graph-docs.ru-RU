---
title: Вывод списка разделов
description: Получение списка объектов Section.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: a388233f237b08d51b98c8906443511cd9deec7c
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406193"
---
# <a name="list-sections"></a><span data-ttu-id="01f47-103">Вывод списка разделов</span><span class="sxs-lookup"><span data-stu-id="01f47-103">List sections</span></span>

<span data-ttu-id="01f47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01f47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01f47-105">Получение списка объектов [section](../resources/onenotesection.md) .</span><span class="sxs-lookup"><span data-stu-id="01f47-105">Retrieve a list of [section](../resources/onenotesection.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="01f47-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01f47-106">Permissions</span></span>
<span data-ttu-id="01f47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01f47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01f47-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01f47-109">Permission type</span></span>      | <span data-ttu-id="01f47-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01f47-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01f47-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01f47-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01f47-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f47-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="01f47-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01f47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01f47-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01f47-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="01f47-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01f47-115">Application</span></span> | <span data-ttu-id="01f47-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f47-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01f47-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01f47-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections
GET /users/{id | userPrincipalName}/onenote/sections
GET /groups/{id}/onenote/sections
GET /sites/{id}/onenote/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01f47-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01f47-118">Optional query parameters</span></span>
<span data-ttu-id="01f47-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="01f47-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="01f47-120">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="01f47-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="01f47-121">Запрос по умолчанию разворачивает `parentNotebook` и выбирает `id` `displayName` свойства, и `self` .</span><span class="sxs-lookup"><span data-stu-id="01f47-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="01f47-122">Допустимые `expand` значения для разделов — `parentNotebook` и `parentSectionGroup` .</span><span class="sxs-lookup"><span data-stu-id="01f47-122">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01f47-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01f47-123">Request headers</span></span>
| <span data-ttu-id="01f47-124">Имя</span><span class="sxs-lookup"><span data-stu-id="01f47-124">Name</span></span>       | <span data-ttu-id="01f47-125">Тип</span><span class="sxs-lookup"><span data-stu-id="01f47-125">Type</span></span> | <span data-ttu-id="01f47-126">Описание</span><span class="sxs-lookup"><span data-stu-id="01f47-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01f47-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="01f47-127">Authorization</span></span>  | <span data-ttu-id="01f47-128">string</span><span class="sxs-lookup"><span data-stu-id="01f47-128">string</span></span>  | <span data-ttu-id="01f47-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01f47-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01f47-131">Accept</span><span class="sxs-lookup"><span data-stu-id="01f47-131">Accept</span></span> | <span data-ttu-id="01f47-132">строка</span><span class="sxs-lookup"><span data-stu-id="01f47-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="01f47-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01f47-133">Request body</span></span>
<span data-ttu-id="01f47-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01f47-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01f47-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="01f47-135">Response</span></span>

<span data-ttu-id="01f47-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [оненотесектион](../resources/onenotesection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01f47-136">If successful, this method returns a `200 OK` response code and collection of [onenoteSection](../resources/onenotesection.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01f47-137">Пример</span><span class="sxs-lookup"><span data-stu-id="01f47-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01f47-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="01f47-138">Request</span></span>
<span data-ttu-id="01f47-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01f47-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01f47-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="01f47-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "onenote_get_sections"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/sections
```
# <a name="c"></a>[<span data-ttu-id="01f47-141">C#</span><span class="sxs-lookup"><span data-stu-id="01f47-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/onenote-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01f47-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01f47-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/onenote-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01f47-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01f47-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/onenote-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="01f47-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="01f47-144">Response</span></span>
<span data-ttu-id="01f47-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01f47-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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