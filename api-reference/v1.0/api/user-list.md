---
title: Перечисление пользователей
description: Получение списка объектов user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d20e60757fce6b2981ce4db1d06ffe29930e3539
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634881"
---
# <a name="list-users"></a><span data-ttu-id="a3da4-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="a3da4-103">List users</span></span>

<span data-ttu-id="a3da4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3da4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a3da4-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="a3da4-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3da4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3da4-106">Permissions</span></span>

<span data-ttu-id="a3da4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3da4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3da4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3da4-109">Permission type</span></span>      | <span data-ttu-id="a3da4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3da4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3da4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3da4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a3da4-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3da4-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3da4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3da4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3da4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3da4-114">Not supported.</span></span>    |
|<span data-ttu-id="a3da4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3da4-115">Application</span></span> | <span data-ttu-id="a3da4-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3da4-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3da4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3da4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3da4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a3da4-118">Optional query parameters</span></span>

<span data-ttu-id="a3da4-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a3da4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="a3da4-120">По умолчанию возвращается только ограниченный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** и **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="a3da4-120">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="a3da4-121">Чтобы получить альтернативный набор свойств, укажите нужный набор свойств объекта [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="a3da4-121">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="a3da4-122">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, добавьте к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="a3da4-122">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="a3da4-p103">Некоторые свойства невозможно возвращать в коллекции пользователей. Следующие свойства поддерживаются только при [получении одного пользователя](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="a3da4-p103">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3da4-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3da4-125">Request headers</span></span>

| <span data-ttu-id="a3da4-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3da4-126">Header</span></span>        | <span data-ttu-id="a3da4-127">Значение</span><span class="sxs-lookup"><span data-stu-id="a3da4-127">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="a3da4-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3da4-128">Authorization</span></span> | <span data-ttu-id="a3da4-129">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="a3da4-129">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3da4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3da4-130">Request body</span></span>

<span data-ttu-id="a3da4-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3da4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3da4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3da4-132">Response</span></span>

<span data-ttu-id="a3da4-133">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a3da4-133">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="a3da4-134">Если возвращается крупная коллекция пользователей, можно использовать [разбиение по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="a3da4-134">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="a3da4-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="a3da4-135">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="a3da4-136">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="a3da4-136">Example 1: Standard users request</span></span>

<span data-ttu-id="a3da4-137">По умолчанию возвращается только стандартный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="a3da4-137">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, **userPrincipalName**).</span></span> <span data-ttu-id="a3da4-138">В этом примере показаны запрос и ответ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a3da4-138">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="a3da4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3da4-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a3da4-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3da4-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="a3da4-141">C#</span><span class="sxs-lookup"><span data-stu-id="a3da4-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3da4-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3da4-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3da4-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3da4-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3da4-144">Java</span><span class="sxs-lookup"><span data-stu-id="a3da4-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a3da4-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3da4-145">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="a3da4-146">Пример 2. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="a3da4-146">Example 2: Users request using $select</span></span>

<span data-ttu-id="a3da4-147">Если вам нужен другой набор свойств, можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="a3da4-147">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="a3da4-148">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="a3da4-148">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

##### <a name="request"></a><span data-ttu-id="a3da4-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3da4-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a3da4-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3da4-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```
# <a name="c"></a>[<span data-ttu-id="a3da4-151">C#</span><span class="sxs-lookup"><span data-stu-id="a3da4-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-properties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3da4-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3da4-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-properties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3da4-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3da4-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-properties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3da4-154">Java</span><span class="sxs-lookup"><span data-stu-id="a3da4-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-properties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a3da4-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3da4-155">Response</span></span>

<span data-ttu-id="a3da4-156">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a3da4-156">Note: The response object shown here may be truncated for brevity.</span></span>
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

### <a name="example-3-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="a3da4-157">Пример 3. Поиск учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="a3da4-157">Example 3: Find a user account using a sign-in name</span></span>

<span data-ttu-id="a3da4-158">Найдите учетную запись пользователя в клиенте B2C, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="a3da4-158">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="a3da4-159">Этот запрос может использоваться службой поддержки для поиска учетной записи пользователя в клиенте B2C (в данном примере клиентом B2C является contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="a3da4-159">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="a3da4-160">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="a3da4-160">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="a3da4-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3da4-161">Request</span></span>

<span data-ttu-id="a3da4-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3da4-162">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a3da4-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3da4-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="a3da4-164">C#</span><span class="sxs-lookup"><span data-stu-id="a3da4-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3da4-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3da4-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3da4-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3da4-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3da4-167">Java</span><span class="sxs-lookup"><span data-stu-id="a3da4-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="a3da4-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3da4-168">Response</span></span>

<span data-ttu-id="a3da4-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a3da4-169">The following is an example of the response.</span></span> 
> <span data-ttu-id="a3da4-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3da4-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
