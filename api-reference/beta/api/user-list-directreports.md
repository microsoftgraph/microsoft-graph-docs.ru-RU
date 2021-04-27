---
title: Список directReports
description: Получение подчиненных пользователя.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 9939d14a71c56e7920eed7755bcb4be8abfe2c58
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053365"
---
# <a name="list-directreports"></a><span data-ttu-id="2270b-103">Список directReports</span><span class="sxs-lookup"><span data-stu-id="2270b-103">List directReports</span></span>

<span data-ttu-id="2270b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2270b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2270b-105">Получение подчиненных пользователя.</span><span class="sxs-lookup"><span data-stu-id="2270b-105">Get a user's direct reports.</span></span> <span data-ttu-id="2270b-106">Возвращает пользователей и контакты, для которых данный пользователь назначен руководителем.</span><span class="sxs-lookup"><span data-stu-id="2270b-106">Returns the users and contacts for whom this user is assigned as manager.</span></span>

## <a name="permissions"></a><span data-ttu-id="2270b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2270b-107">Permissions</span></span>
<span data-ttu-id="2270b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2270b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2270b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2270b-110">Permission type</span></span>      | <span data-ttu-id="2270b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2270b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2270b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2270b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2270b-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2270b-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2270b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2270b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2270b-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2270b-115">Not supported</span></span> |
|<span data-ttu-id="2270b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2270b-116">Application</span></span> | <span data-ttu-id="2270b-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2270b-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2270b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2270b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2270b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2270b-119">Optional query parameters</span></span>
<span data-ttu-id="2270b-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2270b-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2270b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2270b-121">Request headers</span></span>
| <span data-ttu-id="2270b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2270b-122">Header</span></span>       | <span data-ttu-id="2270b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2270b-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="2270b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2270b-124">Authorization</span></span>  | <span data-ttu-id="2270b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2270b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2270b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2270b-127">Content-Type</span></span>   | <span data-ttu-id="2270b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2270b-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2270b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2270b-129">Request body</span></span>
<span data-ttu-id="2270b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2270b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2270b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2270b-131">Response</span></span>

<span data-ttu-id="2270b-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2270b-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2270b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2270b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2270b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2270b-134">Request</span></span>
<span data-ttu-id="2270b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2270b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2270b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2270b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/directReports
```
# <a name="c"></a>[<span data-ttu-id="2270b-137">C#</span><span class="sxs-lookup"><span data-stu-id="2270b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2270b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2270b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2270b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2270b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2270b-140">Java</span><span class="sxs-lookup"><span data-stu-id="2270b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2270b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2270b-141">Response</span></span>
<span data-ttu-id="2270b-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2270b-142">Here is an example of the response.</span></span> 

><span data-ttu-id="2270b-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2270b-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


