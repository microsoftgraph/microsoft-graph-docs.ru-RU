---
title: Список записных книжек
description: Получение списка объектов записных книжек.
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 819120fbd4e91db4edbeff89315396ce3e41e36c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892823"
---
# <a name="list-notebooks"></a><span data-ttu-id="01bcd-103">Список записных книжек</span><span class="sxs-lookup"><span data-stu-id="01bcd-103">List notebooks</span></span>

<span data-ttu-id="01bcd-104">Получение списка объектов [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="01bcd-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="01bcd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01bcd-105">Permissions</span></span>
<span data-ttu-id="01bcd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01bcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01bcd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01bcd-108">Permission type</span></span>      | <span data-ttu-id="01bcd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01bcd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01bcd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01bcd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="01bcd-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bcd-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="01bcd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01bcd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01bcd-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01bcd-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="01bcd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01bcd-114">Application</span></span> | <span data-ttu-id="01bcd-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bcd-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01bcd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01bcd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01bcd-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01bcd-117">Optional query parameters</span></span>
<span data-ttu-id="01bcd-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="01bcd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="01bcd-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="01bcd-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="01bcd-120">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="01bcd-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01bcd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01bcd-121">Request headers</span></span>
| <span data-ttu-id="01bcd-122">Имя</span><span class="sxs-lookup"><span data-stu-id="01bcd-122">Name</span></span>       | <span data-ttu-id="01bcd-123">Тип</span><span class="sxs-lookup"><span data-stu-id="01bcd-123">Type</span></span> | <span data-ttu-id="01bcd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="01bcd-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01bcd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="01bcd-125">Authorization</span></span>  | <span data-ttu-id="01bcd-126">string</span><span class="sxs-lookup"><span data-stu-id="01bcd-126">string</span></span>  | <span data-ttu-id="01bcd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01bcd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01bcd-129">Accept</span><span class="sxs-lookup"><span data-stu-id="01bcd-129">Accept</span></span> | <span data-ttu-id="01bcd-130">строка</span><span class="sxs-lookup"><span data-stu-id="01bcd-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="01bcd-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01bcd-131">Request body</span></span>
<span data-ttu-id="01bcd-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01bcd-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01bcd-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="01bcd-133">Response</span></span>

<span data-ttu-id="01bcd-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01bcd-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01bcd-135">Пример</span><span class="sxs-lookup"><span data-stu-id="01bcd-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01bcd-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="01bcd-136">Request</span></span>
<span data-ttu-id="01bcd-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01bcd-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="01bcd-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="01bcd-138">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="01bcd-139">C#</span><span class="sxs-lookup"><span data-stu-id="01bcd-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notebooks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01bcd-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01bcd-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notebooks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="01bcd-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01bcd-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notebooks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="01bcd-142">Java</span><span class="sxs-lookup"><span data-stu-id="01bcd-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-notebooks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="01bcd-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="01bcd-143">Response</span></span>
<span data-ttu-id="01bcd-p103">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01bcd-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
