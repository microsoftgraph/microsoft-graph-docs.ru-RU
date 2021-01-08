---
title: Перечисление пользователей
description: Получение списка объектов user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ca4d6b4511d5271f0defbcfb29da61a334b790da
ms.sourcegitcommit: df0778a4dbd1e7a2fde1846bdfbfd9440fc91672
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768254"
---
# <a name="list-users"></a><span data-ttu-id="7477b-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="7477b-103">List users</span></span>

<span data-ttu-id="7477b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7477b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7477b-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="7477b-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7477b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7477b-106">Permissions</span></span>

<span data-ttu-id="7477b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7477b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7477b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7477b-109">Permission type</span></span>      | <span data-ttu-id="7477b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7477b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7477b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7477b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7477b-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7477b-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7477b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7477b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7477b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7477b-114">Not supported.</span></span>    |
|<span data-ttu-id="7477b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7477b-115">Application</span></span> | <span data-ttu-id="7477b-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7477b-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7477b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7477b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7477b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7477b-118">Optional query parameters</span></span>

<span data-ttu-id="7477b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7477b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="7477b-120">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="7477b-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="7477b-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="7477b-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="7477b-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="7477b-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="7477b-123">В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="7477b-123">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="7477b-124">По умолчанию возвращается только ограниченный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** и **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="7477b-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="7477b-125">Чтобы получить альтернативный набор свойств, укажите нужный набор свойств объекта [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="7477b-125">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="7477b-126">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, добавьте к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="7477b-126">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="7477b-p104">Некоторые свойства невозможно возвращать в коллекции пользователей. Следующие свойства поддерживаются только при [получении одного пользователя](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="7477b-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7477b-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7477b-129">Request headers</span></span>

| <span data-ttu-id="7477b-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7477b-130">Header</span></span>        | <span data-ttu-id="7477b-131">Значение</span><span class="sxs-lookup"><span data-stu-id="7477b-131">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="7477b-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7477b-132">Authorization</span></span> | <span data-ttu-id="7477b-133">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="7477b-133">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="7477b-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="7477b-134">ConsistencyLevel</span></span> | <span data-ttu-id="7477b-135">необязательный.</span><span class="sxs-lookup"><span data-stu-id="7477b-135">eventual.</span></span> <span data-ttu-id="7477b-136">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="7477b-136">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="7477b-137">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="7477b-137">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7477b-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7477b-138">Request body</span></span>

<span data-ttu-id="7477b-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7477b-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7477b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7477b-140">Response</span></span>

<span data-ttu-id="7477b-141">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7477b-141">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="7477b-142">Если возвращается крупная коллекция пользователей, можно использовать [разбиение по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="7477b-142">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="7477b-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="7477b-143">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="7477b-144">Пример 1. Получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="7477b-144">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="7477b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="7477b-145">Request</span></span>

<span data-ttu-id="7477b-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7477b-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7477b-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="7477b-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="7477b-148">C#</span><span class="sxs-lookup"><span data-stu-id="7477b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7477b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7477b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7477b-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7477b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7477b-151">Java</span><span class="sxs-lookup"><span data-stu-id="7477b-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7477b-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7477b-152">Response</span></span>

<span data-ttu-id="7477b-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7477b-153">The following is an example of the response.</span></span>

><span data-ttu-id="7477b-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7477b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="7477b-156">Пример 2. Получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="7477b-156">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="7477b-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="7477b-157">Request</span></span>

<span data-ttu-id="7477b-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7477b-158">The following is an example of the request.</span></span>

><span data-ttu-id="7477b-159">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="7477b-159">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="7477b-160">Значение **issuerAssignedId** должно быть адресом электронной почты учетной записи пользователя, а не именем субъекта-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="7477b-160">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="7477b-161">Если используется UPN, результатом будет пустой список.</span><span class="sxs-lookup"><span data-stu-id="7477b-161">If a UPN is used, the response will be an empty list.</span></span>


# <a name="http"></a>[<span data-ttu-id="7477b-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="7477b-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="7477b-163">C#</span><span class="sxs-lookup"><span data-stu-id="7477b-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7477b-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7477b-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7477b-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7477b-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7477b-166">Java</span><span class="sxs-lookup"><span data-stu-id="7477b-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7477b-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="7477b-167">Response</span></span>

<span data-ttu-id="7477b-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7477b-168">The following is an example of the response.</span></span> 

> <span data-ttu-id="7477b-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7477b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-3-get-only-a-count-of-users"></a><span data-ttu-id="7477b-171">Пример 3. Получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="7477b-171">Example 3: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="7477b-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="7477b-172">Request</span></span>

<span data-ttu-id="7477b-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7477b-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7477b-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="7477b-174">Response</span></span>

<span data-ttu-id="7477b-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7477b-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-4-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="7477b-176">Пример 4. Использование параметров $filter и $top для получения одного пользователя с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="7477b-176">Example 4: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7477b-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="7477b-177">Request</span></span>

<span data-ttu-id="7477b-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7477b-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7477b-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="7477b-179">Response</span></span>

<span data-ttu-id="7477b-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7477b-180">The following is an example of the response.</span></span>

><span data-ttu-id="7477b-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7477b-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="7477b-183">Пример 5. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="7477b-183">Example 5: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7477b-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="7477b-184">Request</span></span>

<span data-ttu-id="7477b-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7477b-185">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7477b-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="7477b-186">Response</span></span>

<span data-ttu-id="7477b-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7477b-187">The following is an example of the response.</span></span>

><span data-ttu-id="7477b-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7477b-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="7477b-190">Пример 6. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="7477b-190">Example 6: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7477b-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="7477b-191">Request</span></span>

<span data-ttu-id="7477b-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7477b-192">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7477b-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="7477b-193">Response</span></span>

<span data-ttu-id="7477b-194">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7477b-194">The following is an example of the response.</span></span>

> <span data-ttu-id="7477b-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7477b-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
