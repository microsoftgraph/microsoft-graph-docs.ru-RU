---
title: Список записных книжек
description: Получение списка объектов записных книжек.
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: cabdf21f697dd4be36fba34ffbe26eab1e37d288
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976490"
---
# <a name="list-notebooks"></a><span data-ttu-id="723b5-103">Список записных книжек</span><span class="sxs-lookup"><span data-stu-id="723b5-103">List notebooks</span></span>

<span data-ttu-id="723b5-104">Получение списка объектов [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="723b5-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="723b5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="723b5-105">Permissions</span></span>
<span data-ttu-id="723b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="723b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="723b5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="723b5-108">Permission type</span></span>      | <span data-ttu-id="723b5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="723b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="723b5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="723b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="723b5-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="723b5-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="723b5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="723b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="723b5-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="723b5-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="723b5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="723b5-114">Application</span></span> | <span data-ttu-id="723b5-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="723b5-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="723b5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="723b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="723b5-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="723b5-117">Optional query parameters</span></span>
<span data-ttu-id="723b5-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="723b5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="723b5-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="723b5-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="723b5-120">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="723b5-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="723b5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="723b5-121">Request headers</span></span>
| <span data-ttu-id="723b5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="723b5-122">Name</span></span>       | <span data-ttu-id="723b5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="723b5-123">Type</span></span> | <span data-ttu-id="723b5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="723b5-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="723b5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="723b5-125">Authorization</span></span>  | <span data-ttu-id="723b5-126">string</span><span class="sxs-lookup"><span data-stu-id="723b5-126">string</span></span>  | <span data-ttu-id="723b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="723b5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="723b5-129">Accept</span><span class="sxs-lookup"><span data-stu-id="723b5-129">Accept</span></span> | <span data-ttu-id="723b5-130">строка</span><span class="sxs-lookup"><span data-stu-id="723b5-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="723b5-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="723b5-131">Request body</span></span>
<span data-ttu-id="723b5-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="723b5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="723b5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="723b5-133">Response</span></span>

<span data-ttu-id="723b5-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="723b5-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="723b5-135">Пример</span><span class="sxs-lookup"><span data-stu-id="723b5-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="723b5-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="723b5-136">Request</span></span>
<span data-ttu-id="723b5-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="723b5-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="723b5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="723b5-138">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="723b5-139">C#</span><span class="sxs-lookup"><span data-stu-id="723b5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="723b5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="723b5-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="723b5-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="723b5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="723b5-142">Java</span><span class="sxs-lookup"><span data-stu-id="723b5-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebooks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="723b5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="723b5-143">Response</span></span>
<span data-ttu-id="723b5-p103">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="723b5-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
