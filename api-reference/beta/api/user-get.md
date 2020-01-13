---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6e330ce8d12430e8c1bbfa70dd8dc8541f602ecd
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023112"
---
# <a name="get-a-user"></a><span data-ttu-id="92525-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="92525-103">Get a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92525-104">Получение свойств и связей объекта user.</span><span class="sxs-lookup"><span data-stu-id="92525-104">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="92525-105">Эта операция по умолчанию возвращает для каждого пользователя только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="92525-105">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="92525-106">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="92525-106">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="92525-107">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="92525-107">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="92525-108">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **user**.</span><span class="sxs-lookup"><span data-stu-id="92525-108">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="92525-109">Разрешения:</span><span class="sxs-lookup"><span data-stu-id="92525-109">Permissions</span></span>
<span data-ttu-id="92525-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92525-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92525-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92525-112">Permission type</span></span>      | <span data-ttu-id="92525-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92525-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92525-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92525-114">Delegated (work or school account)</span></span> | <span data-ttu-id="92525-115">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="92525-115">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="92525-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92525-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92525-117">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92525-117">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="92525-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92525-118">Application</span></span> | <span data-ttu-id="92525-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92525-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92525-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92525-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92525-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92525-121">Optional query parameters</span></span>
<span data-ttu-id="92525-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="92525-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="92525-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92525-123">Request headers</span></span>
| <span data-ttu-id="92525-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92525-124">Header</span></span>       | <span data-ttu-id="92525-125">Значение</span><span class="sxs-lookup"><span data-stu-id="92525-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="92525-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92525-126">Authorization</span></span>  | <span data-ttu-id="92525-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92525-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="92525-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92525-129">Content-Type</span></span>   | <span data-ttu-id="92525-130">application/json</span><span class="sxs-lookup"><span data-stu-id="92525-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="92525-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92525-131">Request body</span></span>
<span data-ttu-id="92525-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92525-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92525-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="92525-133">Response</span></span>

<span data-ttu-id="92525-134">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="92525-134">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="92525-135">В случае успешной обработки запроса этот метод возвращает `202 Accepted`, но серверу требуется дополнительное время для выполнения соответствующих фоновых операций.</span><span class="sxs-lookup"><span data-stu-id="92525-135">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="92525-136">Пример</span><span class="sxs-lookup"><span data-stu-id="92525-136">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="92525-137">Пример 1. Получение свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="92525-137">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="92525-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="92525-138">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="92525-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="92525-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92525-140">C#</span><span class="sxs-lookup"><span data-stu-id="92525-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92525-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92525-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92525-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92525-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92525-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="92525-143">Response</span></span>
<span data-ttu-id="92525-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92525-144">Here is an example of the response.</span></span> <span data-ttu-id="92525-145">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="92525-145">Note: The response object shown here may be truncated for brevity.</span></span> 

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

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="92525-146">Пример 2. Получение свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="92525-146">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="92525-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="92525-147">Request</span></span>

<span data-ttu-id="92525-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92525-148">The following example shows a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="92525-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="92525-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92525-150">C#</span><span class="sxs-lookup"><span data-stu-id="92525-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92525-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92525-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92525-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92525-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92525-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="92525-153">Response</span></span>

<span data-ttu-id="92525-154">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92525-154">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="92525-155">См. также</span><span class="sxs-lookup"><span data-stu-id="92525-155">See also</span></span>

- [<span data-ttu-id="92525-156">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="92525-156">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="92525-157">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="92525-157">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="92525-158">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="92525-158">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
