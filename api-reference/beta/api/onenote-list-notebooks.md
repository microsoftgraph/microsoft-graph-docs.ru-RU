---
title: Список записных книжек
description: Получение списка объектов записных книжек.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: c0de11f9c42f6204660f57dfb78f601eb612b73f
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473922"
---
# <a name="list-notebooks"></a><span data-ttu-id="3b1e6-103">Список записных книжек</span><span class="sxs-lookup"><span data-stu-id="3b1e6-103">List notebooks</span></span>

<span data-ttu-id="3b1e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b1e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b1e6-105">Получение списка объектов [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="3b1e6-105">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b1e6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b1e6-106">Permissions</span></span>
<span data-ttu-id="3b1e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b1e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b1e6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b1e6-109">Permission type</span></span>      | <span data-ttu-id="3b1e6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b1e6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b1e6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b1e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3b1e6-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b1e6-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b1e6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b1e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b1e6-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b1e6-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3b1e6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b1e6-115">Application</span></span> | <span data-ttu-id="3b1e6-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b1e6-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b1e6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b1e6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3b1e6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3b1e6-118">Optional query parameters</span></span>
<span data-ttu-id="3b1e6-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3b1e6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="3b1e6-120">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="3b1e6-120">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="3b1e6-121">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="3b1e6-121">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b1e6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b1e6-122">Request headers</span></span>
| <span data-ttu-id="3b1e6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3b1e6-123">Name</span></span>       | <span data-ttu-id="3b1e6-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3b1e6-124">Type</span></span> | <span data-ttu-id="3b1e6-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3b1e6-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3b1e6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b1e6-126">Authorization</span></span>  | <span data-ttu-id="3b1e6-127">string</span><span class="sxs-lookup"><span data-stu-id="3b1e6-127">string</span></span>  | <span data-ttu-id="3b1e6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b1e6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b1e6-130">Accept</span><span class="sxs-lookup"><span data-stu-id="3b1e6-130">Accept</span></span> | <span data-ttu-id="3b1e6-131">строка</span><span class="sxs-lookup"><span data-stu-id="3b1e6-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3b1e6-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b1e6-132">Request body</span></span>
<span data-ttu-id="3b1e6-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3b1e6-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b1e6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b1e6-134">Response</span></span>

<span data-ttu-id="3b1e6-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3b1e6-135">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b1e6-136">Пример</span><span class="sxs-lookup"><span data-stu-id="3b1e6-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b1e6-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b1e6-137">Request</span></span>
<span data-ttu-id="3b1e6-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b1e6-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b1e6-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1e6-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
# <a name="c"></a>[<span data-ttu-id="3b1e6-140">C#</span><span class="sxs-lookup"><span data-stu-id="3b1e6-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b1e6-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1e6-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b1e6-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b1e6-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b1e6-143">Java</span><span class="sxs-lookup"><span data-stu-id="3b1e6-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebooks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3b1e6-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b1e6-144">Response</span></span>
<span data-ttu-id="3b1e6-p103">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b1e6-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "isDefault": true,
      "userRole":  "Owner",
      "isShared": false,
      "sectionsUrl": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d/sections",
      "sectionGroupsUrl": "https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/onenote/notebooks/1-10143016-70dc-4449-b92a-3015225f800d/sectionGroups",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
      "links": {
        "oneNoteClientUrl": {
          "href": "onenote:https://contoso-my.sharepoint.com/personal/admin_m365x841051_onmicrosoft_com/Documents/Notebooks/My%20Private%20notebook"
        },
        "oneNoteWebUrl": {
          "href": "https://contoso-my.sharepoint.com/personal/admin_m365x841051_onmicrosoft_com/Documents/Notebooks/My%20Private%20notebook"
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
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
