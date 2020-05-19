---
title: Перечисление пользователей
description: Получение списка объектов user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 5da2a929f054e942819786271aac004ed93baee6
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290695"
---
# <a name="list-users"></a><span data-ttu-id="2b75f-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="2b75f-103">List users</span></span>

<span data-ttu-id="2b75f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b75f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b75f-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="2b75f-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="2b75f-106">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="2b75f-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="2b75f-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="2b75f-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="2b75f-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="2b75f-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b75f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b75f-109">Permissions</span></span>

<span data-ttu-id="2b75f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b75f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b75f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b75f-112">Permission type</span></span>      | <span data-ttu-id="2b75f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b75f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b75f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b75f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2b75f-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All, Auditlogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b75f-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All, Auditlogs.Read.All</span></span> |
|<span data-ttu-id="2b75f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b75f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b75f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b75f-117">Not supported.</span></span>    |
|<span data-ttu-id="2b75f-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2b75f-118">Application</span></span> | <span data-ttu-id="2b75f-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Auditlogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b75f-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Auditlogs.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b75f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b75f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b75f-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b75f-121">Optional query parameters</span></span>

<span data-ttu-id="2b75f-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="2b75f-122">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="2b75f-123">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="2b75f-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="2b75f-124">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="2b75f-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="2b75f-125">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="2b75f-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b75f-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b75f-126">Request headers</span></span>

| <span data-ttu-id="2b75f-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b75f-127">Header</span></span> | <span data-ttu-id="2b75f-128">Значение</span><span class="sxs-lookup"><span data-stu-id="2b75f-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="2b75f-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b75f-129">Authorization</span></span> | <span data-ttu-id="2b75f-130">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="2b75f-130">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="2b75f-131">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="2b75f-131">ConsistencyLevel</span></span> | <span data-ttu-id="2b75f-132">закончить.</span><span class="sxs-lookup"><span data-stu-id="2b75f-132">eventual.</span></span> <span data-ttu-id="2b75f-133">Этот заголовок и `$count` обязательные при использовании `$search` `$filter` с `$orderby` параметром Query.</span><span class="sxs-lookup"><span data-stu-id="2b75f-133">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="2b75f-134">Он использует индекс, который может быть не последним в актуальном изменении объекта.</span><span class="sxs-lookup"><span data-stu-id="2b75f-134">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b75f-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b75f-135">Request body</span></span>

<span data-ttu-id="2b75f-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b75f-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b75f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b75f-137">Response</span></span>

<span data-ttu-id="2b75f-138">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2b75f-138">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b75f-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="2b75f-139">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="2b75f-140">Пример 1: получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="2b75f-140">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="2b75f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b75f-141">Request</span></span>

<span data-ttu-id="2b75f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b75f-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2b75f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b75f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="2b75f-144">C#</span><span class="sxs-lookup"><span data-stu-id="2b75f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b75f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b75f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b75f-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b75f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2b75f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b75f-147">Response</span></span>

<span data-ttu-id="2b75f-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b75f-148">The following is an example of the response.</span></span> 
><span data-ttu-id="2b75f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b75f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="2b75f-151">Пример 2: получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="2b75f-151">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="2b75f-152">Найдите учетную запись пользователя, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="2b75f-152">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="2b75f-153">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="2b75f-153">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="2b75f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b75f-154">Request</span></span>

<span data-ttu-id="2b75f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b75f-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2b75f-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b75f-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="2b75f-157">C#</span><span class="sxs-lookup"><span data-stu-id="2b75f-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b75f-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b75f-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b75f-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b75f-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2b75f-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b75f-160">Response</span></span>

<span data-ttu-id="2b75f-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b75f-161">The following is an example of the response.</span></span> 
> <span data-ttu-id="2b75f-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b75f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="2b75f-164">Пример 3: получение пользователей, включая время последнего входа</span><span class="sxs-lookup"><span data-stu-id="2b75f-164">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="2b75f-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b75f-165">Request</span></span>

<span data-ttu-id="2b75f-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b75f-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b75f-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b75f-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="2b75f-168">C#</span><span class="sxs-lookup"><span data-stu-id="2b75f-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b75f-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b75f-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b75f-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b75f-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2b75f-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b75f-171">Response</span></span>

<span data-ttu-id="2b75f-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b75f-172">The following is an example of the response.</span></span> 
> <span data-ttu-id="2b75f-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b75f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="2b75f-175">Пример 4. Список времени последнего входа пользователей с определенным отображаемым именем</span><span class="sxs-lookup"><span data-stu-id="2b75f-175">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="2b75f-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b75f-176">Request</span></span>

<span data-ttu-id="2b75f-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b75f-177">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```

#### <a name="response"></a><span data-ttu-id="2b75f-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b75f-178">Response</span></span>

<span data-ttu-id="2b75f-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b75f-179">The following is an example of the response.</span></span> 
> <span data-ttu-id="2b75f-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b75f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="2b75f-182">Пример 5: перечисление времени последнего входа пользователей в определенный временной диапазон</span><span class="sxs-lookup"><span data-stu-id="2b75f-182">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="2b75f-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b75f-183">Request</span></span>

<span data-ttu-id="2b75f-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b75f-184">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="2b75f-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b75f-185">Response</span></span>

<span data-ttu-id="2b75f-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b75f-186">The following is an example of the response.</span></span> 
> <span data-ttu-id="2b75f-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b75f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="2b75f-189">Пример 6: получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="2b75f-189">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="2b75f-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b75f-190">Request</span></span>

<span data-ttu-id="2b75f-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b75f-191">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="2b75f-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b75f-192">Response</span></span>

<span data-ttu-id="2b75f-193">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b75f-193">The following is an example of the response.</span></span>

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

<span data-ttu-id="2b75f-194">893</span><span class="sxs-lookup"><span data-stu-id="2b75f-194">893</span></span>


### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="2b75f-195">Пример 7: используйте $filter и $top, чтобы получить одного пользователя с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="2b75f-195">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2b75f-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b75f-196">Request</span></span>

<span data-ttu-id="2b75f-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b75f-197">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="2b75f-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b75f-198">Response</span></span>

<span data-ttu-id="2b75f-199">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b75f-199">The following is an example of the response.</span></span>
><span data-ttu-id="2b75f-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b75f-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="2b75f-202">Пример 8: использование $search для получения пользователям с отображаемыми именами, содержащими "WA", в том числе от количества возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="2b75f-202">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2b75f-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b75f-203">Request</span></span>

<span data-ttu-id="2b75f-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b75f-204">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="2b75f-205">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b75f-205">Response</span></span>

<span data-ttu-id="2b75f-206">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b75f-206">The following is an example of the response.</span></span>
><span data-ttu-id="2b75f-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b75f-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="2b75f-209">Пример 9: использование $search для получения пользователям с отображаемыми именами, содержащими буквы "WA" или "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="2b75f-209">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2b75f-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b75f-210">Request</span></span>

<span data-ttu-id="2b75f-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b75f-211">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="2b75f-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b75f-212">Response</span></span>

<span data-ttu-id="2b75f-213">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b75f-213">The following is an example of the response.</span></span> 
> <span data-ttu-id="2b75f-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b75f-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
