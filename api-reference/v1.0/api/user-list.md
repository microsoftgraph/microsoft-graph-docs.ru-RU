---
title: Перечисление пользователей
description: Получение списка объектов user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ca14af75340441acf8ba7f3049ce3ac744c678e7
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524416"
---
# <a name="list-users"></a><span data-ttu-id="7dac3-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="7dac3-103">List users</span></span>

<span data-ttu-id="7dac3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dac3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7dac3-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="7dac3-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dac3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7dac3-106">Permissions</span></span>

<span data-ttu-id="7dac3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dac3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dac3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dac3-109">Permission type</span></span>      | <span data-ttu-id="7dac3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dac3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dac3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dac3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7dac3-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7dac3-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7dac3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dac3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dac3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dac3-114">Not supported.</span></span>    |
|<span data-ttu-id="7dac3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dac3-115">Application</span></span> | <span data-ttu-id="7dac3-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dac3-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dac3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dac3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7dac3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7dac3-118">Optional query parameters</span></span>

<span data-ttu-id="7dac3-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7dac3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="7dac3-120">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="7dac3-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="7dac3-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="7dac3-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="7dac3-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="7dac3-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="7dac3-123">В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="7dac3-123">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="7dac3-124">По умолчанию возвращается только ограниченный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** и **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="7dac3-124">By default, only a limited set of properties are returned (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, and **userPrincipalName**).</span></span> 

<span data-ttu-id="7dac3-125">Чтобы получить альтернативный набор свойств, укажите нужный набор свойств объекта [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="7dac3-125">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="7dac3-126">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, добавьте к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="7dac3-126">For example, to return **displayName**, **givenName**, and **postalCode**, add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="7dac3-p104">Некоторые свойства невозможно возвращать в коллекции пользователей. Следующие свойства поддерживаются только при [получении одного пользователя](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="7dac3-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7dac3-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dac3-129">Request headers</span></span>

| <span data-ttu-id="7dac3-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7dac3-130">Header</span></span>        | <span data-ttu-id="7dac3-131">Значение</span><span class="sxs-lookup"><span data-stu-id="7dac3-131">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="7dac3-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7dac3-132">Authorization</span></span> | <span data-ttu-id="7dac3-133">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="7dac3-133">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="7dac3-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="7dac3-134">ConsistencyLevel</span></span> | <span data-ttu-id="7dac3-135">необязательный.</span><span class="sxs-lookup"><span data-stu-id="7dac3-135">eventual.</span></span> <span data-ttu-id="7dac3-136">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="7dac3-136">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="7dac3-137">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="7dac3-137">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dac3-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7dac3-138">Request body</span></span>

<span data-ttu-id="7dac3-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7dac3-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dac3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dac3-140">Response</span></span>

<span data-ttu-id="7dac3-141">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7dac3-141">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="7dac3-142">Если возвращается крупная коллекция пользователей, можно использовать [разбиение по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="7dac3-142">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="7dac3-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="7dac3-143">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="7dac3-144">Пример 1. Получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="7dac3-144">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="7dac3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dac3-145">Request</span></span>

<span data-ttu-id="7dac3-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dac3-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7dac3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dac3-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```
# <a name="c"></a>[<span data-ttu-id="7dac3-148">C#</span><span class="sxs-lookup"><span data-stu-id="7dac3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dac3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dac3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dac3-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dac3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7dac3-151">Java</span><span class="sxs-lookup"><span data-stu-id="7dac3-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7dac3-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dac3-152">Response</span></span>

<span data-ttu-id="7dac3-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dac3-153">The following is an example of the response.</span></span>

><span data-ttu-id="7dac3-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dac3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="7dac3-156">Пример 2. Получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="7dac3-156">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="7dac3-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dac3-157">Request</span></span>

<span data-ttu-id="7dac3-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dac3-158">The following is an example of the request.</span></span>

><span data-ttu-id="7dac3-159">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="7dac3-159">**Note:** When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="7dac3-160">Значение **issuerAssignedId** должно быть адресом электронной почты учетной записи пользователя, а не именем субъекта-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="7dac3-160">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="7dac3-161">Если используется UPN, результатом будет пустой список.</span><span class="sxs-lookup"><span data-stu-id="7dac3-161">If a UPN is used, the response will be an empty list.</span></span>


# <a name="http"></a>[<span data-ttu-id="7dac3-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dac3-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="7dac3-163">C#</span><span class="sxs-lookup"><span data-stu-id="7dac3-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dac3-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dac3-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dac3-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dac3-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7dac3-166">Java</span><span class="sxs-lookup"><span data-stu-id="7dac3-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7dac3-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dac3-167">Response</span></span>

<span data-ttu-id="7dac3-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dac3-168">The following is an example of the response.</span></span> 

> <span data-ttu-id="7dac3-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dac3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="7dac3-171">Пример 3. Получение пользователей с указанием времени их последнего входа в систему</span><span class="sxs-lookup"><span data-stu-id="7dac3-171">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="7dac3-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dac3-172">Request</span></span>

<span data-ttu-id="7dac3-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dac3-173">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7dac3-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dac3-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="7dac3-175">C#</span><span class="sxs-lookup"><span data-stu-id="7dac3-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dac3-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dac3-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dac3-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dac3-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7dac3-178">Java</span><span class="sxs-lookup"><span data-stu-id="7dac3-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7dac3-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dac3-179">Response</span></span>

<span data-ttu-id="7dac3-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dac3-180">The following is an example of the response.</span></span>

><span data-ttu-id="7dac3-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dac3-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(displayName,userPrincipalName,signInActivity)",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-07-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="7dac3-183">Пример 4. Список времени последнего входа пользователей с определенным отображаемым именем</span><span class="sxs-lookup"><span data-stu-id="7dac3-183">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="7dac3-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dac3-184">Request</span></span>

<span data-ttu-id="7dac3-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dac3-185">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7dac3-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dac3-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="7dac3-187">C#</span><span class="sxs-lookup"><span data-stu-id="7dac3-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dac3-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dac3-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dac3-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dac3-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7dac3-190">Java</span><span class="sxs-lookup"><span data-stu-id="7dac3-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7dac3-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dac3-191">Response</span></span>

<span data-ttu-id="7dac3-192">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dac3-192">The following is an example of the response.</span></span> 

> <span data-ttu-id="7dac3-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dac3-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
  "value": [
    {
      "displayName": "Eric Solomon",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    }
  ]
}
```

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="7dac3-195">Пример 5: перечисление времени последнего входа пользователей в определенный временной диапазон</span><span class="sxs-lookup"><span data-stu-id="7dac3-195">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="7dac3-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dac3-196">Request</span></span>

<span data-ttu-id="7dac3-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dac3-197">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_signin_last_time_range"
} -->
```http
GET https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="7dac3-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dac3-198">Response</span></span>

<span data-ttu-id="7dac3-199">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dac3-199">The following is an example of the response.</span></span> 

> <span data-ttu-id="7dac3-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dac3-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-05-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-04-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="7dac3-202">Пример 6. Получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="7dac3-202">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="7dac3-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dac3-203">Request</span></span>

<span data-ttu-id="7dac3-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dac3-204">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7dac3-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dac3-205">Response</span></span>

<span data-ttu-id="7dac3-206">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7dac3-206">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="7dac3-207">Пример 7. Использование параметров $filter и $top для получения одного пользователя с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="7dac3-207">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7dac3-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dac3-208">Request</span></span>

<span data-ttu-id="7dac3-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dac3-209">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7dac3-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dac3-210">Response</span></span>

<span data-ttu-id="7dac3-211">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dac3-211">The following is an example of the response.</span></span>

><span data-ttu-id="7dac3-p113">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dac3-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="7dac3-214">Пример 8. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="7dac3-214">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7dac3-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dac3-215">Request</span></span>

<span data-ttu-id="7dac3-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dac3-216">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7dac3-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dac3-217">Response</span></span>

<span data-ttu-id="7dac3-218">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dac3-218">The following is an example of the response.</span></span>

><span data-ttu-id="7dac3-p114">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dac3-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="7dac3-221">Пример 9. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="7dac3-221">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7dac3-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dac3-222">Request</span></span>

<span data-ttu-id="7dac3-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dac3-223">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7dac3-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dac3-224">Response</span></span>

<span data-ttu-id="7dac3-225">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dac3-225">The following is an example of the response.</span></span>

> <span data-ttu-id="7dac3-p115">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dac3-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
