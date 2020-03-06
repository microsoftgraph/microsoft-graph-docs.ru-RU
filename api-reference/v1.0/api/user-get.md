---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 60baf9c66ffa77399694a8e9a0ef846fe3be1cd6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509190"
---
# <a name="get-a-user"></a><span data-ttu-id="09414-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="09414-103">Get a user</span></span>

<span data-ttu-id="09414-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09414-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09414-105">Получение свойств и связей объекта user.</span><span class="sxs-lookup"><span data-stu-id="09414-105">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="09414-p101">Примечание. При получении пользователя возвращается только стандартный набор свойств (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). С помощью параметра `$select` можно получить остальные свойства и связи объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="09414-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09414-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09414-108">Permissions</span></span>
<span data-ttu-id="09414-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09414-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09414-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09414-111">Permission type</span></span>      | <span data-ttu-id="09414-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09414-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09414-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09414-113">Delegated (work or school account)</span></span> | <span data-ttu-id="09414-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09414-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="09414-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09414-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09414-116">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09414-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="09414-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09414-117">Application</span></span> | <span data-ttu-id="09414-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09414-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09414-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09414-119">HTTP request</span></span>
<span data-ttu-id="09414-120">Для определенного пользователя:</span><span class="sxs-lookup"><span data-stu-id="09414-120">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="09414-121">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="09414-121">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09414-122">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="09414-122">Optional query parameters</span></span>
<span data-ttu-id="09414-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="09414-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="09414-124">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="09414-124">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="09414-125">Чтобы возвратить альтернативный набор свойств, необходимо указать нужный набор свойств [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="09414-125">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="09414-126">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="09414-126">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="09414-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09414-127">Request headers</span></span>
| <span data-ttu-id="09414-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09414-128">Header</span></span>       | <span data-ttu-id="09414-129">Значение</span><span class="sxs-lookup"><span data-stu-id="09414-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="09414-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09414-130">Authorization</span></span>  | <span data-ttu-id="09414-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09414-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09414-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09414-133">Content-Type</span></span>   | <span data-ttu-id="09414-134">application/json</span><span class="sxs-lookup"><span data-stu-id="09414-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="09414-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09414-135">Request body</span></span>
<span data-ttu-id="09414-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09414-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09414-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="09414-137">Response</span></span>

<span data-ttu-id="09414-138">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="09414-138">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="09414-139">В случае успешной обработки запроса этот метод возвращает `202 Accepted`, но серверу требуется дополнительное время для выполнения соответствующих фоновых операций.</span><span class="sxs-lookup"><span data-stu-id="09414-139">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="examples"></a><span data-ttu-id="09414-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="09414-140">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="09414-141">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="09414-141">Example 1: Standard users request</span></span>

<span data-ttu-id="09414-142">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="09414-142">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="09414-143">В этом примере показаны запрос и ответ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="09414-143">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="09414-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="09414-144">Response</span></span>

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


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="09414-145">Пример 2. Запрос для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="09414-145">Example 2: Signed-in user request</span></span>

<span data-ttu-id="09414-146">Вы можете получить информацию о вошедшем пользователе, заменив `/users/{id | userPrincipalName}` на `/me`.</span><span class="sxs-lookup"><span data-stu-id="09414-146">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="09414-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="09414-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="09414-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="09414-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me
```
# <a name="c"></a>[<span data-ttu-id="09414-149">C#</span><span class="sxs-lookup"><span data-stu-id="09414-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09414-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09414-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09414-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09414-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="09414-152">Java</span><span class="sxs-lookup"><span data-stu-id="09414-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="09414-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="09414-153">Response</span></span>

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

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="09414-154">Пример 3. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="09414-154">Example 3: Users request using $select</span></span>

<span data-ttu-id="09414-155">Если вам нужен другой набор свойств, можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="09414-155">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="09414-156">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="09414-156">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="09414-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="09414-157">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="09414-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="09414-158">Response</span></span>
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
