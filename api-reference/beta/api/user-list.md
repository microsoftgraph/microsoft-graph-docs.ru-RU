---
title: Перечисление пользователей
description: Получение списка объектов user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 46f4187f184c9303466161d575634224d1961eae
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2020
ms.locfileid: "49030265"
---
# <a name="list-users"></a><span data-ttu-id="21872-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="21872-103">List users</span></span>

<span data-ttu-id="21872-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21872-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21872-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="21872-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="21872-p101">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств. Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties). Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите свойства в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="21872-p101">This operation returns by default only a subset of the more commonly used properties for each user. These _default_ properties are noted in the [Properties](../resources/user.md#properties) section. To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="21872-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21872-109">Permissions</span></span>

<span data-ttu-id="21872-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21872-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21872-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21872-112">Permission type</span></span>      | <span data-ttu-id="21872-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21872-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21872-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21872-114">Delegated (work or school account)</span></span> | <span data-ttu-id="21872-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="21872-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="21872-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21872-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21872-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21872-117">Not supported.</span></span>    |
|<span data-ttu-id="21872-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21872-118">Application</span></span> | <span data-ttu-id="21872-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21872-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21872-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21872-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21872-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="21872-121">Optional query parameters</span></span>

<span data-ttu-id="21872-p103">Этот метод поддерживает [параметры запроса OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`. Вы можете использовать параметр `$search` в свойстве **displayName**. При добавлении или обновлении элементов для этого ресурса они индексируются для использования с параметрами запроса `$count` и `$search`. Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка. В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="21872-p103">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index. The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21872-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21872-127">Request headers</span></span>

| <span data-ttu-id="21872-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21872-128">Header</span></span> | <span data-ttu-id="21872-129">Значение</span><span class="sxs-lookup"><span data-stu-id="21872-129">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="21872-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21872-130">Authorization</span></span> | <span data-ttu-id="21872-131">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="21872-131">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="21872-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="21872-132">ConsistencyLevel</span></span> | <span data-ttu-id="21872-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="21872-133">eventual.</span></span> <span data-ttu-id="21872-134">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="21872-134">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="21872-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="21872-135">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21872-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21872-136">Request body</span></span>

<span data-ttu-id="21872-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21872-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21872-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="21872-138">Response</span></span>

<span data-ttu-id="21872-139">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="21872-139">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21872-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="21872-140">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="21872-141">Пример 1. Получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="21872-141">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="21872-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="21872-142">Request</span></span>

<span data-ttu-id="21872-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21872-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21872-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="21872-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="21872-145">C#</span><span class="sxs-lookup"><span data-stu-id="21872-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21872-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21872-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21872-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21872-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21872-148">Java</span><span class="sxs-lookup"><span data-stu-id="21872-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="21872-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="21872-149">Response</span></span>

<span data-ttu-id="21872-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21872-150">The following is an example of the response.</span></span> 
><span data-ttu-id="21872-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21872-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="21872-153">Пример 2. Получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="21872-153">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="21872-154">Найдите учетную запись пользователя, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="21872-154">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="21872-155">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="21872-155">When filtering on **identities** , you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="21872-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="21872-156">Request</span></span>

<span data-ttu-id="21872-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21872-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21872-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="21872-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="21872-159">C#</span><span class="sxs-lookup"><span data-stu-id="21872-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21872-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21872-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21872-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21872-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21872-162">Java</span><span class="sxs-lookup"><span data-stu-id="21872-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="21872-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="21872-163">Response</span></span>

<span data-ttu-id="21872-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21872-164">The following is an example of the response.</span></span> 
> <span data-ttu-id="21872-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21872-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="21872-167">Пример 3. Получение пользователей с указанием времени их последнего входа в систему</span><span class="sxs-lookup"><span data-stu-id="21872-167">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="21872-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="21872-168">Request</span></span>

<span data-ttu-id="21872-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21872-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="21872-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="21872-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="21872-171">C#</span><span class="sxs-lookup"><span data-stu-id="21872-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21872-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21872-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21872-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21872-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21872-174">Java</span><span class="sxs-lookup"><span data-stu-id="21872-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="21872-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="21872-175">Response</span></span>

<span data-ttu-id="21872-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21872-176">The following is an example of the response.</span></span> 
> <span data-ttu-id="21872-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21872-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="21872-179">Пример 4. Список времени последнего входа пользователей с определенным отображаемым именем</span><span class="sxs-lookup"><span data-stu-id="21872-179">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="21872-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="21872-180">Request</span></span>

<span data-ttu-id="21872-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21872-181">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="21872-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="21872-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="21872-183">C#</span><span class="sxs-lookup"><span data-stu-id="21872-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21872-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21872-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21872-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21872-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21872-186">Java</span><span class="sxs-lookup"><span data-stu-id="21872-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21872-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="21872-187">Response</span></span>

<span data-ttu-id="21872-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21872-188">The following is an example of the response.</span></span> 
> <span data-ttu-id="21872-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21872-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="21872-191">Пример 5: перечисление времени последнего входа пользователей в определенный временной диапазон</span><span class="sxs-lookup"><span data-stu-id="21872-191">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="21872-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="21872-192">Request</span></span>

<span data-ttu-id="21872-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21872-193">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="21872-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="21872-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="21872-195">C#</span><span class="sxs-lookup"><span data-stu-id="21872-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21872-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21872-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21872-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21872-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21872-198">Java</span><span class="sxs-lookup"><span data-stu-id="21872-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21872-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="21872-199">Response</span></span>

<span data-ttu-id="21872-200">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21872-200">The following is an example of the response.</span></span> 
> <span data-ttu-id="21872-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21872-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="21872-203">Пример 6. Получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="21872-203">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="21872-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="21872-204">Request</span></span>

<span data-ttu-id="21872-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21872-205">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="21872-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="21872-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="21872-207">C#</span><span class="sxs-lookup"><span data-stu-id="21872-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21872-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21872-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21872-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21872-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21872-210">Java</span><span class="sxs-lookup"><span data-stu-id="21872-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21872-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="21872-211">Response</span></span>

<span data-ttu-id="21872-212">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21872-212">The following is an example of the response.</span></span>

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

<span data-ttu-id="21872-213">893</span><span class="sxs-lookup"><span data-stu-id="21872-213">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="21872-214">Пример 7. Использование параметров $filter и $top для получения одного пользователя с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="21872-214">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="21872-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="21872-215">Request</span></span>

<span data-ttu-id="21872-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21872-216">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="21872-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="21872-217">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="21872-218">C#</span><span class="sxs-lookup"><span data-stu-id="21872-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21872-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21872-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21872-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21872-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21872-221">Java</span><span class="sxs-lookup"><span data-stu-id="21872-221">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21872-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="21872-222">Response</span></span>

<span data-ttu-id="21872-223">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21872-223">The following is an example of the response.</span></span>
><span data-ttu-id="21872-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21872-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="21872-226">Пример 8. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="21872-226">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="21872-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="21872-227">Request</span></span>

<span data-ttu-id="21872-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21872-228">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="21872-229">HTTP</span><span class="sxs-lookup"><span data-stu-id="21872-229">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="21872-230">C#</span><span class="sxs-lookup"><span data-stu-id="21872-230">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-wa-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21872-231">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21872-231">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-wa-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21872-232">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21872-232">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-wa-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21872-233">Java</span><span class="sxs-lookup"><span data-stu-id="21872-233">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-wa-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21872-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="21872-234">Response</span></span>

<span data-ttu-id="21872-235">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21872-235">The following is an example of the response.</span></span>
><span data-ttu-id="21872-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21872-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="21872-238">Пример 9. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="21872-238">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="21872-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="21872-239">Request</span></span>

<span data-ttu-id="21872-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21872-240">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="21872-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="21872-241">Response</span></span>

<span data-ttu-id="21872-242">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21872-242">The following is an example of the response.</span></span> 
> <span data-ttu-id="21872-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21872-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
