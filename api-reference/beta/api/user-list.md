---
title: Перечисление пользователей
description: Получение списка объектов user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b842ca2a073bfaa7696a6c1c900b2f7d28ddb5de
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980198"
---
# <a name="list-users"></a><span data-ttu-id="519d3-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="519d3-103">List users</span></span>

<span data-ttu-id="519d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="519d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="519d3-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="519d3-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="519d3-106">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="519d3-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="519d3-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="519d3-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="519d3-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="519d3-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="519d3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="519d3-109">Permissions</span></span>

<span data-ttu-id="519d3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="519d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="519d3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="519d3-112">Permission type</span></span>      | <span data-ttu-id="519d3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="519d3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="519d3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="519d3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="519d3-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="519d3-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="519d3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="519d3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="519d3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="519d3-117">Not supported.</span></span>    |
|<span data-ttu-id="519d3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="519d3-118">Application</span></span> | <span data-ttu-id="519d3-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="519d3-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="519d3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="519d3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="519d3-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="519d3-121">Optional query parameters</span></span>

<span data-ttu-id="519d3-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="519d3-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="519d3-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="519d3-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="519d3-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="519d3-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="519d3-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="519d3-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="519d3-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="519d3-126">Request headers</span></span>

| <span data-ttu-id="519d3-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="519d3-127">Header</span></span> | <span data-ttu-id="519d3-128">Значение</span><span class="sxs-lookup"><span data-stu-id="519d3-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="519d3-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="519d3-129">Authorization</span></span> | <span data-ttu-id="519d3-130">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="519d3-130">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="519d3-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="519d3-131">ConsistencyLevel</span></span> | <span data-ttu-id="519d3-132">необязательный.</span><span class="sxs-lookup"><span data-stu-id="519d3-132">eventual.</span></span> <span data-ttu-id="519d3-133">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="519d3-133">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="519d3-134">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="519d3-134">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="519d3-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="519d3-135">Request body</span></span>

<span data-ttu-id="519d3-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="519d3-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="519d3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="519d3-137">Response</span></span>

<span data-ttu-id="519d3-138">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="519d3-138">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="519d3-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="519d3-139">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="519d3-140">Пример 1. Получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="519d3-140">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="519d3-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="519d3-141">Request</span></span>

<span data-ttu-id="519d3-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="519d3-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="519d3-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="519d3-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="519d3-144">C#</span><span class="sxs-lookup"><span data-stu-id="519d3-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="519d3-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519d3-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="519d3-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="519d3-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="519d3-147">Java</span><span class="sxs-lookup"><span data-stu-id="519d3-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="519d3-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="519d3-148">Response</span></span>

<span data-ttu-id="519d3-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="519d3-149">The following is an example of the response.</span></span> 
><span data-ttu-id="519d3-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="519d3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="519d3-152">Пример 2. Получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="519d3-152">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="519d3-153">Найдите учетную запись пользователя, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="519d3-153">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="519d3-154">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="519d3-154">When filtering on **identities** , you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="519d3-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="519d3-155">Request</span></span>

<span data-ttu-id="519d3-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="519d3-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="519d3-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="519d3-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="519d3-158">C#</span><span class="sxs-lookup"><span data-stu-id="519d3-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="519d3-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519d3-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="519d3-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="519d3-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="519d3-161">Java</span><span class="sxs-lookup"><span data-stu-id="519d3-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="519d3-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="519d3-162">Response</span></span>

<span data-ttu-id="519d3-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="519d3-163">The following is an example of the response.</span></span> 
> <span data-ttu-id="519d3-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="519d3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="519d3-166">Пример 3. Получение пользователей с указанием времени их последнего входа в систему</span><span class="sxs-lookup"><span data-stu-id="519d3-166">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="519d3-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="519d3-167">Request</span></span>

<span data-ttu-id="519d3-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="519d3-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="519d3-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="519d3-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="519d3-170">C#</span><span class="sxs-lookup"><span data-stu-id="519d3-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="519d3-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519d3-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="519d3-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="519d3-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="519d3-173">Java</span><span class="sxs-lookup"><span data-stu-id="519d3-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="519d3-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="519d3-174">Response</span></span>

<span data-ttu-id="519d3-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="519d3-175">The following is an example of the response.</span></span> 
> <span data-ttu-id="519d3-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="519d3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="519d3-178">Пример 4. Список времени последнего входа пользователей с определенным отображаемым именем</span><span class="sxs-lookup"><span data-stu-id="519d3-178">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="519d3-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="519d3-179">Request</span></span>

<span data-ttu-id="519d3-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="519d3-180">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="519d3-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="519d3-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="519d3-182">C#</span><span class="sxs-lookup"><span data-stu-id="519d3-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="519d3-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519d3-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="519d3-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="519d3-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="519d3-185">Java</span><span class="sxs-lookup"><span data-stu-id="519d3-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="519d3-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="519d3-186">Response</span></span>

<span data-ttu-id="519d3-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="519d3-187">The following is an example of the response.</span></span> 
> <span data-ttu-id="519d3-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="519d3-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="519d3-190">Пример 5: перечисление времени последнего входа пользователей в определенный временной диапазон</span><span class="sxs-lookup"><span data-stu-id="519d3-190">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="519d3-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="519d3-191">Request</span></span>

<span data-ttu-id="519d3-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="519d3-192">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="519d3-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="519d3-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="519d3-194">C#</span><span class="sxs-lookup"><span data-stu-id="519d3-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="519d3-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519d3-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="519d3-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="519d3-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="519d3-197">Java</span><span class="sxs-lookup"><span data-stu-id="519d3-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="519d3-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="519d3-198">Response</span></span>

<span data-ttu-id="519d3-199">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="519d3-199">The following is an example of the response.</span></span> 
> <span data-ttu-id="519d3-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="519d3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="519d3-202">Пример 6. Получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="519d3-202">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="519d3-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="519d3-203">Request</span></span>

<span data-ttu-id="519d3-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="519d3-204">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="519d3-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="519d3-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="519d3-206">C#</span><span class="sxs-lookup"><span data-stu-id="519d3-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="519d3-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519d3-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="519d3-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="519d3-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="519d3-209">Java</span><span class="sxs-lookup"><span data-stu-id="519d3-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="519d3-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="519d3-210">Response</span></span>

<span data-ttu-id="519d3-211">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="519d3-211">The following is an example of the response.</span></span>

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

<span data-ttu-id="519d3-212">893</span><span class="sxs-lookup"><span data-stu-id="519d3-212">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="519d3-213">Пример 7. Использование параметров $filter и $top для получения одного пользователя с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="519d3-213">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="519d3-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="519d3-214">Request</span></span>

<span data-ttu-id="519d3-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="519d3-215">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="519d3-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="519d3-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="519d3-217">C#</span><span class="sxs-lookup"><span data-stu-id="519d3-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="519d3-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519d3-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="519d3-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="519d3-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="519d3-220">Java</span><span class="sxs-lookup"><span data-stu-id="519d3-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="519d3-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="519d3-221">Response</span></span>

<span data-ttu-id="519d3-222">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="519d3-222">The following is an example of the response.</span></span>
><span data-ttu-id="519d3-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="519d3-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="519d3-225">Пример 8. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="519d3-225">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="519d3-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="519d3-226">Request</span></span>

<span data-ttu-id="519d3-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="519d3-227">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="519d3-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="519d3-228">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="519d3-229">C#</span><span class="sxs-lookup"><span data-stu-id="519d3-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-wa-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="519d3-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519d3-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-wa-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="519d3-231">Objective-C</span><span class="sxs-lookup"><span data-stu-id="519d3-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-wa-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="519d3-232">Java</span><span class="sxs-lookup"><span data-stu-id="519d3-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-wa-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="519d3-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="519d3-233">Response</span></span>

<span data-ttu-id="519d3-234">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="519d3-234">The following is an example of the response.</span></span>
><span data-ttu-id="519d3-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="519d3-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="519d3-237">Пример 9. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="519d3-237">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="519d3-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="519d3-238">Request</span></span>

<span data-ttu-id="519d3-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="519d3-239">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="519d3-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="519d3-240">Response</span></span>

<span data-ttu-id="519d3-241">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="519d3-241">The following is an example of the response.</span></span> 
> <span data-ttu-id="519d3-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="519d3-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
