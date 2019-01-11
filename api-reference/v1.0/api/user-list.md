---
title: Список пользователей
description: Получение списка объектов user.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 16ecb08c5b0780a7d6ec11f11afb24969cecba4d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857759"
---
# <a name="list-users"></a><span data-ttu-id="a24a6-103">Список пользователей</span><span class="sxs-lookup"><span data-stu-id="a24a6-103">List users</span></span>

<span data-ttu-id="a24a6-104">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="a24a6-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a24a6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a24a6-105">Permissions</span></span>

<span data-ttu-id="a24a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a24a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a24a6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a24a6-108">Permission type</span></span>      | <span data-ttu-id="a24a6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a24a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a24a6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a24a6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a24a6-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a24a6-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a24a6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a24a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a24a6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a24a6-113">Not supported.</span></span>    |
|<span data-ttu-id="a24a6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a24a6-114">Application</span></span> | <span data-ttu-id="a24a6-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a24a6-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a24a6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a24a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a24a6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a24a6-117">Optional query parameters</span></span>

<span data-ttu-id="a24a6-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a24a6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a24a6-119">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="a24a6-119">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="a24a6-120">Чтобы возвратить альтернативный набор свойств, необходимо указать нужный набор свойств [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="a24a6-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="a24a6-121">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="a24a6-121">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="a24a6-p103">Примечание. Некоторые свойства не могут быть возвращены в пользовательском наборе. Следующие свойства поддерживаются только при [получении одного пользователя](./user-get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span><span class="sxs-lookup"><span data-stu-id="a24a6-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="a24a6-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a24a6-124">Request headers</span></span>

| <span data-ttu-id="a24a6-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a24a6-125">Header</span></span>        | <span data-ttu-id="a24a6-126">Значение</span><span class="sxs-lookup"><span data-stu-id="a24a6-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="a24a6-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a24a6-127">Authorization</span></span> | <span data-ttu-id="a24a6-128">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="a24a6-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="a24a6-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a24a6-129">Content-Type</span></span>  | <span data-ttu-id="a24a6-130">application/json</span><span class="sxs-lookup"><span data-stu-id="a24a6-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="a24a6-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a24a6-131">Request body</span></span>

<span data-ttu-id="a24a6-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a24a6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a24a6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a24a6-133">Response</span></span>

<span data-ttu-id="a24a6-134">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a24a6-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a24a6-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="a24a6-135">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="a24a6-136">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="a24a6-136">Example 1: Standard users request</span></span>

<span data-ttu-id="a24a6-137">По умолчанию возвращается только стандартный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="a24a6-137">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> <span data-ttu-id="a24a6-138">В этом примере показаны запрос и ответ, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a24a6-138">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="a24a6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a24a6-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="a24a6-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="a24a6-140">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="a24a6-141">Пример 2. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="a24a6-141">Example 2: Users request using $select</span></span>

<span data-ttu-id="a24a6-142">Если вам необходим другой набор свойств, вы можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="a24a6-142">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="a24a6-143">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="a24a6-143">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="a24a6-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="a24a6-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```

##### <a name="response"></a><span data-ttu-id="a24a6-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a24a6-145">Response</span></span>

<span data-ttu-id="a24a6-146">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a24a6-146">Note: The response object shown here may be truncated for brevity.</span></span>
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
  "tocPath": ""
}-->
