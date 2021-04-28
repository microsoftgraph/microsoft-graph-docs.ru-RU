---
title: Перечисление createdObjects
description: Получение списка созданных пользователем объектов каталога.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 55d8d87378eddf3b176d0138ed2f8c32b659142c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049375"
---
# <a name="list-createdobjects"></a><span data-ttu-id="70acd-103">Перечисление createdObjects</span><span class="sxs-lookup"><span data-stu-id="70acd-103">List createdObjects</span></span>

<span data-ttu-id="70acd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70acd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70acd-105">Получение списка созданных пользователем объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="70acd-105">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="70acd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70acd-106">Permissions</span></span>
<span data-ttu-id="70acd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70acd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70acd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70acd-109">Permission type</span></span>      | <span data-ttu-id="70acd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70acd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70acd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70acd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="70acd-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70acd-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="70acd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70acd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70acd-114">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70acd-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="70acd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70acd-115">Application</span></span> | <span data-ttu-id="70acd-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70acd-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="70acd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70acd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="70acd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70acd-118">Optional query parameters</span></span>
<span data-ttu-id="70acd-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="70acd-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="70acd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70acd-120">Request headers</span></span>
| <span data-ttu-id="70acd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70acd-121">Header</span></span>       | <span data-ttu-id="70acd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="70acd-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70acd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70acd-123">Authorization</span></span>  | <span data-ttu-id="70acd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70acd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="70acd-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70acd-126">Content-Type</span></span>  | <span data-ttu-id="70acd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="70acd-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70acd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70acd-128">Request body</span></span>
<span data-ttu-id="70acd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70acd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70acd-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="70acd-130">Response</span></span>

<span data-ttu-id="70acd-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70acd-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70acd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="70acd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70acd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="70acd-133">Request</span></span>
<span data-ttu-id="70acd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70acd-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70acd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="70acd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="70acd-136">C#</span><span class="sxs-lookup"><span data-stu-id="70acd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70acd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70acd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70acd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70acd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70acd-139">Java</span><span class="sxs-lookup"><span data-stu-id="70acd-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="70acd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="70acd-140">Response</span></span>
<span data-ttu-id="70acd-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70acd-141">Here is an example of the response.</span></span> <span data-ttu-id="70acd-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="70acd-142">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
