---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 01c6f404dee2a9a6d5d8d95449fe5f1215a5241f
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522890"
---
# <a name="get-a-user"></a><span data-ttu-id="64c3f-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="64c3f-103">Get a user</span></span>

<span data-ttu-id="64c3f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64c3f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64c3f-105">Получение свойств и связей объекта user.</span><span class="sxs-lookup"><span data-stu-id="64c3f-105">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="64c3f-p101">Примечание. При получении пользователя возвращается только стандартный набор свойств (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). С помощью параметра `$select` можно получить остальные свойства и связи объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="64c3f-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64c3f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64c3f-108">Permissions</span></span>
<span data-ttu-id="64c3f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64c3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64c3f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64c3f-111">Permission type</span></span>      | <span data-ttu-id="64c3f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64c3f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64c3f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64c3f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="64c3f-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64c3f-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64c3f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64c3f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64c3f-116">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64c3f-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="64c3f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64c3f-117">Application</span></span> | <span data-ttu-id="64c3f-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c3f-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="64c3f-119">Для вызова конечной точки `/me` требуется вход пользователя и, следовательно, делегированное разрешение.</span><span class="sxs-lookup"><span data-stu-id="64c3f-119">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="64c3f-120">Разрешения приложений не поддерживаются при использовании конечной точки `/me`.</span><span class="sxs-lookup"><span data-stu-id="64c3f-120">Application permissions are not supported when using the `/me` endpoint.</span></span>

## <a name="http-request"></a><span data-ttu-id="64c3f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64c3f-121">HTTP request</span></span>
<span data-ttu-id="64c3f-122">Для определенного пользователя:</span><span class="sxs-lookup"><span data-stu-id="64c3f-122">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="64c3f-123">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="64c3f-123">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64c3f-124">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="64c3f-124">Optional query parameters</span></span>
<span data-ttu-id="64c3f-125">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64c3f-125">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="64c3f-126">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="64c3f-126">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="64c3f-127">Чтобы возвратить альтернативный набор свойств, необходимо указать нужный набор свойств [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="64c3f-127">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="64c3f-128">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="64c3f-128">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="64c3f-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64c3f-129">Request headers</span></span>
| <span data-ttu-id="64c3f-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64c3f-130">Header</span></span>       | <span data-ttu-id="64c3f-131">Значение</span><span class="sxs-lookup"><span data-stu-id="64c3f-131">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="64c3f-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64c3f-132">Authorization</span></span>  | <span data-ttu-id="64c3f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64c3f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64c3f-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64c3f-135">Content-Type</span></span>   | <span data-ttu-id="64c3f-136">application/json</span><span class="sxs-lookup"><span data-stu-id="64c3f-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="64c3f-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64c3f-137">Request body</span></span>
<span data-ttu-id="64c3f-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64c3f-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64c3f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c3f-139">Response</span></span>

<span data-ttu-id="64c3f-140">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="64c3f-140">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="64c3f-141">В случае успешной обработки запроса этот метод возвращает `202 Accepted`, но серверу требуется дополнительное время для выполнения соответствующих фоновых операций.</span><span class="sxs-lookup"><span data-stu-id="64c3f-141">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="examples"></a><span data-ttu-id="64c3f-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="64c3f-142">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="64c3f-143">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="64c3f-143">Example 1: Standard users request</span></span>

<span data-ttu-id="64c3f-144">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="64c3f-144">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="64c3f-145">В этом примере показаны запрос и ответ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="64c3f-145">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="64c3f-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="64c3f-146">Response</span></span>

<!-- { "blockType": "ignored" } -->
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


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="64c3f-147">Пример 2. Запрос для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="64c3f-147">Example 2: Signed-in user request</span></span>

<span data-ttu-id="64c3f-148">Вы можете получить информацию о вошедшем пользователе, заменив `/users/{id | userPrincipalName}` на `/me`.</span><span class="sxs-lookup"><span data-stu-id="64c3f-148">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="64c3f-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="64c3f-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="64c3f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="64c3f-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me
```
# <a name="c"></a>[<span data-ttu-id="64c3f-151">C#</span><span class="sxs-lookup"><span data-stu-id="64c3f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64c3f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64c3f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64c3f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64c3f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64c3f-154">Java</span><span class="sxs-lookup"><span data-stu-id="64c3f-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="64c3f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c3f-155">Response</span></span>

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

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="64c3f-156">Пример 3. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="64c3f-156">Example 3: Users request using $select</span></span>

<span data-ttu-id="64c3f-157">Если вам нужен другой набор свойств, можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="64c3f-157">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="64c3f-158">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="64c3f-158">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="64c3f-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="64c3f-159">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="64c3f-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c3f-160">Response</span></span>
<!-- { "blockType": "ignored" } -->
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
