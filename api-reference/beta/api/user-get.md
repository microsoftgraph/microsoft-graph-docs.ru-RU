---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b522637b70989203a7fd33fd865ae9c0bdc9c60a
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351162"
---
# <a name="get-a-user"></a><span data-ttu-id="4056d-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="4056d-103">Get a user</span></span>

<span data-ttu-id="4056d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4056d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4056d-105">Получение свойств и связей объекта user.</span><span class="sxs-lookup"><span data-stu-id="4056d-105">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="4056d-106">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="4056d-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="4056d-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="4056d-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="4056d-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="4056d-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="4056d-109">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **user**.</span><span class="sxs-lookup"><span data-stu-id="4056d-109">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="4056d-110">Разрешения:</span><span class="sxs-lookup"><span data-stu-id="4056d-110">Permissions</span></span>
<span data-ttu-id="4056d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4056d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4056d-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4056d-113">Permission type</span></span>      | <span data-ttu-id="4056d-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4056d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4056d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4056d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4056d-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4056d-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4056d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4056d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4056d-118">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4056d-118">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="4056d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4056d-119">Application</span></span> | <span data-ttu-id="4056d-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4056d-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="4056d-121">Для вызова конечной точки `/me` требуется вход пользователя и, следовательно, делегированное разрешение.</span><span class="sxs-lookup"><span data-stu-id="4056d-121">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="4056d-122">Разрешения приложений не поддерживаются при использовании конечной точки `/me`.</span><span class="sxs-lookup"><span data-stu-id="4056d-122">Application permissions are not supported when using the `/me` endpoint.</span></span>

## <a name="http-request"></a><span data-ttu-id="4056d-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4056d-123">HTTP request</span></span>

<span data-ttu-id="4056d-124">Для определенного пользователя:</span><span class="sxs-lookup"><span data-stu-id="4056d-124">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

><span data-ttu-id="4056d-125">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="4056d-125">**Note:**</span></span>
> + <span data-ttu-id="4056d-p104">Если **userPrincipalName** начинается с символа `$`, нужно удалить косую черту (/) после `/users` и заключить **userPrincipalName** в скобки и одиночные кавычки. Например, `/users('$AdeleVance@contoso.com')`. Дополнительные сведения см. в списке [известных проблем](/graph/known-issues#users).</span><span class="sxs-lookup"><span data-stu-id="4056d-p104">When the **userPrincipalName** begins with a `$` character, remove the slash (/) after `/users` and enclose the **userPrincipalName** in parentheses and single quotes. For example, `/users('$AdeleVance@contoso.com')`. For details, see the [known issues](/graph/known-issues#users) list.</span></span>
> + <span data-ttu-id="4056d-129">Чтобы запросить пользователя B2B с помощью **userPrincipalName**, закодируйте хэш-символ (#).</span><span class="sxs-lookup"><span data-stu-id="4056d-129">To query a B2B user using the **userPrincipalName**, encode the hash (#) character.</span></span> <span data-ttu-id="4056d-130">То есть замените символ `#` на `%23`.</span><span class="sxs-lookup"><span data-stu-id="4056d-130">That is, replace the `#` symbol with `%23`.</span></span> <span data-ttu-id="4056d-131">Например, `/users/AdeleVance_adatum.com%23EXT%23@contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="4056d-131">For example, `/users/AdeleVance_adatum.com%23EXT%23@contoso.com`.</span></span>

<span data-ttu-id="4056d-132">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="4056d-132">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4056d-133">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="4056d-133">Optional query parameters</span></span>

<span data-ttu-id="4056d-134">Этот метод поддерживает `$select` [параметр запроса OData](/graph/query-parameters) для получения конкретных свойств пользователя, в том числе тех, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4056d-134">This method supports the `$select` [OData query parameter](/graph/query-parameters) to retrieve specific user properties, including those that are not returned by default.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4056d-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4056d-135">Request headers</span></span>

| <span data-ttu-id="4056d-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4056d-136">Header</span></span>       | <span data-ttu-id="4056d-137">Значение</span><span class="sxs-lookup"><span data-stu-id="4056d-137">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4056d-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4056d-138">Authorization</span></span>  | <span data-ttu-id="4056d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4056d-p106">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4056d-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4056d-141">Content-Type</span></span>   | <span data-ttu-id="4056d-142">application/json</span><span class="sxs-lookup"><span data-stu-id="4056d-142">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4056d-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4056d-143">Request body</span></span>

<span data-ttu-id="4056d-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4056d-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4056d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4056d-145">Response</span></span>

<span data-ttu-id="4056d-146">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4056d-146">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span> <span data-ttu-id="4056d-147">Он возвращает свойства по умолчанию, если не используется `$select` для указания конкретных свойств.</span><span class="sxs-lookup"><span data-stu-id="4056d-147">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

<span data-ttu-id="4056d-148">В случае успешной обработки запроса этот метод возвращает `202 Accepted`, но серверу требуется дополнительное время для выполнения соответствующих фоновых операций.</span><span class="sxs-lookup"><span data-stu-id="4056d-148">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="4056d-149">Пример</span><span class="sxs-lookup"><span data-stu-id="4056d-149">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="4056d-150">Пример 1. Получение свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="4056d-150">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="4056d-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="4056d-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4056d-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="4056d-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="c"></a>[<span data-ttu-id="4056d-153">C#</span><span class="sxs-lookup"><span data-stu-id="4056d-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4056d-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4056d-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4056d-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4056d-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4056d-156">Java</span><span class="sxs-lookup"><span data-stu-id="4056d-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4056d-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="4056d-157">Response</span></span>
<span data-ttu-id="4056d-p108">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4056d-p108">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "Adele Vance",
   "givenName": "Adele",
   "jobTitle": "Retail Manager",
   "mail": "AdeleV@contoso.onmicrosoft.com",
   "mobilePhone": "+1 425 555 0109",
   "officeLocation": "18/2111",
   "preferredLanguage": "en-US",
   "surname": "Vance",
   "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
   "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="4056d-160">Пример 2. Получение свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="4056d-160">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="4056d-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="4056d-161">Request</span></span>

<span data-ttu-id="4056d-162">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4056d-162">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4056d-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="4056d-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="4056d-164">C#</span><span class="sxs-lookup"><span data-stu-id="4056d-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4056d-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4056d-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4056d-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4056d-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4056d-167">Java</span><span class="sxs-lookup"><span data-stu-id="4056d-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4056d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="4056d-168">Response</span></span>

<span data-ttu-id="4056d-169">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4056d-169">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
      "displayName": "Adele Vance",
      "givenName": "Adele",
      "jobTitle": "Retail Manager",
      "mail": "AdeleV@contoso.onmicrosoft.com",
      "mobilePhone": "+1 425 555 0109",
      "officeLocation": "18/2111",
      "preferredLanguage": "en-US",
      "surname": "Vance",
      "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
      "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
}
```

## <a name="see-also"></a><span data-ttu-id="4056d-170">См. также</span><span class="sxs-lookup"><span data-stu-id="4056d-170">See also</span></span>

- [<span data-ttu-id="4056d-171">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="4056d-171">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4056d-172">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4056d-172">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="4056d-173">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4056d-173">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
