# <a name="get-a-user"></a><span data-ttu-id="404d9-101">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="404d9-101">Get a user</span></span>

<span data-ttu-id="404d9-102">Получение свойств и связей объекта пользователей.</span><span class="sxs-lookup"><span data-stu-id="404d9-102">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="404d9-p101">Примечание. При получении пользователя возвращается только стандартный набор свойств (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). С помощью параметра `$select` можно получить остальные свойства и связи объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="404d9-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="404d9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="404d9-105">Permissions</span></span>
<span data-ttu-id="404d9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="404d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="404d9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="404d9-108">Permission type</span></span>      | <span data-ttu-id="404d9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="404d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="404d9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="404d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="404d9-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="404d9-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="404d9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="404d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="404d9-113">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="404d9-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="404d9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="404d9-114">Application</span></span> | <span data-ttu-id="404d9-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="404d9-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="404d9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="404d9-116">HTTP request</span></span>
<span data-ttu-id="404d9-117">Для определенного пользователя:</span><span class="sxs-lookup"><span data-stu-id="404d9-117">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="404d9-118">Для вошедшего пользователя:</span><span class="sxs-lookup"><span data-stu-id="404d9-118">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="404d9-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="404d9-119">Optional query parameters</span></span>
<span data-ttu-id="404d9-120">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="404d9-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="404d9-121">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="404d9-121">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="404d9-122">Чтобы возвратить альтернативный набор свойств, необходимо указать нужный набор свойств [user](../resources/user.md) с помощью параметра запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="404d9-122">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="404d9-123">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="404d9-123">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="404d9-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="404d9-124">Request headers</span></span>
| <span data-ttu-id="404d9-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="404d9-125">Header</span></span>       | <span data-ttu-id="404d9-126">Значение</span><span class="sxs-lookup"><span data-stu-id="404d9-126">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="404d9-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="404d9-127">Authorization</span></span>  | <span data-ttu-id="404d9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="404d9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="404d9-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="404d9-130">Content-Type</span></span>   | <span data-ttu-id="404d9-131">application/json</span><span class="sxs-lookup"><span data-stu-id="404d9-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="404d9-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="404d9-132">Request body</span></span>
<span data-ttu-id="404d9-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="404d9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="404d9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="404d9-134">Response</span></span>

<span data-ttu-id="404d9-135">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [user](../resources/user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="404d9-135">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="404d9-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="404d9-136">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="404d9-137">Пример 1. Обычный запрос пользователей</span><span class="sxs-lookup"><span data-stu-id="404d9-137">Example 1: Standard users request</span></span>

<span data-ttu-id="404d9-138">По умолчанию возвращается только ограниченный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="404d9-138">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="404d9-139">В этом примере показаны запрос и ответ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="404d9-139">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="404d9-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="404d9-140">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

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
```


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="404d9-141">Пример 2. Запрос для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="404d9-141">Example 2: Signed-in user request</span></span>

<span data-ttu-id="404d9-142">Вы можете получить информацию о вошедшем пользователе, заменив `/users/{id | userPrincipalName}` на `/me`.</span><span class="sxs-lookup"><span data-stu-id="404d9-142">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="404d9-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="404d9-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="404d9-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="404d9-144">Response</span></span>

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
```

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="404d9-145">Пример 3. Запрос пользователей с помощью оператора $select</span><span class="sxs-lookup"><span data-stu-id="404d9-145">Example 2: Users request using $select</span></span>

<span data-ttu-id="404d9-146">Если вам нужен другой набор свойств, можете использовать параметр запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="404d9-146">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="404d9-147">Например, чтобы возвратить свойства _displayName_, _givenName_ и _postalCode_, вам следует добавить к запросу следующее: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="404d9-147">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="404d9-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="404d9-148">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="404d9-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="404d9-149">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "postalCode": "postalCode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
