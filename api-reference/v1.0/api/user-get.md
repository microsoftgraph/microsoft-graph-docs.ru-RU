---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93bb0768a9912a8ea0991e52d01428d9569c663b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886208"
---
# <a name="get-a-user"></a><span data-ttu-id="e8205-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="e8205-103">Get a user</span></span>

<span data-ttu-id="e8205-104">Получение свойств и связей объекта пользователей.</span><span class="sxs-lookup"><span data-stu-id="e8205-104">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="e8205-p101">Примечание. При получении пользователя возвращается только стандартный набор свойств (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). С помощью параметра `$select` можно получить остальные свойства и связи объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="e8205-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8205-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8205-107">Permissions</span></span>
<span data-ttu-id="e8205-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8205-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8205-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8205-110">Permission type</span></span>      | <span data-ttu-id="e8205-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8205-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8205-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8205-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8205-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8205-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e8205-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8205-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8205-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8205-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="e8205-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8205-116">Application</span></span> | <span data-ttu-id="e8205-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8205-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8205-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8205-118">HTTP request</span></span>
<span data-ttu-id="e8205-119">Для определенного пользователя:</span><span class="sxs-lookup"><span data-stu-id="e8205-119">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="e8205-120">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="e8205-120">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8205-121">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="e8205-121">Optional query parameters</span></span>
<span data-ttu-id="e8205-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e8205-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e8205-123">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="e8205-123">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="e8205-124">Чтобы возвратить альтернативный набор свойств, необходимо указать нужный набор свойств [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="e8205-124">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="e8205-125">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="e8205-125">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8205-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8205-126">Request headers</span></span>
| <span data-ttu-id="e8205-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8205-127">Header</span></span>       | <span data-ttu-id="e8205-128">Значение</span><span class="sxs-lookup"><span data-stu-id="e8205-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e8205-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8205-129">Authorization</span></span>  | <span data-ttu-id="e8205-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8205-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8205-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8205-132">Content-Type</span></span>   | <span data-ttu-id="e8205-133">application/json</span><span class="sxs-lookup"><span data-stu-id="e8205-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8205-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8205-134">Request body</span></span>
<span data-ttu-id="e8205-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8205-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8205-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8205-136">Response</span></span>

<span data-ttu-id="e8205-137">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e8205-137">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="e8205-138">В случае успешной обработки запроса этот метод возвращает `202 Accepted`, но серверу требуется дополнительное время для выполнения соответствующих фоновых операций.</span><span class="sxs-lookup"><span data-stu-id="e8205-138">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="examples"></a><span data-ttu-id="e8205-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8205-139">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="e8205-140">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="e8205-140">Example 1: Standard users request</span></span>

<span data-ttu-id="e8205-141">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="e8205-141">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="e8205-142">В этом примере показаны запрос и ответ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e8205-142">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="e8205-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8205-143">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

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
```


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="e8205-144">Пример 2. Запрос для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="e8205-144">Example 2: Signed-in user request</span></span>

<span data-ttu-id="e8205-145">Вы можете получить информацию о вошедшем пользователе, заменив `/users/{id | userPrincipalName}` на `/me`.</span><span class="sxs-lookup"><span data-stu-id="e8205-145">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="e8205-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8205-146">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e8205-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8205-147">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8205-148">C#</span><span class="sxs-lookup"><span data-stu-id="e8205-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8205-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8205-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8205-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8205-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e8205-151">Java</span><span class="sxs-lookup"><span data-stu-id="e8205-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e8205-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8205-152">Response</span></span>

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
```

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="e8205-153">Пример 3. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="e8205-153">Example 3: Users request using $select</span></span>

<span data-ttu-id="e8205-154">Если вам нужен другой набор свойств, можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="e8205-154">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="e8205-155">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="e8205-155">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="e8205-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8205-156">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="e8205-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8205-157">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "postalCode": "postalCode-value"
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
