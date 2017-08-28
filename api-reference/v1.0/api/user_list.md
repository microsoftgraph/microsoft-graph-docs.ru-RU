# <a name="list-users"></a><span data-ttu-id="e5ab3-101">Список пользователей</span><span class="sxs-lookup"><span data-stu-id="e5ab3-101">List users</span></span>

<span data-ttu-id="e5ab3-102">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="e5ab3-102">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5ab3-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5ab3-103">Permissions</span></span>

<span data-ttu-id="e5ab3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e5ab3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e5ab3-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5ab3-106">Permission type</span></span>      | <span data-ttu-id="e5ab3-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5ab3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5ab3-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5ab3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e5ab3-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5ab3-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5ab3-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5ab3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5ab3-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5ab3-111">Not supported.</span></span>    |
|<span data-ttu-id="e5ab3-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5ab3-112">Application</span></span> | <span data-ttu-id="e5ab3-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5ab3-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5ab3-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5ab3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5ab3-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e5ab3-115">Optional query parameters</span></span>

<span data-ttu-id="e5ab3-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e5ab3-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e5ab3-117">По умолчанию возвращается только стандартный набор свойств (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="e5ab3-117">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> 

<span data-ttu-id="e5ab3-p102">Чтобы возвратился альтернативный набор свойства, необходимо указать нужный набор [пользовательских](../resources/user.md) свойств с помощью параметра запроса ODATA `$select`. Например, чтобы вернуть свойства _displayName_, _givenName_, _id_ и _postalCode_, нужно добавить к запросу следующее: `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="e5ab3-p102">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the ODATA `$select` query parameter. For example, to return _displayName_, _givenName_, _id_ and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="e5ab3-p103">Примечание. Некоторые свойства не могут быть возвращены в пользовательском наборе. Следующие свойства поддерживаются только при [получении одного пользователя](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span><span class="sxs-lookup"><span data-stu-id="e5ab3-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5ab3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5ab3-122">Request headers</span></span>

| <span data-ttu-id="e5ab3-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5ab3-123">Header</span></span>        | <span data-ttu-id="e5ab3-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e5ab3-124">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="e5ab3-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5ab3-125">Authorization</span></span> | <span data-ttu-id="e5ab3-126">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="e5ab3-126">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="e5ab3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5ab3-127">Content-Type</span></span>  | <span data-ttu-id="e5ab3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e5ab3-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="e5ab3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5ab3-129">Request body</span></span>

<span data-ttu-id="e5ab3-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5ab3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5ab3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5ab3-131">Response</span></span>

<span data-ttu-id="e5ab3-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5ab3-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5ab3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e5ab3-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e5ab3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5ab3-134">Request</span></span>

<span data-ttu-id="e5ab3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5ab3-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="e5ab3-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5ab3-136">Response</span></span>

<span data-ttu-id="e5ab3-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e5ab3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
