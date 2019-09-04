---
title: Вывод записной книжки
description: Получение свойств и связей объекта записной книжки.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 2c7bf57d4bf04784ff0f872ed7cdd5a0a6f0123b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728652"
---
# <a name="get-notebook"></a><span data-ttu-id="23fbc-103">Вывод записной книжки</span><span class="sxs-lookup"><span data-stu-id="23fbc-103">Get notebook</span></span>

<span data-ttu-id="23fbc-104">Получение свойств и связей объекта записной [книжки](../resources/notebook.md) .</span><span class="sxs-lookup"><span data-stu-id="23fbc-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="23fbc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23fbc-105">Permissions</span></span>
<span data-ttu-id="23fbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23fbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23fbc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23fbc-108">Permission type</span></span>      | <span data-ttu-id="23fbc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23fbc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23fbc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23fbc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="23fbc-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23fbc-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="23fbc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23fbc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23fbc-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23fbc-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="23fbc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23fbc-114">Application</span></span> | <span data-ttu-id="23fbc-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23fbc-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23fbc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23fbc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23fbc-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23fbc-117">Optional query parameters</span></span>
<span data-ttu-id="23fbc-118">Этот метод поддерживает `select` `expand` [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="23fbc-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="23fbc-119">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="23fbc-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23fbc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23fbc-120">Request headers</span></span>
| <span data-ttu-id="23fbc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="23fbc-121">Name</span></span>       | <span data-ttu-id="23fbc-122">Тип</span><span class="sxs-lookup"><span data-stu-id="23fbc-122">Type</span></span> | <span data-ttu-id="23fbc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="23fbc-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23fbc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="23fbc-124">Authorization</span></span>  | <span data-ttu-id="23fbc-125">string</span><span class="sxs-lookup"><span data-stu-id="23fbc-125">string</span></span>  | <span data-ttu-id="23fbc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23fbc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23fbc-128">Accept</span><span class="sxs-lookup"><span data-stu-id="23fbc-128">Accept</span></span> | <span data-ttu-id="23fbc-129">строка</span><span class="sxs-lookup"><span data-stu-id="23fbc-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="23fbc-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23fbc-130">Request body</span></span>
<span data-ttu-id="23fbc-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23fbc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23fbc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="23fbc-132">Response</span></span>

<span data-ttu-id="23fbc-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="23fbc-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23fbc-134">Пример</span><span class="sxs-lookup"><span data-stu-id="23fbc-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23fbc-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="23fbc-135">Request</span></span>
<span data-ttu-id="23fbc-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23fbc-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="23fbc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="23fbc-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23fbc-138">C#</span><span class="sxs-lookup"><span data-stu-id="23fbc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23fbc-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23fbc-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23fbc-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="23fbc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="23fbc-141">Java</span><span class="sxs-lookup"><span data-stu-id="23fbc-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="23fbc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="23fbc-142">Response</span></span>
<span data-ttu-id="23fbc-p103">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23fbc-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
