---
title: Перечисление пользователей
description: Получение списка объектов user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f9648b505700b05b05a64f977cb94bbd7d92f6e0
ms.sourcegitcommit: bd0daf5c133ab29af9337a5edd3b8509fd2313d5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/17/2020
ms.locfileid: "41232037"
---
# <a name="list-users"></a><span data-ttu-id="73527-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="73527-103">List users</span></span>

<span data-ttu-id="73527-104">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="73527-104">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="73527-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73527-105">Permissions</span></span>

<span data-ttu-id="73527-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73527-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73527-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73527-108">Permission type</span></span>      | <span data-ttu-id="73527-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73527-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73527-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73527-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73527-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73527-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73527-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73527-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73527-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73527-113">Not supported.</span></span>    |
|<span data-ttu-id="73527-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73527-114">Application</span></span> | <span data-ttu-id="73527-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73527-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73527-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73527-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73527-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="73527-117">Optional query parameters</span></span>

<span data-ttu-id="73527-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="73527-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="73527-119">По умолчанию возвращается только ограниченный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** и **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="73527-119">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="73527-120">Чтобы получить альтернативный набор свойств, укажите нужный набор свойств объекта [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="73527-120">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="73527-121">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, добавьте к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="73527-121">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="73527-p103">Некоторые свойства невозможно возвращать в коллекции пользователей. Следующие свойства поддерживаются только при [получении одного пользователя](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="73527-p103">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73527-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73527-124">Request headers</span></span>

| <span data-ttu-id="73527-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73527-125">Header</span></span>        | <span data-ttu-id="73527-126">Значение</span><span class="sxs-lookup"><span data-stu-id="73527-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="73527-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73527-127">Authorization</span></span> | <span data-ttu-id="73527-128">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="73527-128">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73527-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73527-129">Request body</span></span>

<span data-ttu-id="73527-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73527-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73527-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="73527-131">Response</span></span>

<span data-ttu-id="73527-132">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="73527-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="73527-133">Если возвращается крупная коллекция пользователей, можно использовать [разбиение по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="73527-133">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="73527-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="73527-134">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="73527-135">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="73527-135">Example 1: Standard users request</span></span>

<span data-ttu-id="73527-136">По умолчанию возвращается только стандартный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="73527-136">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, **userPrincipalName**).</span></span> <span data-ttu-id="73527-137">В этом примере показаны запрос и ответ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="73527-137">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="73527-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="73527-138">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="73527-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="73527-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73527-140">C#</span><span class="sxs-lookup"><span data-stu-id="73527-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73527-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73527-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73527-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73527-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="73527-143">Java</span><span class="sxs-lookup"><span data-stu-id="73527-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="73527-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="73527-144">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="73527-145">Пример 2. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="73527-145">Example 2: Users request using $select</span></span>

<span data-ttu-id="73527-146">Если вам нужен другой набор свойств, можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="73527-146">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="73527-147">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="73527-147">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

##### <a name="request"></a><span data-ttu-id="73527-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="73527-148">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="73527-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="73527-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73527-150">C#</span><span class="sxs-lookup"><span data-stu-id="73527-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-properties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73527-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73527-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-properties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73527-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73527-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-properties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="73527-153">Java</span><span class="sxs-lookup"><span data-stu-id="73527-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-properties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="73527-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="73527-154">Response</span></span>

<span data-ttu-id="73527-155">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="73527-155">Note: The response object shown here may be truncated for brevity.</span></span>
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

### <a name="example-3-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="73527-156">Пример 3. Поиск учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="73527-156">Example 2: Find a user account using a sign-in name</span></span>

<span data-ttu-id="73527-157">Найдите учетную запись пользователя в клиенте B2C, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="73527-157">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="73527-158">Этот запрос может использоваться службой поддержки для поиска учетной записи пользователя в клиенте B2C (в данном примере клиентом B2C является contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="73527-158">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="73527-159">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="73527-159">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="73527-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="73527-160">Request</span></span>

<span data-ttu-id="73527-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73527-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```

---

#### <a name="response"></a><span data-ttu-id="73527-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="73527-162">Response</span></span>

<span data-ttu-id="73527-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="73527-163">The following is an example of the response.</span></span> 
> <span data-ttu-id="73527-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73527-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
