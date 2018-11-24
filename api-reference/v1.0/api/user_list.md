# <a name="list-users"></a><span data-ttu-id="4f9ef-101">Список пользователей</span><span class="sxs-lookup"><span data-stu-id="4f9ef-101">List users</span></span>

<span data-ttu-id="4f9ef-102">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="4f9ef-102">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f9ef-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f9ef-103">Permissions</span></span>

<span data-ttu-id="4f9ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f9ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f9ef-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f9ef-106">Permission type</span></span>      | <span data-ttu-id="4f9ef-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f9ef-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f9ef-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f9ef-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4f9ef-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4f9ef-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4f9ef-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f9ef-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f9ef-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f9ef-111">Not supported.</span></span>    |
|<span data-ttu-id="4f9ef-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f9ef-112">Application</span></span> | <span data-ttu-id="4f9ef-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f9ef-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f9ef-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f9ef-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f9ef-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f9ef-115">Optional query parameters</span></span>

<span data-ttu-id="4f9ef-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f9ef-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="4f9ef-117">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="4f9ef-117">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="4f9ef-118">Чтобы возвратить альтернативный набор свойств, необходимо указать нужный набор свойств [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="4f9ef-118">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="4f9ef-119">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="4f9ef-119">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="4f9ef-p103">Примечание. Некоторые свойства не могут быть возвращены в пользовательском наборе. Следующие свойства поддерживаются только при [получении одного пользователя](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span><span class="sxs-lookup"><span data-stu-id="4f9ef-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f9ef-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f9ef-122">Request headers</span></span>

| <span data-ttu-id="4f9ef-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f9ef-123">Header</span></span>        | <span data-ttu-id="4f9ef-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4f9ef-124">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="4f9ef-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f9ef-125">Authorization</span></span> | <span data-ttu-id="4f9ef-126">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="4f9ef-126">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="4f9ef-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f9ef-127">Content-Type</span></span>  | <span data-ttu-id="4f9ef-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4f9ef-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="4f9ef-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f9ef-129">Request body</span></span>

<span data-ttu-id="4f9ef-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f9ef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f9ef-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f9ef-131">Response</span></span>

<span data-ttu-id="4f9ef-132">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4f9ef-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f9ef-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="4f9ef-133">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="4f9ef-134">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="4f9ef-134">Example 1: Standard users request</span></span>

<span data-ttu-id="4f9ef-135">По умолчанию возвращается только стандартный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="4f9ef-135">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> <span data-ttu-id="4f9ef-136">В этом примере показаны запрос и ответ, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4f9ef-136">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="4f9ef-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f9ef-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="4f9ef-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f9ef-138">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="4f9ef-139">Пример 2. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="4f9ef-139">Example 2: Users request using $select</span></span>

<span data-ttu-id="4f9ef-140">Если вам необходим другой набор свойств, вы можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="4f9ef-140">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="4f9ef-141">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="4f9ef-141">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="4f9ef-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f9ef-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```

##### <a name="response"></a><span data-ttu-id="4f9ef-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f9ef-143">Response</span></span>

<span data-ttu-id="4f9ef-144">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="4f9ef-144">Note: The response object shown here may be truncated for brevity.</span></span>
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
