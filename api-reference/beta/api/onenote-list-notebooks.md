---
title: Список записных книжек
description: Получение списка объектов записных книжек.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d0c18b3e7b872b4c3b94fb0ee5b123c78e39febb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265942"
---
# <a name="list-notebooks"></a><span data-ttu-id="a11a7-103">Список записных книжек</span><span class="sxs-lookup"><span data-stu-id="a11a7-103">List notebooks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a11a7-104">Получение списка объектов [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="a11a7-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a11a7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a11a7-105">Permissions</span></span>
<span data-ttu-id="a11a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a11a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a11a7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a11a7-108">Permission type</span></span>      | <span data-ttu-id="a11a7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a11a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a11a7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a11a7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a11a7-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a11a7-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a11a7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a11a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a11a7-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a11a7-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a11a7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a11a7-114">Application</span></span> | <span data-ttu-id="a11a7-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a11a7-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a11a7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a11a7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a11a7-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a11a7-117">Optional query parameters</span></span>
<span data-ttu-id="a11a7-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a11a7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a11a7-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="a11a7-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="a11a7-120">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="a11a7-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a11a7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a11a7-121">Request headers</span></span>
| <span data-ttu-id="a11a7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a11a7-122">Name</span></span>       | <span data-ttu-id="a11a7-123">Тип</span><span class="sxs-lookup"><span data-stu-id="a11a7-123">Type</span></span> | <span data-ttu-id="a11a7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a11a7-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a11a7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a11a7-125">Authorization</span></span>  | <span data-ttu-id="a11a7-126">string</span><span class="sxs-lookup"><span data-stu-id="a11a7-126">string</span></span>  | <span data-ttu-id="a11a7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a11a7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a11a7-129">Accept</span><span class="sxs-lookup"><span data-stu-id="a11a7-129">Accept</span></span> | <span data-ttu-id="a11a7-130">строка</span><span class="sxs-lookup"><span data-stu-id="a11a7-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a11a7-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a11a7-131">Request body</span></span>
<span data-ttu-id="a11a7-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a11a7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a11a7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a11a7-133">Response</span></span>

<span data-ttu-id="a11a7-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a11a7-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a11a7-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a11a7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a11a7-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a11a7-136">Request</span></span>
<span data-ttu-id="a11a7-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a11a7-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="a11a7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a11a7-138">Response</span></span>
<span data-ttu-id="a11a7-p103">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a11a7-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
    {
      "isDefault": true,
      "userRole": {
      },
      "isShared": true,
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
        }
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a11a7-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a11a7-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a11a7-143">C#</span><span class="sxs-lookup"><span data-stu-id="a11a7-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_notebooks-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a11a7-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a11a7-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_notebooks-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a11a7-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a11a7-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_notebooks-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/onenote-list-notebooks.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/onenote-list-notebooks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/onenote-list-notebooks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
