---
title: Список ownedObjects
description: Получение списка объектов каталога, принадлежащих пользователю.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 644b4692589d22d73c50e69f16293f265aa4e884
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703491"
---
# <a name="list-ownedobjects"></a><span data-ttu-id="477e1-103">Список ownedObjects</span><span class="sxs-lookup"><span data-stu-id="477e1-103">List ownedObjects</span></span>

<span data-ttu-id="477e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="477e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="477e1-105">Получение списка объектов каталога, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="477e1-105">Get the list of directory objects that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="477e1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="477e1-106">Permissions</span></span>
<span data-ttu-id="477e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="477e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="477e1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="477e1-109">Permission type</span></span>      | <span data-ttu-id="477e1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="477e1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="477e1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="477e1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="477e1-112">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="477e1-112">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="477e1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="477e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="477e1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="477e1-114">Not supported.</span></span>    |
|<span data-ttu-id="477e1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="477e1-115">Application</span></span> | <span data-ttu-id="477e1-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="477e1-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="477e1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="477e1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="477e1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="477e1-118">Optional query parameters</span></span>
<span data-ttu-id="477e1-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="477e1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="477e1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="477e1-120">Request headers</span></span>
| <span data-ttu-id="477e1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="477e1-121">Header</span></span>       | <span data-ttu-id="477e1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="477e1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="477e1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="477e1-123">Authorization</span></span>  | <span data-ttu-id="477e1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="477e1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="477e1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="477e1-126">Accept</span></span>  | <span data-ttu-id="477e1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="477e1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="477e1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="477e1-128">Request body</span></span>
<span data-ttu-id="477e1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="477e1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="477e1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="477e1-130">Response</span></span>

<span data-ttu-id="477e1-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="477e1-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="477e1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="477e1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="477e1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="477e1-133">Request</span></span>
<span data-ttu-id="477e1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="477e1-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="477e1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="477e1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="477e1-136">C#</span><span class="sxs-lookup"><span data-stu-id="477e1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="477e1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="477e1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="477e1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="477e1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="477e1-139">Java</span><span class="sxs-lookup"><span data-stu-id="477e1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ownedobjects-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="477e1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="477e1-140">Response</span></span>
<span data-ttu-id="477e1-p103">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="477e1-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
