---
title: Получение руководителя
description: Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный в качестве руководителя пользователя.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5cd3cf7139723fc9555dc111a5e409b4ebef4f17
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865134"
---
# <a name="list-manager"></a><span data-ttu-id="30162-104">Получение руководителя</span><span class="sxs-lookup"><span data-stu-id="30162-104">List manager</span></span>

<span data-ttu-id="30162-105">Получение руководителя пользователя.</span><span class="sxs-lookup"><span data-stu-id="30162-105">Get user's manager.</span></span> <span data-ttu-id="30162-106">Возвращает пользователя или контакт организации, назначенный в качестве руководителя пользователя.</span><span class="sxs-lookup"><span data-stu-id="30162-106">Returns the user or organizational contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="30162-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30162-107">Permissions</span></span>
<span data-ttu-id="30162-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30162-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30162-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30162-110">Permission type</span></span>      | <span data-ttu-id="30162-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30162-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30162-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30162-112">Delegated (work or school account)</span></span> | <span data-ttu-id="30162-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="30162-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="30162-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30162-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30162-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30162-115">Not supported.</span></span>    |
|<span data-ttu-id="30162-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30162-116">Application</span></span> | <span data-ttu-id="30162-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30162-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="30162-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30162-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="30162-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="30162-119">Optional query parameters</span></span>
<span data-ttu-id="30162-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="30162-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="30162-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30162-121">Request headers</span></span>
| <span data-ttu-id="30162-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30162-122">Header</span></span>       | <span data-ttu-id="30162-123">Значение</span><span class="sxs-lookup"><span data-stu-id="30162-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="30162-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30162-124">Authorization</span></span>  | <span data-ttu-id="30162-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30162-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="30162-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30162-127">Request body</span></span>
<span data-ttu-id="30162-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30162-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30162-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="30162-129">Response</span></span>

<span data-ttu-id="30162-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30162-130">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30162-131">Пример</span><span class="sxs-lookup"><span data-stu-id="30162-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30162-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="30162-132">Request</span></span>
<span data-ttu-id="30162-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30162-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="30162-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="30162-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="30162-135">C#</span><span class="sxs-lookup"><span data-stu-id="30162-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30162-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30162-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="30162-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30162-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="30162-138">Java</span><span class="sxs-lookup"><span data-stu-id="30162-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="30162-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="30162-139">Response</span></span>
<span data-ttu-id="30162-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30162-140">The following is an example of the response.</span></span>
><span data-ttu-id="30162-141">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="30162-141">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
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
