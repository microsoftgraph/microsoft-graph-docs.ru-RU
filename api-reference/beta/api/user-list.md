---
title: Перечисление пользователей
description: Получение списка объектов user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92ad556051ddddaa767384e46c92b894e152883c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937471"
---
# <a name="list-users"></a><span data-ttu-id="6c4e6-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="6c4e6-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c4e6-104">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="6c4e6-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c4e6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c4e6-105">Permissions</span></span>

<span data-ttu-id="6c4e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c4e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c4e6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c4e6-108">Permission type</span></span>      | <span data-ttu-id="6c4e6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c4e6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c4e6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c4e6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6c4e6-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6c4e6-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6c4e6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c4e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c4e6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-113">Not supported.</span></span>    |
|<span data-ttu-id="6c4e6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c4e6-114">Application</span></span> | <span data-ttu-id="6c4e6-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c4e6-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c4e6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c4e6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c4e6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6c4e6-117">Optional query parameters</span></span>

<span data-ttu-id="6c4e6-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c4e6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c4e6-119">Request headers</span></span>
| <span data-ttu-id="6c4e6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c4e6-120">Header</span></span>        | <span data-ttu-id="6c4e6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6c4e6-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="6c4e6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c4e6-122">Authorization</span></span> | <span data-ttu-id="6c4e6-123">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="6c4e6-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="6c4e6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c4e6-124">Content-Type</span></span>  | <span data-ttu-id="6c4e6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c4e6-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="6c4e6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c4e6-126">Request body</span></span>

<span data-ttu-id="6c4e6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c4e6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c4e6-128">Response</span></span>

<span data-ttu-id="6c4e6-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c4e6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6c4e6-130">Example</span></span>

### <a name="example-1-list-all-users"></a><span data-ttu-id="6c4e6-131">Пример 1. Список всех пользователей</span><span class="sxs-lookup"><span data-stu-id="6c4e6-131">Example 1: List all users</span></span>

#### <a name="request"></a><span data-ttu-id="6c4e6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c4e6-132">Request</span></span>

<span data-ttu-id="6c4e6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6c4e6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c4e6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6c4e6-135">C#</span><span class="sxs-lookup"><span data-stu-id="6c4e6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c4e6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c4e6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6c4e6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c4e6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6c4e6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c4e6-138">Response</span></span>

<span data-ttu-id="6c4e6-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-139">The following is an example of the response.</span></span> 
><span data-ttu-id="6c4e6-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="6c4e6-142">Пример 2. Поиск учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="6c4e6-142">Example 2: Find a user account using a sign-in name</span></span>

<span data-ttu-id="6c4e6-143">Найдите учетную запись пользователя в клиенте B2C, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="6c4e6-143">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="6c4e6-144">Этот запрос может использоваться службой поддержки для поиска учетной записи пользователя в клиенте B2C (в данном примере клиентом B2C является contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="6c4e6-144">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="6c4e6-145">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-145">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="6c4e6-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c4e6-146">Request</span></span>

<span data-ttu-id="6c4e6-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6c4e6-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c4e6-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6c4e6-149">C#</span><span class="sxs-lookup"><span data-stu-id="6c4e6-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c4e6-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c4e6-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6c4e6-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c4e6-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6c4e6-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c4e6-152">Response</span></span>

<span data-ttu-id="6c4e6-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-153">The following is an example of the response.</span></span> 
> <span data-ttu-id="6c4e6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 108

{
  "value": [
    {
      "displayName": "John Smith",
      "id": "4c7be08b-361f-41a8-b1ef-1712f7a3dfb2"
    }
  ]
}
```

### <a name="example-3--list-users-including-their-last-sign-in-time"></a><span data-ttu-id="6c4e6-156">Пример 3. Перечисление пользователей с указанием времени их последнего входа в систему</span><span class="sxs-lookup"><span data-stu-id="6c4e6-156">Example 3:  List users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="6c4e6-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c4e6-157">Request</span></span>

<span data-ttu-id="6c4e6-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName, signInActivity
```

#### <a name="response"></a><span data-ttu-id="6c4e6-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c4e6-159">Response</span></span>

<span data-ttu-id="6c4e6-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-160">The following is an example of the response.</span></span> 
> <span data-ttu-id="6c4e6-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c4e6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(displayName,userPrincipalName,signInActivity)",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-07-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
