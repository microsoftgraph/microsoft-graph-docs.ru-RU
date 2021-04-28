---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8a71a50714d18d4d4d8e91a4f5a7e0c0b31fe9e6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052637"
---
# <a name="get-a-user"></a><span data-ttu-id="f734c-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="f734c-103">Get a user</span></span>

<span data-ttu-id="f734c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f734c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f734c-105">Получение свойств и связей объекта user.</span><span class="sxs-lookup"><span data-stu-id="f734c-105">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="f734c-106">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="f734c-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="f734c-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="f734c-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="f734c-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="f734c-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="f734c-109">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **user**.</span><span class="sxs-lookup"><span data-stu-id="f734c-109">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="f734c-110">Разрешения:</span><span class="sxs-lookup"><span data-stu-id="f734c-110">Permissions</span></span>
<span data-ttu-id="f734c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f734c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f734c-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f734c-113">Permission type</span></span>      | <span data-ttu-id="f734c-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f734c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f734c-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f734c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f734c-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f734c-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f734c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f734c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f734c-118">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f734c-118">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="f734c-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f734c-119">Application</span></span> | <span data-ttu-id="f734c-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f734c-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="f734c-121">Для вызова конечной точки `/me` требуется вход пользователя и, следовательно, делегированное разрешение.</span><span class="sxs-lookup"><span data-stu-id="f734c-121">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="f734c-122">Разрешения приложений не поддерживаются при использовании конечной точки `/me`.</span><span class="sxs-lookup"><span data-stu-id="f734c-122">Application permissions are not supported when using the `/me` endpoint.</span></span>

<span data-ttu-id="f734c-123">Для определенного пользователя:</span><span class="sxs-lookup"><span data-stu-id="f734c-123">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="f734c-124">Обратите внимание, что если **userPrincipalName** начинается с символа `$`, нужно удалить косую черту (/) после `/users` и заключить **userPrincipalName** в скобки и одиночные кавычки.</span><span class="sxs-lookup"><span data-stu-id="f734c-124">Note that when the **userPrincipalName** begins with a `$` character, remove the slash (/) after `/users` and enclose the **userPrincipalName** in parentheses and single quotes.</span></span> <span data-ttu-id="f734c-125">Дополнительные сведения см. в списке [известных проблем](/graph/known-issues#users).</span><span class="sxs-lookup"><span data-stu-id="f734c-125">For details, see the [known issues](/graph/known-issues#users) list.</span></span>

<span data-ttu-id="f734c-126">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="f734c-126">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f734c-127">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="f734c-127">Optional query parameters</span></span>

<span data-ttu-id="f734c-128">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f734c-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f734c-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f734c-129">Request headers</span></span>

| <span data-ttu-id="f734c-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f734c-130">Header</span></span>       | <span data-ttu-id="f734c-131">Значение</span><span class="sxs-lookup"><span data-stu-id="f734c-131">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="f734c-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f734c-132">Authorization</span></span>  | <span data-ttu-id="f734c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f734c-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f734c-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f734c-135">Content-Type</span></span>   | <span data-ttu-id="f734c-136">application/json</span><span class="sxs-lookup"><span data-stu-id="f734c-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f734c-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f734c-137">Request body</span></span>

<span data-ttu-id="f734c-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f734c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f734c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f734c-139">Response</span></span>

<span data-ttu-id="f734c-140">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f734c-140">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="f734c-141">В случае успешной обработки запроса этот метод возвращает `202 Accepted`, но серверу требуется дополнительное время для выполнения соответствующих фоновых операций.</span><span class="sxs-lookup"><span data-stu-id="f734c-141">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="f734c-142">Пример</span><span class="sxs-lookup"><span data-stu-id="f734c-142">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="f734c-143">Пример 1. Получение свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="f734c-143">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="f734c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="f734c-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f734c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f734c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="c"></a>[<span data-ttu-id="f734c-146">C#</span><span class="sxs-lookup"><span data-stu-id="f734c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f734c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f734c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f734c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f734c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f734c-149">Java</span><span class="sxs-lookup"><span data-stu-id="f734c-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f734c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f734c-150">Response</span></span>
<span data-ttu-id="f734c-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f734c-151">Here is an example of the response.</span></span> <span data-ttu-id="f734c-152">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f734c-152">Note: The response object shown here might be shortened for readability.</span></span> 

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

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="f734c-153">Пример 2. Получение свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="f734c-153">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="f734c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="f734c-154">Request</span></span>

<span data-ttu-id="f734c-155">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f734c-155">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f734c-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="f734c-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="f734c-157">C#</span><span class="sxs-lookup"><span data-stu-id="f734c-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f734c-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f734c-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f734c-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f734c-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f734c-160">Java</span><span class="sxs-lookup"><span data-stu-id="f734c-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f734c-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f734c-161">Response</span></span>

<span data-ttu-id="f734c-162">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f734c-162">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f734c-163">См. также</span><span class="sxs-lookup"><span data-stu-id="f734c-163">See also</span></span>

- [<span data-ttu-id="f734c-164">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="f734c-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f734c-165">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f734c-165">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f734c-166">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f734c-166">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
