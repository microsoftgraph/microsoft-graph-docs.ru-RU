---
title: Вывод списка разделов
description: Получение списка объектов Section из указанной записной книжки.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: f30f503d4719f87d008eb98514cbfe8ca5b3e264
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053519"
---
# <a name="list-sections"></a><span data-ttu-id="67644-103">Вывод списка разделов</span><span class="sxs-lookup"><span data-stu-id="67644-103">List sections</span></span>

<span data-ttu-id="67644-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67644-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67644-105">Получение списка объектов [section](../resources/onenotesection.md) из указанной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="67644-105">Retrieve a list of [section](../resources/onenotesection.md) objects from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="67644-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67644-106">Permissions</span></span>
<span data-ttu-id="67644-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67644-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67644-109">Permission type</span></span>      | <span data-ttu-id="67644-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67644-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67644-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67644-111">Delegated (work or school account)</span></span> | <span data-ttu-id="67644-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67644-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="67644-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67644-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67644-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67644-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="67644-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67644-115">Application</span></span> | <span data-ttu-id="67644-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67644-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67644-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67644-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sections
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
GET /groups/{id}/onenote/notebooks/{id}/sections
GET /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67644-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="67644-118">Optional query parameters</span></span>
<span data-ttu-id="67644-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="67644-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="67644-120">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="67644-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="67644-121">Запрос по умолчанию разворачивает `parentNotebook` и выбирает `id` `displayName` свойства, и `self` .</span><span class="sxs-lookup"><span data-stu-id="67644-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="67644-122">Допустимые `expand` значения для разделов — `parentNotebook` и `parentSectionGroup` .</span><span class="sxs-lookup"><span data-stu-id="67644-122">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="67644-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67644-123">Request headers</span></span>
| <span data-ttu-id="67644-124">Имя</span><span class="sxs-lookup"><span data-stu-id="67644-124">Name</span></span>       | <span data-ttu-id="67644-125">Тип</span><span class="sxs-lookup"><span data-stu-id="67644-125">Type</span></span> | <span data-ttu-id="67644-126">Описание</span><span class="sxs-lookup"><span data-stu-id="67644-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="67644-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="67644-127">Authorization</span></span>  | <span data-ttu-id="67644-128">string</span><span class="sxs-lookup"><span data-stu-id="67644-128">string</span></span>  | <span data-ttu-id="67644-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67644-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67644-131">Accept</span><span class="sxs-lookup"><span data-stu-id="67644-131">Accept</span></span> | <span data-ttu-id="67644-132">строка</span><span class="sxs-lookup"><span data-stu-id="67644-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="67644-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67644-133">Request body</span></span>
<span data-ttu-id="67644-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67644-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67644-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="67644-135">Response</span></span>

<span data-ttu-id="67644-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [оненотесектион](../resources/onenotesection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67644-136">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/onenotesection.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67644-137">Пример</span><span class="sxs-lookup"><span data-stu-id="67644-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67644-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="67644-138">Request</span></span>
<span data-ttu-id="67644-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67644-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67644-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="67644-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_get_sections"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
```
# <a name="c"></a>[<span data-ttu-id="67644-141">C#</span><span class="sxs-lookup"><span data-stu-id="67644-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-get-sections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67644-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67644-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-get-sections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67644-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67644-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-get-sections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="67644-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="67644-144">Response</span></span>
<span data-ttu-id="67644-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67644-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


