---
title: Список sectionGroups
description: Получение списка групп разделов из указанной группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 13023456138c8b8a144902a1d44f5f9e399624e9
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458861"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="5d3f0-103">Список sectionGroups</span><span class="sxs-lookup"><span data-stu-id="5d3f0-103">List sectionGroups</span></span>

<span data-ttu-id="5d3f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d3f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d3f0-105">Получение списка [групп разделов](../resources/sectiongroup.md) из указанной группы разделов.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-105">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d3f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d3f0-106">Permissions</span></span>
<span data-ttu-id="5d3f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d3f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d3f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d3f0-109">Permission type</span></span>      | <span data-ttu-id="5d3f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d3f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d3f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d3f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d3f0-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d3f0-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d3f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d3f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d3f0-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d3f0-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5d3f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d3f0-115">Application</span></span> | <span data-ttu-id="5d3f0-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d3f0-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d3f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d3f0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
GET /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
GET /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5d3f0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5d3f0-118">Optional query parameters</span></span>
<span data-ttu-id="5d3f0-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="5d3f0-120">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-120">The default sort order is `name asc`.</span></span>

<span data-ttu-id="5d3f0-121">Запрос по умолчанию разворачивает `parentNotebook` и выбирает `id` `displayName` свойства, и `self` .</span><span class="sxs-lookup"><span data-stu-id="5d3f0-121">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="5d3f0-122">Допустимые `expand` значения для групп разделов: `sections` ,, `sectionGroups` `parentNotebook` и `parentSectionGroup` .</span><span class="sxs-lookup"><span data-stu-id="5d3f0-122">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d3f0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d3f0-123">Request headers</span></span>
| <span data-ttu-id="5d3f0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="5d3f0-124">Name</span></span>       | <span data-ttu-id="5d3f0-125">Тип</span><span class="sxs-lookup"><span data-stu-id="5d3f0-125">Type</span></span> | <span data-ttu-id="5d3f0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="5d3f0-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5d3f0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d3f0-127">Authorization</span></span>  | <span data-ttu-id="5d3f0-128">string</span><span class="sxs-lookup"><span data-stu-id="5d3f0-128">string</span></span>  | <span data-ttu-id="5d3f0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d3f0-131">Accept</span><span class="sxs-lookup"><span data-stu-id="5d3f0-131">Accept</span></span> | <span data-ttu-id="5d3f0-132">строка</span><span class="sxs-lookup"><span data-stu-id="5d3f0-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5d3f0-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d3f0-133">Request body</span></span>
<span data-ttu-id="5d3f0-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d3f0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d3f0-135">Response</span></span>

<span data-ttu-id="5d3f0-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [sectionGroup](../resources/sectiongroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-136">If successful, this method returns a `200 OK` response code and a collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d3f0-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5d3f0-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d3f0-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d3f0-138">Request</span></span>
<span data-ttu-id="5d3f0-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d3f0-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d3f0-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
```
# <a name="c"></a>[<span data-ttu-id="5d3f0-141">C#</span><span class="sxs-lookup"><span data-stu-id="5d3f0-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sectiongroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d3f0-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d3f0-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sectiongroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d3f0-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d3f0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sectiongroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d3f0-144">Java</span><span class="sxs-lookup"><span data-stu-id="5d3f0-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-sectiongroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5d3f0-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d3f0-145">Response</span></span>
<span data-ttu-id="5d3f0-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
