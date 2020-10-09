---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 5896c4a544e8e75a0c248c2c90a18cc403c2d5ea
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405243"
---
# <a name="get-a-user"></a><span data-ttu-id="fcfe6-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="fcfe6-103">Get a user</span></span>

<span data-ttu-id="fcfe6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcfe6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcfe6-105">Получение свойств и связей объекта user.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-105">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="fcfe6-106">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="fcfe6-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="fcfe6-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="fcfe6-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="fcfe6-109">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **user**.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-109">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcfe6-110">Разрешения:</span><span class="sxs-lookup"><span data-stu-id="fcfe6-110">Permissions</span></span>
<span data-ttu-id="fcfe6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcfe6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcfe6-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcfe6-113">Permission type</span></span>      | <span data-ttu-id="fcfe6-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcfe6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcfe6-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcfe6-115">Delegated (work or school account)</span></span> | <span data-ttu-id="fcfe6-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fcfe6-116">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fcfe6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcfe6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcfe6-118">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcfe6-118">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="fcfe6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcfe6-119">Application</span></span> | <span data-ttu-id="fcfe6-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcfe6-120">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

<span data-ttu-id="fcfe6-121">Для вызова конечной точки `/me` требуется вход пользователя и, следовательно, делегированное разрешение.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-121">Calling the `/me` endpoint requires a signed-in user and therefore a delegated permission.</span></span> <span data-ttu-id="fcfe6-122">Разрешения приложений не поддерживаются при использовании конечной точки `/me`.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-122">Application permissions are not supported when using the `/me` endpoint.</span></span>

<span data-ttu-id="fcfe6-123">Для определенного пользователя:</span><span class="sxs-lookup"><span data-stu-id="fcfe6-123">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="fcfe6-124">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="fcfe6-124">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcfe6-125">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="fcfe6-125">Optional query parameters</span></span>

<span data-ttu-id="fcfe6-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcfe6-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcfe6-127">Request headers</span></span>

| <span data-ttu-id="fcfe6-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcfe6-128">Header</span></span>       | <span data-ttu-id="fcfe6-129">Значение</span><span class="sxs-lookup"><span data-stu-id="fcfe6-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="fcfe6-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcfe6-130">Authorization</span></span>  | <span data-ttu-id="fcfe6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="fcfe6-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fcfe6-133">Content-Type</span></span>   | <span data-ttu-id="fcfe6-134">application/json</span><span class="sxs-lookup"><span data-stu-id="fcfe6-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcfe6-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcfe6-135">Request body</span></span>

<span data-ttu-id="fcfe6-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcfe6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcfe6-137">Response</span></span>

<span data-ttu-id="fcfe6-138">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-138">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="fcfe6-139">В случае успешной обработки запроса этот метод возвращает `202 Accepted`, но серверу требуется дополнительное время для выполнения соответствующих фоновых операций.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-139">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="fcfe6-140">Пример</span><span class="sxs-lookup"><span data-stu-id="fcfe6-140">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="fcfe6-141">Пример 1. Получение свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="fcfe6-141">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="fcfe6-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcfe6-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fcfe6-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcfe6-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="c"></a>[<span data-ttu-id="fcfe6-144">C#</span><span class="sxs-lookup"><span data-stu-id="fcfe6-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fcfe6-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fcfe6-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fcfe6-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fcfe6-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fcfe6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcfe6-147">Response</span></span>
<span data-ttu-id="fcfe6-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-148">Here is an example of the response.</span></span> <span data-ttu-id="fcfe6-149">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-149">Note: The response object shown here may be truncated for brevity.</span></span> 

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
```

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="fcfe6-150">Пример 2. Получение свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="fcfe6-150">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="fcfe6-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcfe6-151">Request</span></span>

<span data-ttu-id="fcfe6-152">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-152">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fcfe6-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcfe6-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="fcfe6-154">C#</span><span class="sxs-lookup"><span data-stu-id="fcfe6-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fcfe6-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fcfe6-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fcfe6-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fcfe6-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fcfe6-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcfe6-157">Response</span></span>

<span data-ttu-id="fcfe6-158">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fcfe6-158">The following example shows the response.</span></span>
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
```

## <a name="see-also"></a><span data-ttu-id="fcfe6-159">См. также</span><span class="sxs-lookup"><span data-stu-id="fcfe6-159">See also</span></span>

- [<span data-ttu-id="fcfe6-160">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="fcfe6-160">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fcfe6-161">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="fcfe6-161">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="fcfe6-162">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="fcfe6-162">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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