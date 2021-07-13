---
title: Перечисление пользователей
description: Получение списка объектов user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b9a598d994288859f1f8e2989c90cda7bab3300b
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401381"
---
# <a name="list-users"></a><span data-ttu-id="b4971-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="b4971-103">List users</span></span>

<span data-ttu-id="b4971-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4971-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b4971-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="b4971-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4971-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4971-106">Permissions</span></span>

<span data-ttu-id="b4971-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4971-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4971-109">Permission type</span></span>      | <span data-ttu-id="b4971-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4971-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4971-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4971-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b4971-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4971-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4971-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4971-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4971-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4971-114">Not supported.</span></span>    |
|<span data-ttu-id="b4971-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4971-115">Application</span></span> | <span data-ttu-id="b4971-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4971-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4971-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4971-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4971-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b4971-118">Optional query parameters</span></span>

<span data-ttu-id="b4971-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b4971-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="b4971-120">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="b4971-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="b4971-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="b4971-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="b4971-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="b4971-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="b4971-123">В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="b4971-123">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="b4971-124">По умолчанию возвращается только ограниченный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** и **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="b4971-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> <span data-ttu-id="b4971-125">Чтобы получить альтернативный набор свойств, укажите нужный набор свойств объекта [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="b4971-125">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="b4971-126">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, добавьте к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="b4971-126">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="b4971-p104">Примечание. Некоторые свойства не могут быть возвращены в пользовательском наборе. Следующие свойства поддерживаются только при [извлечении одного пользователя](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="b4971-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving a single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

<span data-ttu-id="b4971-129">Следующие свойства не поддерживаются в личных учетных записях Майкрософт и будут `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span><span class="sxs-lookup"><span data-stu-id="b4971-129">The following properties are not supported in personal Microsoft accounts and will be `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4971-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4971-130">Request headers</span></span>

| <span data-ttu-id="b4971-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4971-131">Header</span></span>        | <span data-ttu-id="b4971-132">Значение</span><span class="sxs-lookup"><span data-stu-id="b4971-132">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="b4971-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4971-133">Authorization</span></span> | <span data-ttu-id="b4971-134">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="b4971-134">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="b4971-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="b4971-135">ConsistencyLevel</span></span> | <span data-ttu-id="b4971-136">необязательный.</span><span class="sxs-lookup"><span data-stu-id="b4971-136">eventual.</span></span> <span data-ttu-id="b4971-137">Этот заголовок и `$count` требуются при использовании `$search`, применении `$filter` с параметром запроса `$orderby` или применении `$filter` с логическим оператором `endsWith`.</span><span class="sxs-lookup"><span data-stu-id="b4971-137">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter, or `$filter` with the `endsWith` logical operator.</span></span> <span data-ttu-id="b4971-138">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="b4971-138">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4971-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4971-139">Request body</span></span>

<span data-ttu-id="b4971-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4971-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4971-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4971-141">Response</span></span>

<span data-ttu-id="b4971-142">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b4971-142">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="b4971-143">Если возвращается крупная коллекция пользователей, можно использовать [разбиение по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="b4971-143">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="b4971-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="b4971-144">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="b4971-145">Пример 1. Получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="b4971-145">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="b4971-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4971-146">Request</span></span>

<span data-ttu-id="b4971-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4971-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b4971-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4971-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_2"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="b4971-149">C#</span><span class="sxs-lookup"><span data-stu-id="b4971-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4971-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4971-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4971-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4971-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4971-152">Java</span><span class="sxs-lookup"><span data-stu-id="b4971-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b4971-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4971-153">Response</span></span>

<span data-ttu-id="b4971-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4971-154">The following is an example of the response.</span></span>

><span data-ttu-id="b4971-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b4971-155">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="b4971-156">Пример 2. Получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="b4971-156">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="b4971-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4971-157">Request</span></span>

<span data-ttu-id="b4971-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4971-158">The following is an example of the request.</span></span>

><span data-ttu-id="b4971-159">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="b4971-159">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="b4971-160">Значение **issuerAssignedId** должно быть адресом электронной почты учетной записи пользователя, а не именем субъекта-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="b4971-160">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="b4971-161">Если используется UPN, результатом будет пустой список.</span><span class="sxs-lookup"><span data-stu-id="b4971-161">If a UPN is used, the response will be an empty list.</span></span>


# <a name="http"></a>[<span data-ttu-id="b4971-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4971-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="b4971-163">C#</span><span class="sxs-lookup"><span data-stu-id="b4971-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4971-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4971-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4971-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4971-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4971-166">Java</span><span class="sxs-lookup"><span data-stu-id="b4971-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b4971-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4971-167">Response</span></span>

<span data-ttu-id="b4971-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4971-168">The following is an example of the response.</span></span> 

> <span data-ttu-id="b4971-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b4971-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-3-get-only-a-count-of-users"></a><span data-ttu-id="b4971-170">Пример 3. Получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="b4971-170">Example 3: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="b4971-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4971-171">Request</span></span>

<span data-ttu-id="b4971-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4971-172">The following is an example of the request.</span></span> <span data-ttu-id="b4971-173">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$count`.</span><span class="sxs-lookup"><span data-stu-id="b4971-173">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="b4971-174">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="b4971-174">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b4971-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4971-175">Response</span></span>

<span data-ttu-id="b4971-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4971-176">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-4-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="b4971-177">Пример 4. Использование параметров $filter и $top для получения одного пользователя с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="b4971-177">Example 4: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b4971-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4971-178">Request</span></span>

<span data-ttu-id="b4971-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4971-179">The following is an example of the request.</span></span> <span data-ttu-id="b4971-180">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual` и строка запроса `$count=true`, так как запрос содержит параметры запроса `$orderBy` и `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b4971-180">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="b4971-181">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="b4971-181">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b4971-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4971-182">Response</span></span>

<span data-ttu-id="b4971-183">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4971-183">The following is an example of the response.</span></span>

><span data-ttu-id="b4971-184">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b4971-184">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="b4971-185">Пример 5. Использование параметра $filter для предоставления всем пользователям почты, которая заканчивается на "a@contoso.com", и в том числе количество возвращаемых объектов с результатами, отсортированными по userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b4971-185">Example 5: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="b4971-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4971-186">Request</span></span>

<span data-ttu-id="b4971-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4971-187">The following is an example of the request.</span></span> <span data-ttu-id="b4971-188">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual` и строка запроса `$count=true`, так как запрос содержит параметры запроса `$orderBy` и `$filter`, а также использует оператор `endsWith`.</span><span class="sxs-lookup"><span data-stu-id="b4971-188">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters, and also uses the `endsWith` operator.</span></span> <span data-ttu-id="b4971-189">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="b4971-189">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>


# <a name="http"></a>[<span data-ttu-id="b4971-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4971-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="b4971-191">C#</span><span class="sxs-lookup"><span data-stu-id="b4971-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4971-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4971-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4971-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4971-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4971-194">Java</span><span class="sxs-lookup"><span data-stu-id="b4971-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b4971-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4971-195">Response</span></span>

<span data-ttu-id="b4971-196">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4971-196">The following is an example of the response.</span></span>

><span data-ttu-id="b4971-197">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b4971-197">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-6-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="b4971-198">Пример 6. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="b4971-198">Example 6: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b4971-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4971-199">Request</span></span>

<span data-ttu-id="b4971-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4971-200">The following is an example of the request.</span></span> <span data-ttu-id="b4971-201">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$search`.</span><span class="sxs-lookup"><span data-stu-id="b4971-201">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="b4971-202">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="b4971-202">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b4971-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4971-203">Response</span></span>

<span data-ttu-id="b4971-204">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4971-204">The following is an example of the response.</span></span>

><span data-ttu-id="b4971-205">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b4971-205">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-7-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="b4971-206">Пример 7. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="b4971-206">Example 7: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b4971-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4971-207">Request</span></span>

<span data-ttu-id="b4971-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4971-208">The following is an example of the request.</span></span> <span data-ttu-id="b4971-209">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$search`.</span><span class="sxs-lookup"><span data-stu-id="b4971-209">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="b4971-210">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="b4971-210">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b4971-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4971-211">Response</span></span>

<span data-ttu-id="b4971-212">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4971-212">The following is an example of the response.</span></span>

> <span data-ttu-id="b4971-213">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b4971-213">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-8-use-filter-to-get-users-who-are-assigned-a-specific-license"></a><span data-ttu-id="b4971-214">Пример 8. Использование $filter для получения пользователей, которым назначена определенная лицензия</span><span class="sxs-lookup"><span data-stu-id="b4971-214">Example 8: Use $filter to get users who are assigned a specific license</span></span>

#### <a name="request"></a><span data-ttu-id="b4971-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4971-215">Request</span></span>

<span data-ttu-id="b4971-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4971-216">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_assignedLicenses"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=id,mail,assignedLicenses&$filter=assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)
```

#### <a name="response"></a><span data-ttu-id="b4971-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4971-217">Response</span></span>

<span data-ttu-id="b4971-218">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4971-218">The following is an example of the response.</span></span>

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
