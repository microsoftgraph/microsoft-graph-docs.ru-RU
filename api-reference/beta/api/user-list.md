---
title: Перечисление пользователей
description: Получение списка объектов user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 09c296c88fc2b7ceab48018745b2686c08b8db21
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400987"
---
# <a name="list-users"></a><span data-ttu-id="ac950-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="ac950-103">List users</span></span>

<span data-ttu-id="ac950-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac950-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac950-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="ac950-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="ac950-106">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="ac950-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="ac950-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="ac950-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="ac950-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="ac950-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac950-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac950-109">Permissions</span></span>

<span data-ttu-id="ac950-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac950-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac950-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac950-112">Permission type</span></span>      | <span data-ttu-id="ac950-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac950-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac950-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac950-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ac950-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ac950-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ac950-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac950-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac950-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac950-117">Not supported.</span></span>    |
|<span data-ttu-id="ac950-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac950-118">Application</span></span> | <span data-ttu-id="ac950-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac950-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac950-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac950-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ac950-121">Optional query parameters</span></span>

<span data-ttu-id="ac950-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select` и `$top` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ac950-122">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="ac950-123">Некоторые запросы поддерживаются только при использовании заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`.</span><span class="sxs-lookup"><span data-stu-id="ac950-123">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="ac950-124">Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ac950-124">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> <span data-ttu-id="ac950-125">В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="ac950-125">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="ac950-p104">Примечание. Некоторые свойства не могут быть возвращены в пользовательском наборе. Следующие свойства поддерживаются только при [извлечении одного пользователя](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="ac950-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving a single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

<span data-ttu-id="ac950-128">Следующие свойства не поддерживаются в личных учетных записях Майкрософт и будут `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span><span class="sxs-lookup"><span data-stu-id="ac950-128">The following properties are not supported in personal Microsoft accounts and will be `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac950-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac950-129">Request headers</span></span>

| <span data-ttu-id="ac950-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac950-130">Header</span></span> | <span data-ttu-id="ac950-131">Значение</span><span class="sxs-lookup"><span data-stu-id="ac950-131">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="ac950-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac950-132">Authorization</span></span> | <span data-ttu-id="ac950-133">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="ac950-133">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="ac950-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="ac950-134">ConsistencyLevel</span></span> | <span data-ttu-id="ac950-135">необязательный.</span><span class="sxs-lookup"><span data-stu-id="ac950-135">eventual.</span></span> <span data-ttu-id="ac950-136">Этот заголовок и `$count` требуются при использовании `$search` или определенном использовании `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ac950-136">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="ac950-137">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ac950-137">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac950-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac950-138">Request body</span></span>

<span data-ttu-id="ac950-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac950-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac950-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-140">Response</span></span>

<span data-ttu-id="ac950-141">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-141">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac950-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="ac950-142">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="ac950-143">Пример 1. Получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="ac950-143">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="ac950-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-144">Request</span></span>

<span data-ttu-id="ac950-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac950-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac950-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac950-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="ac950-147">C#</span><span class="sxs-lookup"><span data-stu-id="ac950-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac950-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac950-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac950-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac950-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac950-150">Java</span><span class="sxs-lookup"><span data-stu-id="ac950-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ac950-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-151">Response</span></span>

<span data-ttu-id="ac950-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-152">The following is an example of the response.</span></span> 
><span data-ttu-id="ac950-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac950-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="ac950-154">Пример 2. Получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="ac950-154">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="ac950-155">Найдите учетную запись пользователя, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="ac950-155">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="ac950-156">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="ac950-156">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="ac950-157">Значение **issuerAssignedId** должно быть адресом электронной почты учетной записи пользователя, а не именем субъекта-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="ac950-157">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="ac950-158">Если используется UPN, результатом будет пустой список.</span><span class="sxs-lookup"><span data-stu-id="ac950-158">If a UPN is used, the response will be an empty list.</span></span>

#### <a name="request"></a><span data-ttu-id="ac950-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-159">Request</span></span>

<span data-ttu-id="ac950-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac950-160">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac950-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac950-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="ac950-162">C#</span><span class="sxs-lookup"><span data-stu-id="ac950-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac950-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac950-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac950-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac950-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac950-165">Java</span><span class="sxs-lookup"><span data-stu-id="ac950-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ac950-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-166">Response</span></span>

<span data-ttu-id="ac950-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-167">The following is an example of the response.</span></span> 
> <span data-ttu-id="ac950-168">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac950-168">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="ac950-169">Пример 3. Получение пользователей с указанием времени их последнего входа в систему</span><span class="sxs-lookup"><span data-stu-id="ac950-169">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="ac950-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-170">Request</span></span>

<span data-ttu-id="ac950-p107">Ниже приведен пример запроса. Сведения для свойства **signInActivity** требуют лицензии Azure AD Premium P1/P2 и разрешения AuditLog.Read.All.</span><span class="sxs-lookup"><span data-stu-id="ac950-p107">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>


# <a name="http"></a>[<span data-ttu-id="ac950-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac950-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="ac950-174">C#</span><span class="sxs-lookup"><span data-stu-id="ac950-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac950-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac950-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac950-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac950-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac950-177">Java</span><span class="sxs-lookup"><span data-stu-id="ac950-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ac950-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-178">Response</span></span>

<span data-ttu-id="ac950-179">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-179">The following is an example of the response.</span></span> 
> <span data-ttu-id="ac950-180">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac950-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="ac950-181">Пример 4. Список времени последнего входа пользователей с определенным отображаемым именем</span><span class="sxs-lookup"><span data-stu-id="ac950-181">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="ac950-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-182">Request</span></span>

<span data-ttu-id="ac950-p108">Ниже приведен пример запроса. Сведения для свойства **signInActivity** требуют лицензии Azure AD Premium P1/P2 и разрешения AuditLog.Read.All.</span><span class="sxs-lookup"><span data-stu-id="ac950-p108">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac950-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac950-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="ac950-186">C#</span><span class="sxs-lookup"><span data-stu-id="ac950-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac950-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac950-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac950-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac950-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac950-189">Java</span><span class="sxs-lookup"><span data-stu-id="ac950-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ac950-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-190">Response</span></span>

<span data-ttu-id="ac950-191">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-191">The following is an example of the response.</span></span> 
> <span data-ttu-id="ac950-192">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac950-192">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="ac950-193">Пример 5: перечисление времени последнего входа пользователей в определенный временной диапазон</span><span class="sxs-lookup"><span data-stu-id="ac950-193">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="ac950-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-194">Request</span></span>

<span data-ttu-id="ac950-p109">Ниже приведен пример запроса. Сведения для свойства **signInActivity** требуют лицензии Azure AD Premium P1/P2 и разрешения AuditLog.Read.All.</span><span class="sxs-lookup"><span data-stu-id="ac950-p109">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_signin_last_time_range"
}-->
```http
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="ac950-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-197">Response</span></span>

<span data-ttu-id="ac950-198">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-198">The following is an example of the response.</span></span> 
> <span data-ttu-id="ac950-199">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac950-199">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="ac950-200">Пример 6. Получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="ac950-200">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="ac950-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-201">Request</span></span>

<span data-ttu-id="ac950-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac950-202">The following is an example of the request.</span></span> <span data-ttu-id="ac950-203">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$count`.</span><span class="sxs-lookup"><span data-stu-id="ac950-203">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="ac950-204">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ac950-204">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ac950-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-205">Response</span></span>

<span data-ttu-id="ac950-206">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-206">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="ac950-207">Пример 7. Использование параметров $filter и $top для получения одного пользователя с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="ac950-207">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ac950-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-208">Request</span></span>

<span data-ttu-id="ac950-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac950-209">The following is an example of the request.</span></span> <span data-ttu-id="ac950-210">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual` и строка запроса `$count=true`, так как запрос содержит параметры запроса `$orderBy` и `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ac950-210">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="ac950-211">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ac950-211">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ac950-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-212">Response</span></span>

<span data-ttu-id="ac950-213">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-213">The following is an example of the response.</span></span>
><span data-ttu-id="ac950-214">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac950-214">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-8-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="ac950-215">Пример 8. Использование параметра $filter для предоставления всем пользователям почты, которая заканчивается на "a@contoso.com", и в том числе количество возвращаемых объектов с результатами, отсортированными по userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ac950-215">Example 8: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="ac950-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-216">Request</span></span>

<span data-ttu-id="ac950-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac950-217">The following is an example of the request.</span></span> <span data-ttu-id="ac950-218">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual` и строка запроса `$count=true`, так как запрос содержит параметры запроса `$orderBy` и `$filter`, а также использует оператор `endsWith`.</span><span class="sxs-lookup"><span data-stu-id="ac950-218">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters, and also uses the `endsWith` operator.</span></span> <span data-ttu-id="ac950-219">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ac950-219">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>


# <a name="http"></a>[<span data-ttu-id="ac950-220">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac950-220">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ac950-221">C#</span><span class="sxs-lookup"><span data-stu-id="ac950-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac950-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac950-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac950-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac950-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac950-224">Java</span><span class="sxs-lookup"><span data-stu-id="ac950-224">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ac950-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-225">Response</span></span>

<span data-ttu-id="ac950-226">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-226">The following is an example of the response.</span></span>

><span data-ttu-id="ac950-227">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac950-227">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users",
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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="ac950-228">Пример 9. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="ac950-228">Example 9: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ac950-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-229">Request</span></span>

<span data-ttu-id="ac950-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac950-230">The following is an example of the request.</span></span> <span data-ttu-id="ac950-231">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$search`.</span><span class="sxs-lookup"><span data-stu-id="ac950-231">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="ac950-232">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ac950-232">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ac950-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-233">Response</span></span>

<span data-ttu-id="ac950-234">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-234">The following is an example of the response.</span></span>
><span data-ttu-id="ac950-235">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac950-235">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-10-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="ac950-236">Пример 10. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="ac950-236">Example 10: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ac950-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-237">Request</span></span>

<span data-ttu-id="ac950-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac950-238">The following is an example of the request.</span></span> <span data-ttu-id="ac950-239">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$search`.</span><span class="sxs-lookup"><span data-stu-id="ac950-239">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="ac950-240">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ac950-240">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ac950-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-241">Response</span></span>

<span data-ttu-id="ac950-242">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-242">The following is an example of the response.</span></span> 
> <span data-ttu-id="ac950-243">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac950-243">**Note:** The response object shown here might be shortened for readability.</span></span>

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


### <a name="example-11-use-filter-to-get-users-who-are-assigned-a-specific-license"></a><span data-ttu-id="ac950-244">Пример 11. Использование $filter для получения пользователей, которым назначена определенная лицензия</span><span class="sxs-lookup"><span data-stu-id="ac950-244">Example 11: Use $filter to get users who are assigned a specific license</span></span>

#### <a name="request"></a><span data-ttu-id="ac950-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac950-245">Request</span></span>

<span data-ttu-id="ac950-246">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac950-246">The following is an example of the request.</span></span> <span data-ttu-id="ac950-247">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$search`.</span><span class="sxs-lookup"><span data-stu-id="ac950-247">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="ac950-248">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="ac950-248">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_assignedLicenses"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=id,mail,assignedLicenses&$filter=assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)
```

#### <a name="response"></a><span data-ttu-id="ac950-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac950-249">Response</span></span>

<span data-ttu-id="ac950-250">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac950-250">The following is an example of the response.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(id,mail,assignedLicenses)",
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
