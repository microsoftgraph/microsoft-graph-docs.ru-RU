---
title: Получение пользователя
description: Получение свойств и связей объекта user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2632dfa8395d7ad68ae280e448eb095582827dd2
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538534"
---
# <a name="get-a-user"></a><span data-ttu-id="5011e-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="5011e-103">Get a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5011e-104">Получение свойств и связей объекта user.</span><span class="sxs-lookup"><span data-stu-id="5011e-104">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="5011e-105">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **user**.</span><span class="sxs-lookup"><span data-stu-id="5011e-105">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="5011e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5011e-106">Permissions</span></span>
<span data-ttu-id="5011e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5011e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5011e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5011e-109">Permission type</span></span>      | <span data-ttu-id="5011e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5011e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5011e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5011e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5011e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5011e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5011e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5011e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5011e-114">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5011e-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="5011e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5011e-115">Application</span></span> | <span data-ttu-id="5011e-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5011e-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5011e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5011e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5011e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5011e-118">Optional query parameters</span></span>
<span data-ttu-id="5011e-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5011e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5011e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5011e-120">Request headers</span></span>
| <span data-ttu-id="5011e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5011e-121">Header</span></span>       | <span data-ttu-id="5011e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5011e-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="5011e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5011e-123">Authorization</span></span>  | <span data-ttu-id="5011e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5011e-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5011e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5011e-126">Content-Type</span></span>   | <span data-ttu-id="5011e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5011e-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5011e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5011e-128">Request body</span></span>
<span data-ttu-id="5011e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5011e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5011e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5011e-130">Response</span></span>

<span data-ttu-id="5011e-131">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5011e-131">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="5011e-132">В случае успешной обработки запроса этот метод возвращает `202 Accepted`, но серверу требуется дополнительное время для выполнения соответствующих фоновых операций.</span><span class="sxs-lookup"><span data-stu-id="5011e-132">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="5011e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5011e-133">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="5011e-134">Пример 1. Получение свойств вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="5011e-134">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="5011e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="5011e-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5011e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5011e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5011e-137">C#</span><span class="sxs-lookup"><span data-stu-id="5011e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5011e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5011e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5011e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5011e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5011e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5011e-140">Response</span></span>
<span data-ttu-id="5011e-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5011e-141">Here is an example of the response.</span></span> <span data-ttu-id="5011e-142">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="5011e-142">Note: The response object shown here may be truncated for brevity.</span></span> 

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

### <a name="example-2-get-the-properties-of-the-specified-user"></a><span data-ttu-id="5011e-143">Пример 2. Получение свойств указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="5011e-143">Example 2: Get the properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="5011e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="5011e-144">Request</span></span>

<span data-ttu-id="5011e-145">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5011e-145">The following example shows a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5011e-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5011e-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_other_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5011e-147">C#</span><span class="sxs-lookup"><span data-stu-id="5011e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5011e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5011e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5011e-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5011e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5011e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="5011e-150">Response</span></span>

<span data-ttu-id="5011e-151">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5011e-151">The following example shows the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5011e-152">См. также</span><span class="sxs-lookup"><span data-stu-id="5011e-152">See also</span></span>

- [<span data-ttu-id="5011e-153">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="5011e-153">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5011e-154">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5011e-154">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5011e-155">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5011e-155">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
