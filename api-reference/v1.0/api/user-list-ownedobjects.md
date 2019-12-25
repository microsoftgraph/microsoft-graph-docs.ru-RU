---
title: Список ownedObjects
description: Получение списка объектов каталога, принадлежащих пользователю.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1438eecbfadd5af320918d1b65a5721bf17c8d6b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863993"
---
# <a name="list-ownedobjects"></a><span data-ttu-id="81014-103">Список ownedObjects</span><span class="sxs-lookup"><span data-stu-id="81014-103">List ownedObjects</span></span>

<span data-ttu-id="81014-104">Получение списка объектов каталога, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="81014-104">Get the list of directory objects that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="81014-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81014-105">Permissions</span></span>
<span data-ttu-id="81014-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81014-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81014-108">Permission type</span></span>      | <span data-ttu-id="81014-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81014-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81014-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81014-110">Delegated (work or school account)</span></span> | <span data-ttu-id="81014-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81014-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81014-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81014-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81014-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81014-113">Not supported.</span></span>    |
|<span data-ttu-id="81014-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81014-114">Application</span></span> | <span data-ttu-id="81014-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81014-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="81014-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81014-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="81014-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81014-117">Optional query parameters</span></span>
<span data-ttu-id="81014-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="81014-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="81014-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81014-119">Request headers</span></span>
| <span data-ttu-id="81014-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81014-120">Header</span></span>       | <span data-ttu-id="81014-121">Значение</span><span class="sxs-lookup"><span data-stu-id="81014-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="81014-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81014-122">Authorization</span></span>  | <span data-ttu-id="81014-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81014-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="81014-125">Accept</span><span class="sxs-lookup"><span data-stu-id="81014-125">Accept</span></span>  | <span data-ttu-id="81014-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81014-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81014-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81014-127">Request body</span></span>
<span data-ttu-id="81014-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81014-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81014-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="81014-129">Response</span></span>

<span data-ttu-id="81014-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81014-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="81014-131">Пример</span><span class="sxs-lookup"><span data-stu-id="81014-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81014-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="81014-132">Request</span></span>
<span data-ttu-id="81014-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81014-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="81014-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="81014-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/ownedObjects
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="81014-135">C#</span><span class="sxs-lookup"><span data-stu-id="81014-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81014-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81014-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81014-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81014-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="81014-138">Java</span><span class="sxs-lookup"><span data-stu-id="81014-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ownedobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="81014-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="81014-139">Response</span></span>
<span data-ttu-id="81014-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81014-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
