---
title: Перечисление пользователей
description: Получение списка объектов user.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2459c8a01facff8e233eb19482def8e18bec6957
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796859"
---
# <a name="list-users"></a><span data-ttu-id="1709a-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="1709a-103">List users</span></span>

<span data-ttu-id="1709a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1709a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1709a-105">Получение списка объектов [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="1709a-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1709a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1709a-106">Permissions</span></span>

<span data-ttu-id="1709a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1709a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1709a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1709a-109">Permission type</span></span>      | <span data-ttu-id="1709a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1709a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1709a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1709a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1709a-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1709a-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1709a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1709a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1709a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1709a-114">Not supported.</span></span>    |
|<span data-ttu-id="1709a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1709a-115">Application</span></span> | <span data-ttu-id="1709a-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1709a-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1709a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1709a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1709a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1709a-118">Optional query parameters</span></span>

<span data-ttu-id="1709a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика, в том числе `$search`, `$count`, `$filter` и `$select`.</span><span class="sxs-lookup"><span data-stu-id="1709a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, `$filter`, and `$select`.</span></span> <span data-ttu-id="1709a-120">`$search` можно использовать в свойстве **displayName** .</span><span class="sxs-lookup"><span data-stu-id="1709a-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="1709a-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="1709a-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="1709a-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="1709a-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="1709a-123">По умолчанию возвращается только ограниченный набор свойств ( **businessPhones** , **displayName** , **givenName** , **id** , **jobTitle** , **mail** , **mobilePhone** , **officeLocation** , **preferredLanguage** , **surname** и **userPrincipalName** ).</span><span class="sxs-lookup"><span data-stu-id="1709a-123">By default, only a limited set of properties are returned ( **businessPhones** , **displayName** , **givenName** , **id** , **jobTitle** , **mail** , **mobilePhone** , **officeLocation** , **preferredLanguage** , **surname** , and **userPrincipalName** ).</span></span> 

<span data-ttu-id="1709a-124">Чтобы получить альтернативный набор свойств, укажите нужный набор свойств объекта [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="1709a-124">To return an alternative property set, specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="1709a-125">Например, чтобы получить свойства **displayName** , **givenName** и **postalCode** , добавьте к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="1709a-125">For example, to return **displayName** , **givenName** , and **postalCode** , add the following to your query `$select=displayName,givenName,postalCode`.</span></span>

<span data-ttu-id="1709a-p104">Некоторые свойства невозможно возвращать в коллекции пользователей. Следующие свойства поддерживаются только при [получении одного пользователя](./user-get.md): **aboutMe** , **birthday** , **hireDate** , **interests** , **mySite** , **pastProjects** , **preferredName** , **responsibilities** , **schools** , **skills** , **mailboxSettings** .</span><span class="sxs-lookup"><span data-stu-id="1709a-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe** , **birthday** , **hireDate** , **interests** , **mySite** , **pastProjects** , **preferredName** , **responsibilities** , **schools** , **skills** , **mailboxSettings** .</span></span>

## <a name="request-headers"></a><span data-ttu-id="1709a-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1709a-128">Request headers</span></span>

| <span data-ttu-id="1709a-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1709a-129">Header</span></span>        | <span data-ttu-id="1709a-130">Значение</span><span class="sxs-lookup"><span data-stu-id="1709a-130">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="1709a-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1709a-131">Authorization</span></span> | <span data-ttu-id="1709a-132">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="1709a-132">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="1709a-133">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="1709a-133">ConsistencyLevel</span></span> | <span data-ttu-id="1709a-134">необязательный.</span><span class="sxs-lookup"><span data-stu-id="1709a-134">eventual.</span></span> <span data-ttu-id="1709a-135">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="1709a-135">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="1709a-136">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="1709a-136">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1709a-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1709a-137">Request body</span></span>

<span data-ttu-id="1709a-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1709a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1709a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1709a-139">Response</span></span>

<span data-ttu-id="1709a-140">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1709a-140">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="1709a-141">Если возвращается крупная коллекция пользователей, можно использовать [разбиение по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="1709a-141">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="1709a-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="1709a-142">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="1709a-143">Пример 1. Получение всех пользователей</span><span class="sxs-lookup"><span data-stu-id="1709a-143">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="1709a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="1709a-144">Request</span></span>

<span data-ttu-id="1709a-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1709a-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users
```

#### <a name="response"></a><span data-ttu-id="1709a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1709a-146">Response</span></span>

<span data-ttu-id="1709a-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1709a-147">The following is an example of the response.</span></span>

><span data-ttu-id="1709a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1709a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "otherMails":["contoso1@gmail.com"],
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="1709a-150">Пример 2. Получение учетной записи пользователя с помощью имени для входа</span><span class="sxs-lookup"><span data-stu-id="1709a-150">Example 2: Get a user account using a sign-in name</span></span>

#### <a name="request"></a><span data-ttu-id="1709a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="1709a-151">Request</span></span>

<span data-ttu-id="1709a-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1709a-152">The following is an example of the request.</span></span>

><span data-ttu-id="1709a-153">**Примечание.** При фильтрации по свойству **identities** требуется указывать параметры **issuer** и **issuerAssignedId** .</span><span class="sxs-lookup"><span data-stu-id="1709a-153">**Note:** When filtering on **identities** , you must supply both **issuer** and **issuerAssignedId** .</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```

#### <a name="response"></a><span data-ttu-id="1709a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1709a-154">Response</span></span>

<span data-ttu-id="1709a-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1709a-155">The following is an example of the response.</span></span> 

> <span data-ttu-id="1709a-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1709a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "displayName": "John Smith"
    }
  ]
}
```

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="1709a-158">Пример 3. Получение пользователей с указанием времени их последнего входа в систему</span><span class="sxs-lookup"><span data-stu-id="1709a-158">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="1709a-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="1709a-159">Request</span></span>

<span data-ttu-id="1709a-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1709a-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=displayName,userPrincipalName,signInActivity
```

#### <a name="response"></a><span data-ttu-id="1709a-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="1709a-161">Response</span></span>

<span data-ttu-id="1709a-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1709a-162">The following is an example of the response.</span></span>

><span data-ttu-id="1709a-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1709a-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(displayName,userPrincipalName,signInActivity)",
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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="1709a-165">Пример 4. Список времени последнего входа пользователей с определенным отображаемым именем</span><span class="sxs-lookup"><span data-stu-id="1709a-165">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="1709a-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="1709a-166">Request</span></span>

<span data-ttu-id="1709a-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1709a-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```

#### <a name="response"></a><span data-ttu-id="1709a-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="1709a-168">Response</span></span>

<span data-ttu-id="1709a-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1709a-169">The following is an example of the response.</span></span> 

> <span data-ttu-id="1709a-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1709a-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
  "value": [
    {
      "displayName": "Eric Solomon",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    }
  ]
}
```

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="1709a-172">Пример 5: перечисление времени последнего входа пользователей в определенный временной диапазон</span><span class="sxs-lookup"><span data-stu-id="1709a-172">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="1709a-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="1709a-173">Request</span></span>

<span data-ttu-id="1709a-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1709a-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_range"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="1709a-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="1709a-175">Response</span></span>

<span data-ttu-id="1709a-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1709a-176">The following is an example of the response.</span></span> 

> <span data-ttu-id="1709a-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1709a-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-05-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-04-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="1709a-179">Пример 6. Получение только количества пользователей</span><span class="sxs-lookup"><span data-stu-id="1709a-179">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="1709a-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="1709a-180">Request</span></span>

<span data-ttu-id="1709a-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1709a-181">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1709a-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="1709a-182">Response</span></span>

<span data-ttu-id="1709a-183">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1709a-183">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="1709a-184">Пример 7. Использование параметров $filter и $top для получения одного пользователя с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="1709a-184">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1709a-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="1709a-185">Request</span></span>

<span data-ttu-id="1709a-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1709a-186">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1709a-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="1709a-187">Response</span></span>

<span data-ttu-id="1709a-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1709a-188">The following is an example of the response.</span></span>

><span data-ttu-id="1709a-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1709a-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mail":"a@contoso.com",
      "mailNickname":"a_contoso.com#EXT#",
      "otherMails":["a@contoso.com"],
      "proxyAddresses":["SMTP:a@contoso.com"],
      "userPrincipalName":"a_contoso.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-8-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="1709a-191">Пример 8. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="1709a-191">Example 8: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1709a-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="1709a-192">Request</span></span>

<span data-ttu-id="1709a-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1709a-193">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_wa_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1709a-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="1709a-194">Response</span></span>

<span data-ttu-id="1709a-195">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1709a-195">The following is an example of the response.</span></span>

><span data-ttu-id="1709a-p113">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1709a-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    }
  ]
}
```

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="1709a-198">Пример 9. Использование параметра $search для получения пользователей с отображаемыми именами, содержащими буквы "wa" или буквы "to", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="1709a-198">Example 9: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1709a-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="1709a-199">Request</span></span>

<span data-ttu-id="1709a-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1709a-200">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_to_count"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$search="displayName:wa" OR "displayName:to"&$orderbydisplayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1709a-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="1709a-201">Response</span></span>

<span data-ttu-id="1709a-202">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1709a-202">The following is an example of the response.</span></span>

> <span data-ttu-id="1709a-p114">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1709a-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    },
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
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
