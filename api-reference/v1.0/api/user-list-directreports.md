---
title: Список directReports
description: Получение подчиненных пользователя.
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a5434dd1406afca1891695dd3d0b84c29f188a2a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050215"
---
# <a name="list-directreports"></a><span data-ttu-id="c7f0d-103">Список directReports</span><span class="sxs-lookup"><span data-stu-id="c7f0d-103">List directReports</span></span>

<span data-ttu-id="c7f0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7f0d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7f0d-105">Получение подчиненных пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7f0d-105">Get a user's direct reports.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7f0d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7f0d-106">Permissions</span></span>
<span data-ttu-id="c7f0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7f0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7f0d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7f0d-109">Permission type</span></span>      | <span data-ttu-id="c7f0d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7f0d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7f0d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7f0d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7f0d-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c7f0d-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c7f0d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7f0d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7f0d-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c7f0d-114">Not supported</span></span> |
|<span data-ttu-id="c7f0d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7f0d-115">Application</span></span> | <span data-ttu-id="c7f0d-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7f0d-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c7f0d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7f0d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c7f0d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7f0d-118">Optional query parameters</span></span>
<span data-ttu-id="c7f0d-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c7f0d-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7f0d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7f0d-120">Request headers</span></span>
| <span data-ttu-id="c7f0d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7f0d-121">Header</span></span>       | <span data-ttu-id="c7f0d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7f0d-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="c7f0d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7f0d-123">Authorization</span></span>  | <span data-ttu-id="c7f0d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7f0d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c7f0d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7f0d-126">Content-Type</span></span>   | <span data-ttu-id="c7f0d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c7f0d-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7f0d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7f0d-128">Request body</span></span>
<span data-ttu-id="c7f0d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7f0d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7f0d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7f0d-130">Response</span></span>

<span data-ttu-id="c7f0d-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7f0d-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7f0d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c7f0d-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7f0d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7f0d-133">Request</span></span>
<span data-ttu-id="c7f0d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7f0d-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7f0d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7f0d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/directReports
```
# <a name="c"></a>[<span data-ttu-id="c7f0d-136">C#</span><span class="sxs-lookup"><span data-stu-id="c7f0d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7f0d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7f0d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7f0d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7f0d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7f0d-139">Java</span><span class="sxs-lookup"><span data-stu-id="c7f0d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c7f0d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7f0d-140">Response</span></span>
<span data-ttu-id="c7f0d-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c7f0d-141">Here is an example of the response.</span></span> 

><span data-ttu-id="c7f0d-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c7f0d-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "a97733ce-92a4-4e7e-8d45-8e1f3e6a69d8"
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

