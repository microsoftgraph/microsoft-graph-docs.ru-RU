---
title: Перечисление пользователей
description: Получение списка объектов user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2ba361107d022f9835767c57f99c1ce6333878fa
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054737"
---
# <a name="list-users"></a><span data-ttu-id="9bab9-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="9bab9-103">List users</span></span>

<span data-ttu-id="9bab9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bab9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bab9-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="9bab9-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="9bab9-106">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="9bab9-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="9bab9-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="9bab9-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="9bab9-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="9bab9-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bab9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9bab9-109">Permissions</span></span>

<span data-ttu-id="9bab9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bab9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bab9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bab9-112">Permission type</span></span>      | <span data-ttu-id="9bab9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bab9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bab9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bab9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9bab9-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9bab9-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9bab9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bab9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bab9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bab9-117">Not supported.</span></span>    |
|<span data-ttu-id="9bab9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9bab9-118">Application</span></span> | <span data-ttu-id="9bab9-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bab9-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bab9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9bab9-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9bab9-121">Optional query parameters</span></span>

<span data-ttu-id="9bab9-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="9bab9-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="9bab9-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="9bab9-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="9bab9-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="9bab9-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="9bab9-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="9bab9-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="9bab9-126">В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="9bab9-126">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bab9-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bab9-127">Request headers</span></span>

| <span data-ttu-id="9bab9-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9bab9-128">Header</span></span> | <span data-ttu-id="9bab9-129">Значение</span><span class="sxs-lookup"><span data-stu-id="9bab9-129">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="9bab9-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9bab9-130">Authorization</span></span> | <span data-ttu-id="9bab9-131">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="9bab9-131">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="9bab9-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="9bab9-132">ConsistencyLevel</span></span> | <span data-ttu-id="9bab9-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="9bab9-133">eventual.</span></span> <span data-ttu-id="9bab9-134">Этот заголовок и `$count` требуются при использовании `$search`, применении `$filter` с параметром запроса `$orderby` или применении `$filter` с логическим оператором `endsWith`.</span><span class="sxs-lookup"><span data-stu-id="9bab9-134">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter, or `$filter` with the `endsWith` logical operator.</span></span> <span data-ttu-id="9bab9-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="9bab9-135">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bab9-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bab9-136">Request body</span></span>

<span data-ttu-id="9bab9-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9bab9-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bab9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-138">Response</span></span>

<span data-ttu-id="9bab9-139">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-139">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9bab9-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="9bab9-140">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="9bab9-141">Пример 1. Получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="9bab9-141">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="9bab9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-142">Request</span></span>

<span data-ttu-id="9bab9-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bab9-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9bab9-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bab9-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="9bab9-145">C#</span><span class="sxs-lookup"><span data-stu-id="9bab9-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bab9-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bab9-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bab9-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bab9-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9bab9-148">Java</span><span class="sxs-lookup"><span data-stu-id="9bab9-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9bab9-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-149">Response</span></span>

<span data-ttu-id="9bab9-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-150">The following is an example of the response.</span></span> 
><span data-ttu-id="9bab9-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9bab9-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="9bab9-152">Пример 2. Получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="9bab9-152">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="9bab9-153">Найдите учетную запись пользователя, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="9bab9-153">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="9bab9-154">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="9bab9-154">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="9bab9-155">Значение **issuerAssignedId** должно быть адресом электронной почты учетной записи пользователя, а не именем субъекта-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="9bab9-155">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="9bab9-156">Если используется UPN, результатом будет пустой список.</span><span class="sxs-lookup"><span data-stu-id="9bab9-156">If a UPN is used, the response will be an empty list.</span></span>

#### <a name="request"></a><span data-ttu-id="9bab9-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-157">Request</span></span>

<span data-ttu-id="9bab9-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bab9-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9bab9-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bab9-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="9bab9-160">C#</span><span class="sxs-lookup"><span data-stu-id="9bab9-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bab9-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bab9-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bab9-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bab9-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9bab9-163">Java</span><span class="sxs-lookup"><span data-stu-id="9bab9-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9bab9-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-164">Response</span></span>

<span data-ttu-id="9bab9-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-165">The following is an example of the response.</span></span> 
> <span data-ttu-id="9bab9-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9bab9-166">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="9bab9-167">Пример 3. Получение пользователей с указанием времени их последнего входа в систему</span><span class="sxs-lookup"><span data-stu-id="9bab9-167">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="9bab9-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-168">Request</span></span>

<span data-ttu-id="9bab9-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bab9-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9bab9-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bab9-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="9bab9-171">C#</span><span class="sxs-lookup"><span data-stu-id="9bab9-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bab9-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bab9-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bab9-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bab9-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9bab9-174">Java</span><span class="sxs-lookup"><span data-stu-id="9bab9-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9bab9-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-175">Response</span></span>

<span data-ttu-id="9bab9-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-176">The following is an example of the response.</span></span> 
> <span data-ttu-id="9bab9-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9bab9-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="9bab9-178">Пример 4. Список времени последнего входа пользователей с определенным отображаемым именем</span><span class="sxs-lookup"><span data-stu-id="9bab9-178">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="9bab9-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-179">Request</span></span>

<span data-ttu-id="9bab9-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bab9-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9bab9-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bab9-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="9bab9-182">C#</span><span class="sxs-lookup"><span data-stu-id="9bab9-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bab9-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bab9-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bab9-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bab9-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9bab9-185">Java</span><span class="sxs-lookup"><span data-stu-id="9bab9-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9bab9-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-186">Response</span></span>

<span data-ttu-id="9bab9-187">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-187">The following is an example of the response.</span></span> 
> <span data-ttu-id="9bab9-188">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9bab9-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="9bab9-189">Пример 5: перечисление времени последнего входа пользователей в определенный временной диапазон</span><span class="sxs-lookup"><span data-stu-id="9bab9-189">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="9bab9-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-190">Request</span></span>

<span data-ttu-id="9bab9-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bab9-191">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_signin_last_time_range"
}-->
```http
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="9bab9-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-192">Response</span></span>

<span data-ttu-id="9bab9-193">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-193">The following is an example of the response.</span></span> 
> <span data-ttu-id="9bab9-194">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9bab9-194">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="9bab9-195">Пример 6. Получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="9bab9-195">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="9bab9-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-196">Request</span></span>

<span data-ttu-id="9bab9-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bab9-197">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9bab9-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-198">Response</span></span>

<span data-ttu-id="9bab9-199">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-199">The following is an example of the response.</span></span>

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

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="9bab9-200">Пример 7. Использование параметров $filter и $top для получения одного пользователя с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="9bab9-200">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9bab9-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-201">Request</span></span>

<span data-ttu-id="9bab9-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bab9-202">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9bab9-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-203">Response</span></span>

<span data-ttu-id="9bab9-204">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-204">The following is an example of the response.</span></span>
><span data-ttu-id="9bab9-205">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9bab9-205">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-8-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="9bab9-206">Пример 8. Использование параметра $filter для предоставления всем пользователям почты, которая заканчивается на "a@contoso.com", и в том числе количество возвращаемых объектов с результатами, отсортированными по userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9bab9-206">Example 8: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="9bab9-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-207">Request</span></span>

<span data-ttu-id="9bab9-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bab9-208">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9bab9-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bab9-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9bab9-210">C#</span><span class="sxs-lookup"><span data-stu-id="9bab9-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bab9-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bab9-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bab9-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bab9-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9bab9-213">Java</span><span class="sxs-lookup"><span data-stu-id="9bab9-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9bab9-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-214">Response</span></span>

<span data-ttu-id="9bab9-215">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-215">The following is an example of the response.</span></span>

><span data-ttu-id="9bab9-216">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9bab9-216">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="9bab9-217">Пример 9. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="9bab9-217">Example 9: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9bab9-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-218">Request</span></span>

<span data-ttu-id="9bab9-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bab9-219">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9bab9-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-220">Response</span></span>

<span data-ttu-id="9bab9-221">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-221">The following is an example of the response.</span></span>
><span data-ttu-id="9bab9-222">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9bab9-222">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-10-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="9bab9-223">Пример 10. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="9bab9-223">Example 10: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9bab9-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-224">Request</span></span>

<span data-ttu-id="9bab9-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bab9-225">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9bab9-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-226">Response</span></span>

<span data-ttu-id="9bab9-227">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-227">The following is an example of the response.</span></span> 
> <span data-ttu-id="9bab9-228">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9bab9-228">**Note:** The response object shown here might be shortened for readability.</span></span>

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


### <a name="example-11-use-filter-to-get-users-who-are-assigned-a-specific-license"></a><span data-ttu-id="9bab9-229">Пример 11. Использование $filter для получения пользователей, которым назначена определенная лицензия</span><span class="sxs-lookup"><span data-stu-id="9bab9-229">Example 11: Use $filter to get users who are assigned a specific license</span></span>

#### <a name="request"></a><span data-ttu-id="9bab9-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bab9-230">Request</span></span>

<span data-ttu-id="9bab9-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bab9-231">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_assignedLicenses"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=id,mail,assignedLicenses&$filter=assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)
```

#### <a name="response"></a><span data-ttu-id="9bab9-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bab9-232">Response</span></span>

<span data-ttu-id="9bab9-233">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bab9-233">The following is an example of the response.</span></span>

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
