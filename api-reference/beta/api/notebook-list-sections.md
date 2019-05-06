---
title: Вывод списка разделов
description: Получение списка объектов Section из указанной записной книжки.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: e77ed40e0b76f8d591fc87ae17cd6ab46c12175e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597957"
---
# <a name="list-sections"></a><span data-ttu-id="f3ba1-103">Вывод списка разделов</span><span class="sxs-lookup"><span data-stu-id="f3ba1-103">List sections</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3ba1-104">Получение списка объектов [section](../resources/onenotesection.md) из указанной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="f3ba1-104">Retrieve a list of [section](../resources/onenotesection.md) objects from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3ba1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3ba1-105">Permissions</span></span>
<span data-ttu-id="f3ba1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3ba1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3ba1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3ba1-108">Permission type</span></span>      | <span data-ttu-id="f3ba1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3ba1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3ba1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3ba1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3ba1-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3ba1-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3ba1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3ba1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3ba1-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3ba1-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f3ba1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3ba1-114">Application</span></span> | <span data-ttu-id="f3ba1-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3ba1-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3ba1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3ba1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sections
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
GET /groups/{id}/onenote/notebooks/{id}/sections
GET /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f3ba1-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f3ba1-117">Optional query parameters</span></span>
<span data-ttu-id="f3ba1-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f3ba1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f3ba1-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="f3ba1-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="f3ba1-120">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `displayName`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="f3ba1-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="f3ba1-121">Допустимые `expand` значения для разделов `parentNotebook` — `parentSectionGroup`и.</span><span class="sxs-lookup"><span data-stu-id="f3ba1-121">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="f3ba1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3ba1-122">Request headers</span></span>
| <span data-ttu-id="f3ba1-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f3ba1-123">Name</span></span>       | <span data-ttu-id="f3ba1-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f3ba1-124">Type</span></span> | <span data-ttu-id="f3ba1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f3ba1-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f3ba1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3ba1-126">Authorization</span></span>  | <span data-ttu-id="f3ba1-127">string</span><span class="sxs-lookup"><span data-stu-id="f3ba1-127">string</span></span>  | <span data-ttu-id="f3ba1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3ba1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3ba1-130">Accept</span><span class="sxs-lookup"><span data-stu-id="f3ba1-130">Accept</span></span> | <span data-ttu-id="f3ba1-131">строка</span><span class="sxs-lookup"><span data-stu-id="f3ba1-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f3ba1-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3ba1-132">Request body</span></span>
<span data-ttu-id="f3ba1-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3ba1-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3ba1-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3ba1-134">Response</span></span>

<span data-ttu-id="f3ba1-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [оненотесектион](../resources/onenotesection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3ba1-135">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/onenotesection.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f3ba1-136">Пример</span><span class="sxs-lookup"><span data-stu-id="f3ba1-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3ba1-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3ba1-137">Request</span></span>
<span data-ttu-id="f3ba1-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3ba1-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
```
##### <a name="response"></a><span data-ttu-id="f3ba1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3ba1-139">Response</span></span>
<span data-ttu-id="f3ba1-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3ba1-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f3ba1-143">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="f3ba1-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f3ba1-144">Языках</span><span class="sxs-lookup"><span data-stu-id="f3ba1-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_sections-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3ba1-145">Язык</span><span class="sxs-lookup"><span data-stu-id="f3ba1-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_sections-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/notebook-list-sections.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/notebook-list-sections.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
