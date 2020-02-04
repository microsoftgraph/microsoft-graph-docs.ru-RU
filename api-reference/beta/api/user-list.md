---
title: Перечисление пользователей
description: Получение списка объектов user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5c56bb12953c756099d7c66d913658739e32ee71
ms.sourcegitcommit: 360d176a29047a2686f1bff076f15c6ce9d12ef5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/04/2020
ms.locfileid: "41711726"
---
# <a name="list-users"></a><span data-ttu-id="376b2-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="376b2-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="376b2-104">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="376b2-104">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="376b2-105">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="376b2-105">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="376b2-106">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="376b2-106">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="376b2-107">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="376b2-107">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="376b2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="376b2-108">Permissions</span></span>

<span data-ttu-id="376b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="376b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="376b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="376b2-111">Permission type</span></span>      | <span data-ttu-id="376b2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="376b2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="376b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="376b2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="376b2-114">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="376b2-114">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="376b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="376b2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="376b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="376b2-116">Not supported.</span></span>    |
|<span data-ttu-id="376b2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="376b2-117">Application</span></span> | <span data-ttu-id="376b2-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376b2-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="376b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="376b2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="376b2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="376b2-120">Optional query parameters</span></span>

<span data-ttu-id="376b2-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="376b2-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="376b2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="376b2-122">Request headers</span></span>
| <span data-ttu-id="376b2-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="376b2-123">Header</span></span>        | <span data-ttu-id="376b2-124">Значение</span><span class="sxs-lookup"><span data-stu-id="376b2-124">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="376b2-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="376b2-125">Authorization</span></span> | <span data-ttu-id="376b2-126">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="376b2-126">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="376b2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="376b2-127">Request body</span></span>

<span data-ttu-id="376b2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="376b2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="376b2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="376b2-129">Response</span></span>

<span data-ttu-id="376b2-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="376b2-130">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="376b2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="376b2-131">Example</span></span>

### <a name="example-1-list-all-users"></a><span data-ttu-id="376b2-132">Пример 1. Список всех пользователей</span><span class="sxs-lookup"><span data-stu-id="376b2-132">Example 1: List all users</span></span>

#### <a name="request"></a><span data-ttu-id="376b2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="376b2-133">Request</span></span>

<span data-ttu-id="376b2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="376b2-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="376b2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="376b2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="376b2-136">C#</span><span class="sxs-lookup"><span data-stu-id="376b2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="376b2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="376b2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="376b2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="376b2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="376b2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="376b2-139">Response</span></span>

<span data-ttu-id="376b2-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="376b2-140">The following is an example of the response.</span></span> 
><span data-ttu-id="376b2-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="376b2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="376b2-143">Пример 2. Поиск учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="376b2-143">Example 2: Find a user account using a sign-in name</span></span>

<span data-ttu-id="376b2-144">Найдите учетную запись пользователя в клиенте B2C, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="376b2-144">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="376b2-145">Этот запрос может использоваться службой поддержки для поиска учетной записи пользователя в клиенте B2C (в данном примере клиентом B2C является contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="376b2-145">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="376b2-146">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="376b2-146">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="376b2-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="376b2-147">Request</span></span>

<span data-ttu-id="376b2-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="376b2-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="376b2-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="376b2-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="376b2-150">C#</span><span class="sxs-lookup"><span data-stu-id="376b2-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="376b2-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="376b2-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="376b2-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="376b2-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="376b2-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="376b2-153">Response</span></span>

<span data-ttu-id="376b2-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="376b2-154">The following is an example of the response.</span></span> 
> <span data-ttu-id="376b2-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="376b2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 108

{
  "value": [
    {
      "displayName": "John Smith",
      "id": "4c7be08b-361f-41a8-b1ef-1712f7a3dfb2"
    }
  ]
}
```

### <a name="example-3--list-users-including-their-last-sign-in-time"></a><span data-ttu-id="376b2-157">Пример 3. Перечисление пользователей с указанием времени их последнего входа в систему</span><span class="sxs-lookup"><span data-stu-id="376b2-157">Example 3:  List users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="376b2-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="376b2-158">Request</span></span>

<span data-ttu-id="376b2-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="376b2-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="376b2-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="376b2-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="376b2-161">C#</span><span class="sxs-lookup"><span data-stu-id="376b2-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="376b2-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="376b2-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="376b2-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="376b2-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="376b2-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="376b2-164">Response</span></span>

<span data-ttu-id="376b2-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="376b2-165">The following is an example of the response.</span></span> 
> <span data-ttu-id="376b2-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="376b2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
