---
title: Перечисление пользователей
description: Получение списка объектов user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 235411d1b323bbacc5ffb3f86cf68242b8a41861
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316289"
---
# <a name="list-users"></a><span data-ttu-id="c4ad6-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="c4ad6-103">List users</span></span>

<span data-ttu-id="c4ad6-104">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4ad6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4ad6-105">Permissions</span></span>

<span data-ttu-id="c4ad6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4ad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4ad6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4ad6-108">Permission type</span></span>      | <span data-ttu-id="c4ad6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4ad6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4ad6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4ad6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4ad6-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4ad6-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4ad6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4ad6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4ad6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-113">Not supported.</span></span>    |
|<span data-ttu-id="c4ad6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4ad6-114">Application</span></span> | <span data-ttu-id="c4ad6-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4ad6-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4ad6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4ad6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4ad6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4ad6-117">Optional query parameters</span></span>

<span data-ttu-id="c4ad6-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c4ad6-119">По умолчанию возвращается только ограниченный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname** и **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="c4ad6-119">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> 

<span data-ttu-id="c4ad6-120">Чтобы получить альтернативный набор свойств, укажите нужный набор свойств объекта [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="c4ad6-121">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, добавьте к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-121">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

<span data-ttu-id="c4ad6-p103">Некоторые свойства невозможно возвращать в коллекции пользователей. Следующие свойства поддерживаются только при [получении одного пользователя](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings**</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4ad6-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4ad6-124">Request headers</span></span>

| <span data-ttu-id="c4ad6-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4ad6-125">Header</span></span>        | <span data-ttu-id="c4ad6-126">Значение</span><span class="sxs-lookup"><span data-stu-id="c4ad6-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="c4ad6-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4ad6-127">Authorization</span></span> | <span data-ttu-id="c4ad6-128">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="c4ad6-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="c4ad6-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4ad6-129">Content-Type</span></span>  | <span data-ttu-id="c4ad6-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c4ad6-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="c4ad6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4ad6-131">Request body</span></span>

<span data-ttu-id="c4ad6-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4ad6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4ad6-133">Response</span></span>

<span data-ttu-id="c4ad6-134">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="c4ad6-135">Если возвращается крупная коллекция пользователей, можно использовать [разбиение по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="c4ad6-135">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="c4ad6-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4ad6-136">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="c4ad6-137">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="c4ad6-137">Example 1: Standard users request</span></span>

<span data-ttu-id="c4ad6-138">По умолчанию возвращается только стандартный набор свойств (**businessPhones**, **displayName**, **givenName**, **id**, **jobTitle**, **mail**, **mobilePhone**, **officeLocation**, **preferredLanguage**, **surname**, **userPrincipalName**).</span><span class="sxs-lookup"><span data-stu-id="c4ad6-138">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> <span data-ttu-id="c4ad6-139">В этом примере показаны запрос и ответ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-139">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="c4ad6-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4ad6-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4ad6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4ad6-141">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4ad6-142">C#</span><span class="sxs-lookup"><span data-stu-id="c4ad6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4ad6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4ad6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4ad6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4ad6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c4ad6-145">Java</span><span class="sxs-lookup"><span data-stu-id="c4ad6-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c4ad6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4ad6-146">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="c4ad6-147">Пример 2. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="c4ad6-147">Example 2: Users request using $select</span></span>

<span data-ttu-id="c4ad6-148">Если вам нужен другой набор свойств, можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-148">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="c4ad6-149">Например, чтобы получить свойства **displayName**, **givenName** и **postalCode**, следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-149">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="c4ad6-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4ad6-150">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4ad6-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4ad6-151">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4ad6-152">C#</span><span class="sxs-lookup"><span data-stu-id="c4ad6-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-properties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4ad6-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4ad6-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-properties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4ad6-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4ad6-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-properties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c4ad6-155">Java</span><span class="sxs-lookup"><span data-stu-id="c4ad6-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-properties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c4ad6-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4ad6-156">Response</span></span>

<span data-ttu-id="c4ad6-157">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c4ad6-157">Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
