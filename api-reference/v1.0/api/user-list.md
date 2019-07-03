---
title: Перечисление пользователей
description: Получение списка объектов user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b83071ec8ff36fd197d9d27f9326e0019a5f131e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460177"
---
# <a name="list-users"></a><span data-ttu-id="e46ce-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="e46ce-103">List users</span></span>

<span data-ttu-id="e46ce-104">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="e46ce-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e46ce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e46ce-105">Permissions</span></span>

<span data-ttu-id="e46ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e46ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e46ce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e46ce-108">Permission type</span></span>      | <span data-ttu-id="e46ce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e46ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e46ce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e46ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e46ce-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e46ce-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e46ce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e46ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e46ce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e46ce-113">Not supported.</span></span>    |
|<span data-ttu-id="e46ce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e46ce-114">Application</span></span> | <span data-ttu-id="e46ce-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e46ce-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e46ce-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e46ce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e46ce-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e46ce-117">Optional query parameters</span></span>

<span data-ttu-id="e46ce-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e46ce-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e46ce-119">По умолчанию возвращается только ограниченный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** и **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="e46ce-119">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> 

<span data-ttu-id="e46ce-120">Чтобы получить альтернативный набор свойств, укажите нужный набор свойств объекта [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="e46ce-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="e46ce-121">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, добавьте к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="e46ce-121">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

<span data-ttu-id="e46ce-p103">Некоторые свойства невозможно возвращать в коллекции пользователей. Следующие свойства поддерживаются только при [получении одного пользователя](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="e46ce-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings**</span></span>

## <a name="request-headers"></a><span data-ttu-id="e46ce-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e46ce-124">Request headers</span></span>

| <span data-ttu-id="e46ce-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e46ce-125">Header</span></span>        | <span data-ttu-id="e46ce-126">Значение</span><span class="sxs-lookup"><span data-stu-id="e46ce-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="e46ce-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e46ce-127">Authorization</span></span> | <span data-ttu-id="e46ce-128">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="e46ce-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="e46ce-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e46ce-129">Content-Type</span></span>  | <span data-ttu-id="e46ce-130">application/json</span><span class="sxs-lookup"><span data-stu-id="e46ce-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="e46ce-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e46ce-131">Request body</span></span>

<span data-ttu-id="e46ce-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e46ce-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e46ce-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e46ce-133">Response</span></span>

<span data-ttu-id="e46ce-134">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e46ce-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="e46ce-135">Если возвращается крупная коллекция пользователей, можно использовать [разбиение по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="e46ce-135">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="e46ce-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="e46ce-136">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="e46ce-137">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="e46ce-137">Example 1: Standard users request</span></span>

<span data-ttu-id="e46ce-138">По умолчанию возвращается только стандартный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="e46ce-138">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> <span data-ttu-id="e46ce-139">В этом примере показаны запрос и ответ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e46ce-139">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="e46ce-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e46ce-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e46ce-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e46ce-141">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e46ce-142">C#</span><span class="sxs-lookup"><span data-stu-id="e46ce-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e46ce-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e46ce-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e46ce-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e46ce-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e46ce-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="e46ce-145">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="e46ce-146">Пример 2. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="e46ce-146">Example 2: Users request using $select</span></span>

<span data-ttu-id="e46ce-147">Если вам нужен другой набор свойств, можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="e46ce-147">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="e46ce-148">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="e46ce-148">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="e46ce-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e46ce-149">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e46ce-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="e46ce-150">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e46ce-151">C#</span><span class="sxs-lookup"><span data-stu-id="e46ce-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-properties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e46ce-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e46ce-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-properties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e46ce-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e46ce-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-properties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e46ce-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="e46ce-154">Response</span></span>

<span data-ttu-id="e46ce-155">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e46ce-155">Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
