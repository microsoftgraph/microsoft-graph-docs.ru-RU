---
title: Список sectionGroups
description: Получение списка групп разделов из указанной записной книжки.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d52a88e689c2fadab3bba5c10107538ad92a8b59
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266383"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="671fb-103">Список sectionGroups</span><span class="sxs-lookup"><span data-stu-id="671fb-103">List sectionGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="671fb-104">Получение списка [групп разделов](../resources/sectiongroup.md) из указанной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="671fb-104">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="671fb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="671fb-105">Permissions</span></span>
<span data-ttu-id="671fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="671fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="671fb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="671fb-108">Permission type</span></span>      | <span data-ttu-id="671fb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="671fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="671fb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="671fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="671fb-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="671fb-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="671fb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="671fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="671fb-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="671fb-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="671fb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="671fb-114">Application</span></span> | <span data-ttu-id="671fb-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="671fb-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="671fb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="671fb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
GET /groups/{id}/onenote/notebooks/{id}/sectionGroups
GET /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="671fb-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="671fb-117">Optional query parameters</span></span>
<span data-ttu-id="671fb-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="671fb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="671fb-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="671fb-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="671fb-120">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `displayName`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="671fb-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="671fb-121">Допустимые `expand` значения для групп разделов `sections`: `sectionGroups`, `parentNotebook`, и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="671fb-121">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="671fb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="671fb-122">Request headers</span></span>
| <span data-ttu-id="671fb-123">Имя</span><span class="sxs-lookup"><span data-stu-id="671fb-123">Name</span></span>       | <span data-ttu-id="671fb-124">Тип</span><span class="sxs-lookup"><span data-stu-id="671fb-124">Type</span></span> | <span data-ttu-id="671fb-125">Описание</span><span class="sxs-lookup"><span data-stu-id="671fb-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="671fb-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="671fb-126">Authorization</span></span>  | <span data-ttu-id="671fb-127">string</span><span class="sxs-lookup"><span data-stu-id="671fb-127">string</span></span>  | <span data-ttu-id="671fb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="671fb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="671fb-130">Accept</span><span class="sxs-lookup"><span data-stu-id="671fb-130">Accept</span></span> | <span data-ttu-id="671fb-131">строка</span><span class="sxs-lookup"><span data-stu-id="671fb-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="671fb-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="671fb-132">Request body</span></span>
<span data-ttu-id="671fb-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="671fb-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="671fb-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="671fb-134">Response</span></span>

<span data-ttu-id="671fb-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [sectionGroup](../resources/sectiongroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="671fb-135">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="671fb-136">Пример</span><span class="sxs-lookup"><span data-stu-id="671fb-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="671fb-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="671fb-137">Request</span></span>
<span data-ttu-id="671fb-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="671fb-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="671fb-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="671fb-139">Response</span></span>
<span data-ttu-id="671fb-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="671fb-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
    {
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="671fb-143">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="671fb-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="671fb-144">C#</span><span class="sxs-lookup"><span data-stu-id="671fb-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_sectiongroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="671fb-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="671fb-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_sectiongroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="671fb-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="671fb-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_sectiongroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-list-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/notebook-list-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/notebook-list-sectiongroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
