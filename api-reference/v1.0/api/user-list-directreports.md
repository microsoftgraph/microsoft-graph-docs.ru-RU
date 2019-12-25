---
title: Список directReports
description: Получение подчиненных пользователя.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b86b0aaac9308f17079df1f696f7eb660ef814ac
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865148"
---
# <a name="list-directreports"></a><span data-ttu-id="e79a7-103">Список directReports</span><span class="sxs-lookup"><span data-stu-id="e79a7-103">List directReports</span></span>

<span data-ttu-id="e79a7-104">Получение подчиненных пользователя.</span><span class="sxs-lookup"><span data-stu-id="e79a7-104">Get a user's direct reports.</span></span>

## <a name="permissions"></a><span data-ttu-id="e79a7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e79a7-105">Permissions</span></span>
<span data-ttu-id="e79a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e79a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e79a7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e79a7-108">Permission type</span></span>      | <span data-ttu-id="e79a7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e79a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e79a7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e79a7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e79a7-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e79a7-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e79a7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e79a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e79a7-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e79a7-113">Not supported</span></span> |
|<span data-ttu-id="e79a7-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e79a7-114">Application</span></span> | <span data-ttu-id="e79a7-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e79a7-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e79a7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e79a7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e79a7-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e79a7-117">Optional query parameters</span></span>
<span data-ttu-id="e79a7-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e79a7-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e79a7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e79a7-119">Request headers</span></span>
| <span data-ttu-id="e79a7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e79a7-120">Header</span></span>       | <span data-ttu-id="e79a7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e79a7-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e79a7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e79a7-122">Authorization</span></span>  | <span data-ttu-id="e79a7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e79a7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e79a7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e79a7-125">Content-Type</span></span>   | <span data-ttu-id="e79a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e79a7-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e79a7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e79a7-127">Request body</span></span>
<span data-ttu-id="e79a7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e79a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e79a7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e79a7-129">Response</span></span>

<span data-ttu-id="e79a7-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e79a7-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e79a7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e79a7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e79a7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e79a7-132">Request</span></span>
<span data-ttu-id="e79a7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e79a7-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e79a7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e79a7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/directReports
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e79a7-135">C#</span><span class="sxs-lookup"><span data-stu-id="e79a7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e79a7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e79a7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e79a7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e79a7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e79a7-138">Java</span><span class="sxs-lookup"><span data-stu-id="e79a7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e79a7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e79a7-139">Response</span></span>
<span data-ttu-id="e79a7-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e79a7-140">Here is an example of the response.</span></span> 

><span data-ttu-id="e79a7-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e79a7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
