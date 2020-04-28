---
title: Список sectionGroups
description: Получение списка групп разделов из указанной записной книжки.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: a2d619829ac888e7210cfa525226ec1013a2cb05
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456728"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="d959d-103">Список sectionGroups</span><span class="sxs-lookup"><span data-stu-id="d959d-103">List sectionGroups</span></span>

<span data-ttu-id="d959d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d959d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d959d-105">Получение списка [групп разделов](../resources/sectiongroup.md) из указанной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="d959d-105">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="d959d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d959d-106">Permissions</span></span>
<span data-ttu-id="d959d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d959d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d959d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d959d-109">Permission type</span></span>      | <span data-ttu-id="d959d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d959d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d959d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d959d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d959d-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d959d-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d959d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d959d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d959d-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d959d-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d959d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d959d-115">Application</span></span> | <span data-ttu-id="d959d-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d959d-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d959d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d959d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
GET /groups/{id}/onenote/notebooks/{id}/sectionGroups
GET /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d959d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d959d-118">Optional query parameters</span></span>
<span data-ttu-id="d959d-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d959d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d959d-120">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="d959d-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="d959d-121">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `displayName`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="d959d-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="d959d-122">Допустимые `expand` значения для групп разделов `sections`: `sectionGroups`, `parentNotebook`, и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="d959d-122">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d959d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d959d-123">Request headers</span></span>
| <span data-ttu-id="d959d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d959d-124">Name</span></span>       | <span data-ttu-id="d959d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d959d-125">Type</span></span> | <span data-ttu-id="d959d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d959d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d959d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d959d-127">Authorization</span></span>  | <span data-ttu-id="d959d-128">string</span><span class="sxs-lookup"><span data-stu-id="d959d-128">string</span></span>  | <span data-ttu-id="d959d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d959d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d959d-131">Accept</span><span class="sxs-lookup"><span data-stu-id="d959d-131">Accept</span></span> | <span data-ttu-id="d959d-132">строка</span><span class="sxs-lookup"><span data-stu-id="d959d-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d959d-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d959d-133">Request body</span></span>
<span data-ttu-id="d959d-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d959d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d959d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d959d-135">Response</span></span>

<span data-ttu-id="d959d-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [sectionGroup](../resources/sectiongroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d959d-136">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d959d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d959d-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d959d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d959d-138">Request</span></span>
<span data-ttu-id="d959d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d959d-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d959d-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d959d-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_get_sectiongroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sectionGroups
```
# <a name="c"></a>[<span data-ttu-id="d959d-141">C#</span><span class="sxs-lookup"><span data-stu-id="d959d-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-get-sectiongroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d959d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d959d-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-get-sectiongroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d959d-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d959d-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-get-sectiongroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d959d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d959d-144">Response</span></span>
<span data-ttu-id="d959d-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d959d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
