---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 94ceebb51dfe1d43bea7404213ef8fdb56535701
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579783"
---
# <a name="get-a-user"></a><span data-ttu-id="3bb2c-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="3bb2c-103">Get a user</span></span>

<span data-ttu-id="3bb2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bb2c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3bb2c-105">Получение свойств и связей объекта user.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-105">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="3bb2c-p101">Примечание. При получении пользователя возвращается только стандартный набор свойств (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). С помощью параметра `$select` можно получить остальные свойства и связи объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="3bb2c-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bb2c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3bb2c-108">Permissions</span></span>
<span data-ttu-id="3bb2c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bb2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bb2c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bb2c-111">Permission type</span></span>      | <span data-ttu-id="3bb2c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bb2c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bb2c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bb2c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3bb2c-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3bb2c-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3bb2c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bb2c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bb2c-116">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bb2c-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="3bb2c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bb2c-117">Application</span></span> | <span data-ttu-id="3bb2c-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bb2c-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="3bb2c-119">Для вызова конечной точки `/me` требуется вход пользователя и, следовательно, делегированное разрешение.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-119">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="3bb2c-120">Разрешения приложений не поддерживаются при использовании конечной точки `/me`.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-120">Application permissions are not supported when using the `/me` endpoint.</span></span>

## <a name="http-request"></a><span data-ttu-id="3bb2c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bb2c-121">HTTP request</span></span>
<span data-ttu-id="3bb2c-122">Для определенного пользователя:</span><span class="sxs-lookup"><span data-stu-id="3bb2c-122">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
<span data-ttu-id="3bb2c-p104">Обратите внимание, что если **userPrincipalName** начинается с символа `$`, нужно удалить косую черту (/) после `/users` и заключить **userPrincipalName** в скобки и одиночные кавычки. Дополнительные сведения см. в списке [известных проблем](/graph/known-issues#users).</span><span class="sxs-lookup"><span data-stu-id="3bb2c-p104">Note that when the **userPrincipalName** begins with a `$` character, remove the slash (/) after `/users` and enclose the **userPrincipalName** in parentheses and single quotes. For details, see the [known issues](/graph/known-issues#users) list.</span></span>

<span data-ttu-id="3bb2c-125">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="3bb2c-125">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3bb2c-126">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="3bb2c-126">Optional query parameters</span></span>
<span data-ttu-id="3bb2c-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="3bb2c-128">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="3bb2c-128">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="3bb2c-129">Чтобы возвратить альтернативный набор свойств, необходимо указать нужный набор свойств [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-129">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="3bb2c-130">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-130">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bb2c-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bb2c-131">Request headers</span></span>
| <span data-ttu-id="3bb2c-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3bb2c-132">Header</span></span>       | <span data-ttu-id="3bb2c-133">Значение</span><span class="sxs-lookup"><span data-stu-id="3bb2c-133">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="3bb2c-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bb2c-134">Authorization</span></span>  | <span data-ttu-id="3bb2c-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3bb2c-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3bb2c-137">Content-Type</span></span>   | <span data-ttu-id="3bb2c-138">application/json</span><span class="sxs-lookup"><span data-stu-id="3bb2c-138">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bb2c-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3bb2c-139">Request body</span></span>
<span data-ttu-id="3bb2c-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bb2c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bb2c-141">Response</span></span>

<span data-ttu-id="3bb2c-142">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-142">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="3bb2c-143">В случае успешной обработки запроса этот метод возвращает `202 Accepted`, но серверу требуется дополнительное время для выполнения соответствующих фоновых операций.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-143">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="examples"></a><span data-ttu-id="3bb2c-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="3bb2c-144">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="3bb2c-145">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="3bb2c-145">Example 1: Standard users request</span></span>

<span data-ttu-id="3bb2c-146">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="3bb2c-146">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="3bb2c-147">В этом примере показаны запрос и ответ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-147">This example illustrates the default request and response.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_user_1"
} -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="3bb2c-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="3bb2c-148">Response</span></span>

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


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="3bb2c-149">Пример 2. Запрос для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="3bb2c-149">Example 2: Signed-in user request</span></span>

<span data-ttu-id="3bb2c-150">Вы можете получить информацию о вошедшем пользователе, заменив `/users/{id | userPrincipalName}` на `/me`.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-150">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="3bb2c-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bb2c-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3bb2c-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bb2c-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me
```
# <a name="c"></a>[<span data-ttu-id="3bb2c-153">C#</span><span class="sxs-lookup"><span data-stu-id="3bb2c-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bb2c-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bb2c-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bb2c-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bb2c-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3bb2c-156">Java</span><span class="sxs-lookup"><span data-stu-id="3bb2c-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3bb2c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bb2c-157">Response</span></span>

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

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="3bb2c-158">Пример 3. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="3bb2c-158">Example 3: Users request using $select</span></span>

<span data-ttu-id="3bb2c-159">Если вам нужен другой набор свойств, можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-159">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="3bb2c-160">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="3bb2c-160">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="3bb2c-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bb2c-161">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_2"
} -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="3bb2c-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bb2c-162">Response</span></span>
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
