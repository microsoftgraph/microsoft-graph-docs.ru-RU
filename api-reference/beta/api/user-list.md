---
title: Перечисление пользователей
description: Получение списка объектов user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: bd56e0b6849626bc31a5397ce47fae8a1279aed2
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352398"
---
# <a name="list-users"></a><span data-ttu-id="adbeb-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="adbeb-103">List users</span></span>

<span data-ttu-id="adbeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adbeb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adbeb-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="adbeb-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="adbeb-p101">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств. Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties). Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите свойства в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="adbeb-p101">This operation returns by default only a subset of the more commonly used properties for each user. These _default_ properties are noted in the [Properties](../resources/user.md#properties) section. To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="adbeb-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="adbeb-109">Permissions</span></span>

<span data-ttu-id="adbeb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adbeb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adbeb-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adbeb-112">Permission type</span></span>      | <span data-ttu-id="adbeb-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="adbeb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adbeb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adbeb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="adbeb-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="adbeb-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="adbeb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adbeb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adbeb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adbeb-117">Not supported.</span></span>    |
|<span data-ttu-id="adbeb-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adbeb-118">Application</span></span> | <span data-ttu-id="adbeb-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adbeb-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="adbeb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adbeb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="adbeb-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="adbeb-121">Optional query parameters</span></span>

<span data-ttu-id="adbeb-p103">Этот метод поддерживает [параметры запроса OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`. Вы можете использовать параметр `$search` в свойстве **displayName**. При добавлении или обновлении элементов для этого ресурса они индексируются для использования с параметрами запроса `$count` и `$search`. Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка. В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="adbeb-p103">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index. The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

## <a name="request-headers"></a><span data-ttu-id="adbeb-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="adbeb-127">Request headers</span></span>

| <span data-ttu-id="adbeb-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="adbeb-128">Header</span></span> | <span data-ttu-id="adbeb-129">Значение</span><span class="sxs-lookup"><span data-stu-id="adbeb-129">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="adbeb-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="adbeb-130">Authorization</span></span> | <span data-ttu-id="adbeb-131">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="adbeb-131">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="adbeb-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="adbeb-132">ConsistencyLevel</span></span> | <span data-ttu-id="adbeb-p104">необязательный. Этот заголовок и `$count` требуются при использовании `$search` или применении `$filter` с параметром запроса `$orderby`. В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="adbeb-p104">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adbeb-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="adbeb-136">Request body</span></span>

<span data-ttu-id="adbeb-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="adbeb-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adbeb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbeb-138">Response</span></span>

<span data-ttu-id="adbeb-139">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="adbeb-139">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="adbeb-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="adbeb-140">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="adbeb-141">Пример 1. Получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="adbeb-141">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="adbeb-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbeb-142">Request</span></span>

<span data-ttu-id="adbeb-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbeb-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="adbeb-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="adbeb-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="adbeb-145">C#</span><span class="sxs-lookup"><span data-stu-id="adbeb-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adbeb-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adbeb-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adbeb-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adbeb-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adbeb-148">Java</span><span class="sxs-lookup"><span data-stu-id="adbeb-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="adbeb-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbeb-149">Response</span></span>

<span data-ttu-id="adbeb-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adbeb-150">The following is an example of the response.</span></span> 
><span data-ttu-id="adbeb-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adbeb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value":[
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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="adbeb-153">Пример 2. Получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="adbeb-153">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="adbeb-154">Найдите учетную запись пользователя, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="adbeb-154">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="adbeb-155">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="adbeb-155">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="adbeb-156">Значение **issuerAssignedId** должно быть адресом электронной почты учетной записи пользователя, а не именем субъекта-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="adbeb-156">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="adbeb-157">Если используется UPN, результатом будет пустой список.</span><span class="sxs-lookup"><span data-stu-id="adbeb-157">If a UPN is used, the response will be an empty list.</span></span>

#### <a name="request"></a><span data-ttu-id="adbeb-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbeb-158">Request</span></span>

<span data-ttu-id="adbeb-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbeb-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="adbeb-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="adbeb-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="adbeb-161">C#</span><span class="sxs-lookup"><span data-stu-id="adbeb-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adbeb-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adbeb-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adbeb-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adbeb-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adbeb-164">Java</span><span class="sxs-lookup"><span data-stu-id="adbeb-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="adbeb-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbeb-165">Response</span></span>

<span data-ttu-id="adbeb-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adbeb-166">The following is an example of the response.</span></span> 
> <span data-ttu-id="adbeb-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adbeb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="adbeb-169">Пример 3. Получение пользователей с указанием времени их последнего входа в систему</span><span class="sxs-lookup"><span data-stu-id="adbeb-169">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="adbeb-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbeb-170">Request</span></span>

<span data-ttu-id="adbeb-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbeb-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="adbeb-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="adbeb-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="adbeb-173">C#</span><span class="sxs-lookup"><span data-stu-id="adbeb-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adbeb-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adbeb-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adbeb-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adbeb-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adbeb-176">Java</span><span class="sxs-lookup"><span data-stu-id="adbeb-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="adbeb-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbeb-177">Response</span></span>

<span data-ttu-id="adbeb-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adbeb-178">The following is an example of the response.</span></span> 
> <span data-ttu-id="adbeb-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adbeb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(displayName,userPrincipalName,signInActivity)",
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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="adbeb-181">Пример 4. Список времени последнего входа пользователей с определенным отображаемым именем</span><span class="sxs-lookup"><span data-stu-id="adbeb-181">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="adbeb-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbeb-182">Request</span></span>

<span data-ttu-id="adbeb-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbeb-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="adbeb-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="adbeb-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="adbeb-185">C#</span><span class="sxs-lookup"><span data-stu-id="adbeb-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adbeb-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adbeb-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adbeb-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adbeb-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adbeb-188">Java</span><span class="sxs-lookup"><span data-stu-id="adbeb-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="adbeb-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbeb-189">Response</span></span>

<span data-ttu-id="adbeb-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adbeb-190">The following is an example of the response.</span></span> 
> <span data-ttu-id="adbeb-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adbeb-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="adbeb-193">Пример 5: перечисление времени последнего входа пользователей в определенный временной диапазон</span><span class="sxs-lookup"><span data-stu-id="adbeb-193">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="adbeb-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbeb-194">Request</span></span>

<span data-ttu-id="adbeb-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbeb-195">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="adbeb-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="adbeb-196">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="adbeb-197">C#</span><span class="sxs-lookup"><span data-stu-id="adbeb-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adbeb-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adbeb-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adbeb-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adbeb-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adbeb-200">Java</span><span class="sxs-lookup"><span data-stu-id="adbeb-200">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="adbeb-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbeb-201">Response</span></span>

<span data-ttu-id="adbeb-202">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adbeb-202">The following is an example of the response.</span></span> 
> <span data-ttu-id="adbeb-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adbeb-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="adbeb-205">Пример 6. Получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="adbeb-205">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="adbeb-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbeb-206">Request</span></span>

<span data-ttu-id="adbeb-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbeb-207">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="adbeb-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbeb-208">Response</span></span>

<span data-ttu-id="adbeb-209">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adbeb-209">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="adbeb-210">893</span><span class="sxs-lookup"><span data-stu-id="adbeb-210">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="adbeb-211">Пример 7. Использование параметров $filter и $top для получения одного пользователя с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="adbeb-211">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="adbeb-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbeb-212">Request</span></span>

<span data-ttu-id="adbeb-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbeb-213">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="adbeb-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbeb-214">Response</span></span>

<span data-ttu-id="adbeb-215">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adbeb-215">The following is an example of the response.</span></span>
><span data-ttu-id="adbeb-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adbeb-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="adbeb-218">Пример 8. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="adbeb-218">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="adbeb-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbeb-219">Request</span></span>

<span data-ttu-id="adbeb-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbeb-220">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="adbeb-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbeb-221">Response</span></span>

<span data-ttu-id="adbeb-222">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adbeb-222">The following is an example of the response.</span></span>
><span data-ttu-id="adbeb-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adbeb-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="adbeb-225">Пример 9. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="adbeb-225">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="adbeb-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbeb-226">Request</span></span>

<span data-ttu-id="adbeb-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbeb-227">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="adbeb-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbeb-228">Response</span></span>

<span data-ttu-id="adbeb-229">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adbeb-229">The following is an example of the response.</span></span> 
> <span data-ttu-id="adbeb-p113">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adbeb-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
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
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
