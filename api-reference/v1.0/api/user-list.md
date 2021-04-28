---
title: Перечисление пользователей
description: Получение списка объектов user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 79c60a53edf8d5c105d0a12a4ce53514e6dc8cb2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52033659"
---
# <a name="list-users"></a><span data-ttu-id="b3074-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="b3074-103">List users</span></span>

<span data-ttu-id="b3074-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3074-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3074-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="b3074-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3074-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3074-106">Permissions</span></span>

<span data-ttu-id="b3074-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3074-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3074-109">Permission type</span></span>      | <span data-ttu-id="b3074-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3074-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3074-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3074-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3074-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3074-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3074-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3074-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3074-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3074-114">Not supported.</span></span>    |
|<span data-ttu-id="b3074-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3074-115">Application</span></span> | <span data-ttu-id="b3074-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3074-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3074-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3074-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3074-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b3074-118">Optional query parameters</span></span>

<span data-ttu-id="b3074-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b3074-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="b3074-120">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="b3074-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="b3074-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="b3074-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="b3074-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="b3074-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="b3074-123">В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="b3074-123">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="b3074-124">По умолчанию возвращается только ограниченный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** и **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="b3074-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="b3074-125">Чтобы получить альтернативный набор свойств, укажите нужный набор свойств объекта [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="b3074-125">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="b3074-126">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, добавьте к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="b3074-126">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="b3074-p104">Некоторые свойства невозможно возвращать в коллекции пользователей. Следующие свойства поддерживаются только при [получении одного пользователя](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="b3074-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3074-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3074-129">Request headers</span></span>

| <span data-ttu-id="b3074-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3074-130">Header</span></span>        | <span data-ttu-id="b3074-131">Значение</span><span class="sxs-lookup"><span data-stu-id="b3074-131">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="b3074-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3074-132">Authorization</span></span> | <span data-ttu-id="b3074-133">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="b3074-133">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="b3074-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="b3074-134">ConsistencyLevel</span></span> | <span data-ttu-id="b3074-135">необязательный.</span><span class="sxs-lookup"><span data-stu-id="b3074-135">eventual.</span></span> <span data-ttu-id="b3074-136">Этот заголовок и `$count` требуются при использовании `$search`, применении `$filter` с параметром запроса `$orderby` или применении `$filter` с логическим оператором `endsWith`.</span><span class="sxs-lookup"><span data-stu-id="b3074-136">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter, or `$filter` with the `endsWith` logical operator.</span></span> <span data-ttu-id="b3074-137">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="b3074-137">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3074-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3074-138">Request body</span></span>

<span data-ttu-id="b3074-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3074-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3074-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3074-140">Response</span></span>

<span data-ttu-id="b3074-141">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b3074-141">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="b3074-142">Если возвращается крупная коллекция пользователей, можно использовать [разбиение по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="b3074-142">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="b3074-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3074-143">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="b3074-144">Пример 1. Получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="b3074-144">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="b3074-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3074-145">Request</span></span>

<span data-ttu-id="b3074-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3074-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b3074-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3074-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_2"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="b3074-148">C#</span><span class="sxs-lookup"><span data-stu-id="b3074-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3074-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3074-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3074-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3074-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3074-151">Java</span><span class="sxs-lookup"><span data-stu-id="b3074-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b3074-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3074-152">Response</span></span>

<span data-ttu-id="b3074-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b3074-153">The following is an example of the response.</span></span>

><span data-ttu-id="b3074-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3074-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "value": [
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "otherMails":["contoso1@gmail.com"],
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="b3074-155">Пример 2. Получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="b3074-155">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="b3074-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3074-156">Request</span></span>

<span data-ttu-id="b3074-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3074-157">The following is an example of the request.</span></span>

><span data-ttu-id="b3074-158">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="b3074-158">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="b3074-159">Значение **issuerAssignedId** должно быть адресом электронной почты учетной записи пользователя, а не именем субъекта-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="b3074-159">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="b3074-160">Если используется UPN, результатом будет пустой список.</span><span class="sxs-lookup"><span data-stu-id="b3074-160">If a UPN is used, the response will be an empty list.</span></span>


# <a name="http"></a>[<span data-ttu-id="b3074-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3074-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="b3074-162">C#</span><span class="sxs-lookup"><span data-stu-id="b3074-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3074-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3074-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3074-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3074-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3074-165">Java</span><span class="sxs-lookup"><span data-stu-id="b3074-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b3074-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3074-166">Response</span></span>

<span data-ttu-id="b3074-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b3074-167">The following is an example of the response.</span></span> 

> <span data-ttu-id="b3074-168">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3074-168">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "value": [
    {
      "displayName": "John Smith"
    }
  ]
}
```
### <a name="example-3-get-only-a-count-of-users"></a><span data-ttu-id="b3074-169">Пример 3. Получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="b3074-169">Example 3: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="b3074-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3074-170">Request</span></span>

<span data-ttu-id="b3074-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3074-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b3074-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3074-172">Response</span></span>

<span data-ttu-id="b3074-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b3074-173">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-4-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="b3074-174">Пример 4. Использование параметров $filter и $top для получения одного пользователя с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="b3074-174">Example 4: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b3074-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3074-175">Request</span></span>

<span data-ttu-id="b3074-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3074-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b3074-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3074-177">Response</span></span>

<span data-ttu-id="b3074-178">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b3074-178">The following is an example of the response.</span></span>

><span data-ttu-id="b3074-179">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3074-179">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mail":"a@contoso.com",
      "mailNickname":"a_contoso.com#EXT#",
      "otherMails":["a@contoso.com"],
      "proxyAddresses":["SMTP:a@contoso.com"],
      "userPrincipalName":"a_contoso.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-5-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="b3074-180">Пример 5. Использование параметра $filter для предоставления всем пользователям почты, которая заканчивается на "a@contoso.com", и в том числе количество возвращаемых объектов с результатами, отсортированными по userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b3074-180">Example 5: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="b3074-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3074-181">Request</span></span>

<span data-ttu-id="b3074-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3074-182">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b3074-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3074-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="b3074-184">C#</span><span class="sxs-lookup"><span data-stu-id="b3074-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3074-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3074-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3074-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3074-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3074-187">Java</span><span class="sxs-lookup"><span data-stu-id="b3074-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b3074-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3074-188">Response</span></span>

<span data-ttu-id="b3074-189">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b3074-189">The following is an example of the response.</span></span>

><span data-ttu-id="b3074-190">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3074-190">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count": 1,
  "value": [
    {
      "displayName": "Grady Archie",
      "givenName": "Grady",
      "jobTitle": "Designer",
      "mail": "GradyA@contoso.com",
      "userPrincipalName": "GradyA@contoso.com",
      "id": "e8b753b5-4117-464e-9a08-713e1ff266b3"
      }
    ]
}
```

### <a name="example-6-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="b3074-191">Пример 6. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="b3074-191">Example 6: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b3074-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3074-192">Request</span></span>

<span data-ttu-id="b3074-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3074-193">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b3074-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3074-194">Response</span></span>

<span data-ttu-id="b3074-195">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b3074-195">The following is an example of the response.</span></span>

><span data-ttu-id="b3074-196">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3074-196">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    }
  ]
}
```

### <a name="example-7-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="b3074-197">Пример 7. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="b3074-197">Example 7: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b3074-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3074-198">Request</span></span>

<span data-ttu-id="b3074-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3074-199">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b3074-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3074-200">Response</span></span>

<span data-ttu-id="b3074-201">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b3074-201">The following is an example of the response.</span></span>

> <span data-ttu-id="b3074-202">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3074-202">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    },
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-8-use-filter-to-get-users-who-are-assigned-a-specific-license"></a><span data-ttu-id="b3074-203">Пример 8. Использование $filter для получения пользователей, которым назначена определенная лицензия</span><span class="sxs-lookup"><span data-stu-id="b3074-203">Example 8: Use $filter to get users who are assigned a specific license</span></span>

#### <a name="request"></a><span data-ttu-id="b3074-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3074-204">Request</span></span>

<span data-ttu-id="b3074-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3074-205">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_assignedLicenses"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=id,mail,assignedLicenses&$filter=assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)
```

#### <a name="response"></a><span data-ttu-id="b3074-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3074-206">Response</span></span>

<span data-ttu-id="b3074-207">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b3074-207">The following is an example of the response.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(id,mail,assignedLicenses)",
  "value": [
    {
      "id": "cb4954e8-467f-4a6d-a8c8-28b9034fadbc",
      "mail": "admin@contoso.com",
      "assignedLicenses": [
        {
          "disabledPlans": [],
          "skuId": "cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46"
        }
      ]
    },
    {
      "id": "81a133c2-bdf2-4e67-8755-7264366b04ee",
      "mail": "DebraB@contoso.com",
      "assignedLicenses": [
        {
          "disabledPlans": [],
          "skuId": "cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46"
        }
      ]
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
