---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8024db6c3f3263becdf7b22ca388a5c7462ce4c1
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351337"
---
# <a name="get-a-user"></a><span data-ttu-id="181d0-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="181d0-103">Get a user</span></span>

<span data-ttu-id="181d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="181d0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="181d0-105">Получение свойств и связей объекта user.</span><span class="sxs-lookup"><span data-stu-id="181d0-105">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="181d0-p101">Примечание. При получении пользователя возвращается только стандартный набор свойств (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). С помощью параметра `$select` можно получить остальные свойства и связи объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="181d0-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="181d0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="181d0-108">Permissions</span></span>
<span data-ttu-id="181d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="181d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="181d0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="181d0-111">Permission type</span></span>      | <span data-ttu-id="181d0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="181d0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="181d0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="181d0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="181d0-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="181d0-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="181d0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="181d0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="181d0-116">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="181d0-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="181d0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="181d0-117">Application</span></span> | <span data-ttu-id="181d0-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181d0-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="181d0-119">Для вызова конечной точки `/me` требуется вход пользователя и, следовательно, делегированное разрешение.</span><span class="sxs-lookup"><span data-stu-id="181d0-119">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="181d0-120">Разрешения приложений не поддерживаются при использовании конечной точки `/me`.</span><span class="sxs-lookup"><span data-stu-id="181d0-120">Application permissions are not supported when using the `/me` endpoint.</span></span>

## <a name="http-request"></a><span data-ttu-id="181d0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="181d0-121">HTTP request</span></span>
<span data-ttu-id="181d0-122">Для определенного пользователя:</span><span class="sxs-lookup"><span data-stu-id="181d0-122">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

><span data-ttu-id="181d0-123">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="181d0-123">**Note:**</span></span>
> + <span data-ttu-id="181d0-p104">Если **userPrincipalName** начинается с символа `$`, нужно удалить косую черту (/) после `/users` и заключить **userPrincipalName** в скобки и одиночные кавычки. Например, `/users('$AdeleVance@contoso.com')`. Дополнительные сведения см. в списке [известных проблем](/graph/known-issues#users).</span><span class="sxs-lookup"><span data-stu-id="181d0-p104">When the **userPrincipalName** begins with a `$` character, remove the slash (/) after `/users` and enclose the **userPrincipalName** in parentheses and single quotes. For example, `/users('$AdeleVance@contoso.com')`. For details, see the [known issues](/graph/known-issues#users) list.</span></span>
> + <span data-ttu-id="181d0-127">Чтобы запросить пользователя B2B с помощью **userPrincipalName**, закодируйте хэш-символ (#).</span><span class="sxs-lookup"><span data-stu-id="181d0-127">To query a B2B user using the **userPrincipalName**, encode the hash (#) character.</span></span> <span data-ttu-id="181d0-128">То есть замените символ `#` на `%23`.</span><span class="sxs-lookup"><span data-stu-id="181d0-128">That is, replace the `#` symbol with `%23`.</span></span> <span data-ttu-id="181d0-129">Например, `/users/AdeleVance_adatum.com%23EXT%23@contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="181d0-129">For example, `/users/AdeleVance_adatum.com%23EXT%23@contoso.com`.</span></span>

<span data-ttu-id="181d0-130">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="181d0-130">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="181d0-131">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="181d0-131">Optional query parameters</span></span>
<span data-ttu-id="181d0-132">Этот метод поддерживает `$select` [параметр запроса OData](/graph/query-parameters) для получения конкретных свойств пользователя, в том числе тех, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="181d0-132">This method supports the `$select` [OData query parameter](/graph/query-parameters) to retrieve specific user properties, including those that are not returned by default.</span></span>

<span data-ttu-id="181d0-133">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="181d0-133">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="181d0-134">Чтобы возвратить альтернативный набор свойств, необходимо указать нужный набор свойств [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="181d0-134">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="181d0-135">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="181d0-135">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="181d0-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="181d0-136">Request headers</span></span>
| <span data-ttu-id="181d0-137">Заголовок</span><span class="sxs-lookup"><span data-stu-id="181d0-137">Header</span></span>       | <span data-ttu-id="181d0-138">Значение</span><span class="sxs-lookup"><span data-stu-id="181d0-138">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="181d0-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="181d0-139">Authorization</span></span>  | <span data-ttu-id="181d0-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="181d0-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="181d0-142">Content-Type</span><span class="sxs-lookup"><span data-stu-id="181d0-142">Content-Type</span></span>   | <span data-ttu-id="181d0-143">application/json</span><span class="sxs-lookup"><span data-stu-id="181d0-143">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="181d0-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="181d0-144">Request body</span></span>
<span data-ttu-id="181d0-145">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="181d0-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="181d0-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="181d0-146">Response</span></span>

<span data-ttu-id="181d0-147">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="181d0-147">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span> <span data-ttu-id="181d0-148">Он возвращает свойства по умолчанию, если не используется `$select` для указания конкретных свойств.</span><span class="sxs-lookup"><span data-stu-id="181d0-148">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

<span data-ttu-id="181d0-149">В случае успешной обработки запроса этот метод возвращает `202 Accepted`, но серверу требуется дополнительное время для выполнения соответствующих фоновых операций.</span><span class="sxs-lookup"><span data-stu-id="181d0-149">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="examples"></a><span data-ttu-id="181d0-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="181d0-150">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="181d0-151">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="181d0-151">Example 1: Standard users request</span></span>

<span data-ttu-id="181d0-p109">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_). В этом примере показаны запрос и отклик по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="181d0-p109">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ). This example illustrates the default request and response.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_user_1"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="181d0-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="181d0-154">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "+1 425 555 0109"
   ],
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "jobTitle": "Retail Manager",
   "mail": "AdeleV@contoso.onmicrosoft.com",
   "mobilePhone": "+1 425 555 0109",
   "officeLocation": "18/2111",
   "preferredLanguage": "en-US",
   "surname": "Vance",
   "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
   "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="181d0-155">Пример 2. Запрос для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="181d0-155">Example 2: Signed-in user request</span></span>

<span data-ttu-id="181d0-156">Вы можете получить информацию о вошедшем пользователе, заменив `/users/{id | userPrincipalName}` на `/me`.</span><span class="sxs-lookup"><span data-stu-id="181d0-156">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="181d0-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="181d0-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="181d0-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="181d0-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me
```
# <a name="c"></a>[<span data-ttu-id="181d0-159">C#</span><span class="sxs-lookup"><span data-stu-id="181d0-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="181d0-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="181d0-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="181d0-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="181d0-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="181d0-162">Java</span><span class="sxs-lookup"><span data-stu-id="181d0-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="181d0-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="181d0-163">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "+1 425 555 0109"
   ],
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "jobTitle": "Retail Manager",
   "mail": "AdeleV@contoso.onmicrosoft.com",
   "mobilePhone": "+1 425 555 0109",
   "officeLocation": "18/2111",
   "preferredLanguage": "en-US",
   "surname": "Vance",
   "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
   "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="181d0-164">Пример 3. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="181d0-164">Example 3: Users request using $select</span></span>

<span data-ttu-id="181d0-165">Если вам нужен другой набор свойств, можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="181d0-165">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="181d0-166">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="181d0-166">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="181d0-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="181d0-167">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="181d0-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="181d0-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_2"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
# <a name="c"></a>[<span data-ttu-id="181d0-169">C#</span><span class="sxs-lookup"><span data-stu-id="181d0-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="181d0-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="181d0-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="181d0-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="181d0-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="181d0-172">Java</span><span class="sxs-lookup"><span data-stu-id="181d0-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="181d0-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="181d0-173">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "postalCode": "98004"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
