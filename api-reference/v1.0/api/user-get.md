---
title: Получение пользователя
description: Получение свойств и связей объекта пользователей.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc408abf60ad42f564c4c36a37151db122ad573d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984152"
---
# <a name="get-a-user"></a><span data-ttu-id="1be28-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="1be28-103">Get a user</span></span>

<span data-ttu-id="1be28-104">Получение свойств и связей объекта пользователей.</span><span class="sxs-lookup"><span data-stu-id="1be28-104">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="1be28-p101">Примечание. При получении пользователя возвращается только стандартный набор свойств (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). С помощью параметра `$select` можно получить остальные свойства и связи объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="1be28-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1be28-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1be28-107">Permissions</span></span>
<span data-ttu-id="1be28-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1be28-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1be28-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1be28-110">Permission type</span></span>      | <span data-ttu-id="1be28-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1be28-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1be28-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1be28-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1be28-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1be28-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1be28-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1be28-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1be28-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1be28-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="1be28-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1be28-116">Application</span></span> | <span data-ttu-id="1be28-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1be28-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1be28-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1be28-118">HTTP request</span></span>
<span data-ttu-id="1be28-119">Для конкретного пользователя.<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="1be28-119">For a specific user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="1be28-120">Для пользователя выполнил вход.<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="1be28-120">For the signed-in user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1be28-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1be28-121">Optional query parameters</span></span>
<span data-ttu-id="1be28-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1be28-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1be28-123">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="1be28-123">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="1be28-124">Чтобы возвратить альтернативный набор свойств, необходимо указать нужный набор свойств [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="1be28-124">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="1be28-125">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="1be28-125">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="1be28-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1be28-126">Request headers</span></span>
| <span data-ttu-id="1be28-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1be28-127">Header</span></span>       | <span data-ttu-id="1be28-128">Значение</span><span class="sxs-lookup"><span data-stu-id="1be28-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="1be28-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1be28-129">Authorization</span></span>  | <span data-ttu-id="1be28-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1be28-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1be28-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1be28-132">Content-Type</span></span>   | <span data-ttu-id="1be28-133">application/json</span><span class="sxs-lookup"><span data-stu-id="1be28-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1be28-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1be28-134">Request body</span></span>
<span data-ttu-id="1be28-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1be28-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1be28-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1be28-136">Response</span></span>

<span data-ttu-id="1be28-137">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1be28-137">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1be28-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="1be28-138">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="1be28-139">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="1be28-139">Example 1: Standard users request</span></span>

<span data-ttu-id="1be28-140">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="1be28-140">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="1be28-141">В этом примере показаны запрос и ответ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1be28-141">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="1be28-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="1be28-142">Response</span></span>

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


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="1be28-143">Пример 2. Запрос для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="1be28-143">Example 2: Signed-in user request</span></span>

<span data-ttu-id="1be28-144">Вы можете получить информацию о вошедшем пользователе, заменив `/users/{id | userPrincipalName}` на `/me`.</span><span class="sxs-lookup"><span data-stu-id="1be28-144">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="1be28-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="1be28-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="1be28-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="1be28-146">Response</span></span>

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

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="1be28-147">Пример 3. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="1be28-147">Example 3: Users request using $select</span></span>

<span data-ttu-id="1be28-148">Если вам нужен другой набор свойств, можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="1be28-148">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="1be28-149">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="1be28-149">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="1be28-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="1be28-150">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="1be28-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="1be28-151">Response</span></span>
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
  "tocPath": ""
}-->
