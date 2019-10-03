---
title: Перечисление пользователей
description: Получение списка объектов user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eac2031d6de80937598a66dd6086e7419dff3f1f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357544"
---
# <a name="list-users"></a><span data-ttu-id="33c83-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="33c83-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33c83-104">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="33c83-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="33c83-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33c83-105">Permissions</span></span>

<span data-ttu-id="33c83-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33c83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33c83-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33c83-108">Permission type</span></span>      | <span data-ttu-id="33c83-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33c83-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33c83-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33c83-110">Delegated (work or school account)</span></span> | <span data-ttu-id="33c83-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33c83-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33c83-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33c83-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33c83-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33c83-113">Not supported.</span></span>    |
|<span data-ttu-id="33c83-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33c83-114">Application</span></span> | <span data-ttu-id="33c83-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33c83-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33c83-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33c83-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33c83-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="33c83-117">Optional query parameters</span></span>

<span data-ttu-id="33c83-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="33c83-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33c83-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33c83-119">Request headers</span></span>
| <span data-ttu-id="33c83-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33c83-120">Header</span></span>        | <span data-ttu-id="33c83-121">Значение</span><span class="sxs-lookup"><span data-stu-id="33c83-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="33c83-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33c83-122">Authorization</span></span> | <span data-ttu-id="33c83-123">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="33c83-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="33c83-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33c83-124">Content-Type</span></span>  | <span data-ttu-id="33c83-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33c83-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="33c83-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33c83-126">Request body</span></span>

<span data-ttu-id="33c83-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33c83-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33c83-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="33c83-128">Response</span></span>

<span data-ttu-id="33c83-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33c83-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33c83-130">Пример</span><span class="sxs-lookup"><span data-stu-id="33c83-130">Example</span></span>

### <a name="example-1-list-all-users"></a><span data-ttu-id="33c83-131">Пример 1. Список всех пользователей</span><span class="sxs-lookup"><span data-stu-id="33c83-131">Example 1: List all users</span></span>

#### <a name="request"></a><span data-ttu-id="33c83-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="33c83-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="33c83-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="33c83-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33c83-134">C#</span><span class="sxs-lookup"><span data-stu-id="33c83-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33c83-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33c83-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33c83-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33c83-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="33c83-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="33c83-137">Response</span></span>

<span data-ttu-id="33c83-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33c83-138">Here is an example of the response.</span></span> 

><span data-ttu-id="33c83-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33c83-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-find-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="33c83-141">Пример 2. Поиск учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="33c83-141">Example 2: Find a user account using a sign-in name</span></span>

<span data-ttu-id="33c83-142">Найдите учетную запись пользователя в клиенте B2C, используя имя для входа (также называемое локальной учетной записью).</span><span class="sxs-lookup"><span data-stu-id="33c83-142">Find a user account in a B2C tenant, using a sign-in name (also known as a local account).</span></span> <span data-ttu-id="33c83-143">Этот запрос может использоваться службой поддержки для поиска учетной записи пользователя в клиенте B2C (в данном примере клиентом B2C является contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="33c83-143">This request can be used by a helpdesk to find a customer's user account, in a B2C tenant (in this example the B2C tenant is contoso.onmicrosoft.com).</span></span>

>[!NOTE]
><span data-ttu-id="33c83-144">При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId**.</span><span class="sxs-lookup"><span data-stu-id="33c83-144">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span>

#### <a name="request"></a><span data-ttu-id="33c83-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="33c83-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="33c83-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="33c83-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```http
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33c83-147">C#</span><span class="sxs-lookup"><span data-stu-id="33c83-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33c83-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33c83-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33c83-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33c83-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="33c83-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="33c83-150">Response</span></span>

<span data-ttu-id="33c83-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33c83-151">Here is an example of the response.</span></span> 

> <span data-ttu-id="33c83-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33c83-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
