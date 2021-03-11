---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e6caed0bcd6a8327068726a403b7531354864a25
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720139"
---
# <a name="get-a-user"></a><span data-ttu-id="5d97b-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="5d97b-103">Get a user</span></span>

<span data-ttu-id="5d97b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d97b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d97b-105">Получение свойств и связей объекта user.</span><span class="sxs-lookup"><span data-stu-id="5d97b-105">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="5d97b-106">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="5d97b-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="5d97b-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="5d97b-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="5d97b-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="5d97b-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="5d97b-109">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **user**.</span><span class="sxs-lookup"><span data-stu-id="5d97b-109">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d97b-110">Разрешения:</span><span class="sxs-lookup"><span data-stu-id="5d97b-110">Permissions</span></span>
<span data-ttu-id="5d97b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d97b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d97b-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d97b-113">Permission type</span></span>      | <span data-ttu-id="5d97b-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d97b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d97b-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d97b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="5d97b-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d97b-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5d97b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d97b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d97b-118">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d97b-118">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="5d97b-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d97b-119">Application</span></span> | <span data-ttu-id="5d97b-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d97b-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="5d97b-121">Для вызова конечной точки `/me` требуется вход пользователя и, следовательно, делегированное разрешение.</span><span class="sxs-lookup"><span data-stu-id="5d97b-121">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="5d97b-122">Разрешения приложений не поддерживаются при использовании конечной точки `/me`.</span><span class="sxs-lookup"><span data-stu-id="5d97b-122">Application permissions are not supported when using the `/me` endpoint.</span></span>

<span data-ttu-id="5d97b-123">Для определенного пользователя:</span><span class="sxs-lookup"><span data-stu-id="5d97b-123">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="5d97b-124">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="5d97b-124">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d97b-125">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="5d97b-125">Optional query parameters</span></span>

<span data-ttu-id="5d97b-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5d97b-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d97b-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d97b-127">Request headers</span></span>

| <span data-ttu-id="5d97b-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d97b-128">Header</span></span>       | <span data-ttu-id="5d97b-129">Значение</span><span class="sxs-lookup"><span data-stu-id="5d97b-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="5d97b-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d97b-130">Authorization</span></span>  | <span data-ttu-id="5d97b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d97b-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5d97b-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d97b-133">Content-Type</span></span>   | <span data-ttu-id="5d97b-134">application/json</span><span class="sxs-lookup"><span data-stu-id="5d97b-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d97b-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d97b-135">Request body</span></span>

<span data-ttu-id="5d97b-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d97b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d97b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d97b-137">Response</span></span>

<span data-ttu-id="5d97b-138">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5d97b-138">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="5d97b-139">В случае успешной обработки запроса этот метод возвращает `202 Accepted`, но серверу требуется дополнительное время для выполнения соответствующих фоновых операций.</span><span class="sxs-lookup"><span data-stu-id="5d97b-139">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="5d97b-140">Пример</span><span class="sxs-lookup"><span data-stu-id="5d97b-140">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="5d97b-141">Пример 1. Получение свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="5d97b-141">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="5d97b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d97b-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5d97b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d97b-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="c"></a>[<span data-ttu-id="5d97b-144">C#</span><span class="sxs-lookup"><span data-stu-id="5d97b-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d97b-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d97b-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d97b-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d97b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d97b-147">Java</span><span class="sxs-lookup"><span data-stu-id="5d97b-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5d97b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d97b-148">Response</span></span>
<span data-ttu-id="5d97b-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5d97b-149">Here is an example of the response.</span></span> <span data-ttu-id="5d97b-150">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="5d97b-150">Note: The response object shown here may be truncated for brevity.</span></span> 

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

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="5d97b-151">Пример 2. Получение свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="5d97b-151">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="5d97b-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d97b-152">Request</span></span>

<span data-ttu-id="5d97b-153">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d97b-153">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5d97b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d97b-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="5d97b-155">C#</span><span class="sxs-lookup"><span data-stu-id="5d97b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d97b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d97b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d97b-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d97b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d97b-158">Java</span><span class="sxs-lookup"><span data-stu-id="5d97b-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5d97b-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d97b-159">Response</span></span>

<span data-ttu-id="5d97b-160">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5d97b-160">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5d97b-161">См. также</span><span class="sxs-lookup"><span data-stu-id="5d97b-161">See also</span></span>

- [<span data-ttu-id="5d97b-162">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="5d97b-162">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5d97b-163">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5d97b-163">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5d97b-164">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5d97b-164">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
