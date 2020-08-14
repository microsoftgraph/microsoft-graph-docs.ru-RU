---
title: Перечисление пользователей
description: Получение списка объектов user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 38d9f6044a90e422d68e55466ffd1e6191c54caf
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643920"
---
# <a name="list-users"></a><span data-ttu-id="23b52-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="23b52-103">List users</span></span>

<span data-ttu-id="23b52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23b52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23b52-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="23b52-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="23b52-106">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="23b52-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="23b52-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="23b52-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="23b52-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="23b52-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="23b52-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23b52-109">Permissions</span></span>

<span data-ttu-id="23b52-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23b52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23b52-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23b52-112">Permission type</span></span>      | <span data-ttu-id="23b52-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23b52-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23b52-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23b52-114">Delegated (work or school account)</span></span> | <span data-ttu-id="23b52-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23b52-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="23b52-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23b52-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23b52-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23b52-117">Not supported.</span></span>    |
|<span data-ttu-id="23b52-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23b52-118">Application</span></span> | <span data-ttu-id="23b52-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23b52-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23b52-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23b52-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23b52-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23b52-121">Optional query parameters</span></span>

<span data-ttu-id="23b52-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="23b52-122">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="23b52-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="23b52-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="23b52-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="23b52-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="23b52-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="23b52-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23b52-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23b52-126">Request headers</span></span>

| <span data-ttu-id="23b52-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23b52-127">Header</span></span> | <span data-ttu-id="23b52-128">Значение</span><span class="sxs-lookup"><span data-stu-id="23b52-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="23b52-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23b52-129">Authorization</span></span> | <span data-ttu-id="23b52-130">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="23b52-130">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="23b52-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="23b52-131">ConsistencyLevel</span></span> | <span data-ttu-id="23b52-132">необязательный.</span><span class="sxs-lookup"><span data-stu-id="23b52-132">eventual.</span></span> <span data-ttu-id="23b52-133">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="23b52-133">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="23b52-134">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="23b52-134">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23b52-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23b52-135">Request body</span></span>

<span data-ttu-id="23b52-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23b52-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23b52-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b52-137">Response</span></span>

<span data-ttu-id="23b52-138">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="23b52-138">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23b52-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="23b52-139">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="23b52-140">Пример 1. Получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="23b52-140">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="23b52-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b52-141">Request</span></span>

<span data-ttu-id="23b52-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b52-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="23b52-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b52-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="23b52-144">C#</span><span class="sxs-lookup"><span data-stu-id="23b52-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23b52-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b52-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23b52-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b52-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="23b52-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b52-147">Response</span></span>

<span data-ttu-id="23b52-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b52-148">The following is an example of the response.</span></span> 
><span data-ttu-id="23b52-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b52-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="23b52-151">Пример 2. Получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="23b52-151">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="23b52-152">Найдите учетную запись пользователя, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="23b52-152">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="23b52-153">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="23b52-153">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="23b52-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b52-154">Request</span></span>

<span data-ttu-id="23b52-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b52-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="23b52-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b52-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="23b52-157">C#</span><span class="sxs-lookup"><span data-stu-id="23b52-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23b52-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b52-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23b52-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b52-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="23b52-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b52-160">Response</span></span>

<span data-ttu-id="23b52-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b52-161">The following is an example of the response.</span></span> 
> <span data-ttu-id="23b52-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b52-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="23b52-164">Пример 3. Получение пользователей с указанием времени их последнего входа в систему</span><span class="sxs-lookup"><span data-stu-id="23b52-164">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="23b52-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b52-165">Request</span></span>

<span data-ttu-id="23b52-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b52-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23b52-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b52-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="23b52-168">C#</span><span class="sxs-lookup"><span data-stu-id="23b52-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23b52-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b52-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23b52-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b52-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="23b52-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b52-171">Response</span></span>

<span data-ttu-id="23b52-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b52-172">The following is an example of the response.</span></span> 
> <span data-ttu-id="23b52-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b52-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="23b52-175">Пример 4. Список времени последнего входа пользователей с определенным отображаемым именем</span><span class="sxs-lookup"><span data-stu-id="23b52-175">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="23b52-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b52-176">Request</span></span>

<span data-ttu-id="23b52-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b52-177">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="23b52-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b52-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="23b52-179">C#</span><span class="sxs-lookup"><span data-stu-id="23b52-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23b52-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b52-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23b52-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b52-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23b52-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b52-182">Response</span></span>

<span data-ttu-id="23b52-183">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b52-183">The following is an example of the response.</span></span> 
> <span data-ttu-id="23b52-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b52-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="23b52-186">Пример 5: перечисление времени последнего входа пользователей в определенный временной диапазон</span><span class="sxs-lookup"><span data-stu-id="23b52-186">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="23b52-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b52-187">Request</span></span>

<span data-ttu-id="23b52-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b52-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="23b52-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b52-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="23b52-190">C#</span><span class="sxs-lookup"><span data-stu-id="23b52-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23b52-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b52-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23b52-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b52-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23b52-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b52-193">Response</span></span>

<span data-ttu-id="23b52-194">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b52-194">The following is an example of the response.</span></span> 
> <span data-ttu-id="23b52-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b52-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="23b52-197">Пример 6. Получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="23b52-197">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="23b52-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b52-198">Request</span></span>

<span data-ttu-id="23b52-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b52-199">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23b52-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b52-200">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="23b52-201">C#</span><span class="sxs-lookup"><span data-stu-id="23b52-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23b52-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b52-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23b52-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b52-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23b52-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b52-204">Response</span></span>

<span data-ttu-id="23b52-205">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b52-205">The following is an example of the response.</span></span>

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

<span data-ttu-id="23b52-206">893</span><span class="sxs-lookup"><span data-stu-id="23b52-206">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="23b52-207">Пример 7. Использование параметров $filter и $top для получения одного пользователя с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="23b52-207">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="23b52-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b52-208">Request</span></span>

<span data-ttu-id="23b52-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b52-209">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23b52-210">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b52-210">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="23b52-211">C#</span><span class="sxs-lookup"><span data-stu-id="23b52-211">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23b52-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b52-212">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23b52-213">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b52-213">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23b52-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b52-214">Response</span></span>

<span data-ttu-id="23b52-215">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b52-215">The following is an example of the response.</span></span>
><span data-ttu-id="23b52-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b52-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="23b52-218">Пример 8. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="23b52-218">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="23b52-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b52-219">Request</span></span>

<span data-ttu-id="23b52-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b52-220">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23b52-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b52-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="23b52-222">C#</span><span class="sxs-lookup"><span data-stu-id="23b52-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-wa-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23b52-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b52-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-wa-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23b52-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b52-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-wa-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23b52-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b52-225">Response</span></span>

<span data-ttu-id="23b52-226">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b52-226">The following is an example of the response.</span></span>
><span data-ttu-id="23b52-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b52-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="23b52-229">Пример 9. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="23b52-229">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="23b52-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b52-230">Request</span></span>

<span data-ttu-id="23b52-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b52-231">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="23b52-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b52-232">Response</span></span>

<span data-ttu-id="23b52-233">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b52-233">The following is an example of the response.</span></span> 
> <span data-ttu-id="23b52-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b52-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
