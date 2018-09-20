# <a name="list-contacts"></a><span data-ttu-id="1b4a6-101">Список контактов</span><span class="sxs-lookup"><span data-stu-id="1b4a6-101">List contacts</span></span>

<span data-ttu-id="1b4a6-102">Получение коллекции контактов из папки контактов по умолчанию для пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="1b4a6-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>

<span data-ttu-id="1b4a6-103">Существует два сценария, в которых приложение может получать контакт из папки контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="1b4a6-103">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="1b4a6-104">Если программа имеет разрешения для приложения, или,</span><span class="sxs-lookup"><span data-stu-id="1b4a6-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="1b4a6-105">Если приложение имеет соответствующие делегированные [разрешения](#permissions) от одного пользователя и другой пользователь поделился календарем с этим пользователем или предоставил делегированный доступ к этому пользователю.</span><span class="sxs-lookup"><span data-stu-id="1b4a6-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="1b4a6-106">См. [сведения и примеры](../../../concepts/outlook-get-shared-contacts-folders.md).</span><span class="sxs-lookup"><span data-stu-id="1b4a6-106">See [details and an example](../../../concepts/outlook-get-shared-contacts-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="1b4a6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b4a6-107">Permissions</span></span>
<span data-ttu-id="1b4a6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b4a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1b4a6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b4a6-110">Permission type</span></span>      | <span data-ttu-id="1b4a6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b4a6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b4a6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b4a6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1b4a6-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b4a6-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1b4a6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b4a6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b4a6-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b4a6-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1b4a6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b4a6-116">Application</span></span> | <span data-ttu-id="1b4a6-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b4a6-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b4a6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b4a6-118">HTTP request</span></span>

<span data-ttu-id="1b4a6-119">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="1b4a6-119">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="1b4a6-120">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="1b4a6-120">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1b4a6-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1b4a6-121">Optional query parameters</span></span>
<span data-ttu-id="1b4a6-122">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1b4a6-122">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1b4a6-123">Например, с помощью параметра запроса `$filter` можно фильтровать контакты на основе домена, указанного в адресе электронной почты:</span><span class="sxs-lookup"><span data-stu-id="1b4a6-123">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="1b4a6-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b4a6-124">Request headers</span></span>
| <span data-ttu-id="1b4a6-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b4a6-125">Header</span></span>       | <span data-ttu-id="1b4a6-126">Значение</span><span class="sxs-lookup"><span data-stu-id="1b4a6-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b4a6-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b4a6-127">Authorization</span></span>  | <span data-ttu-id="1b4a6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b4a6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1b4a6-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b4a6-130">Content-Type</span></span>   | <span data-ttu-id="1b4a6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="1b4a6-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b4a6-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b4a6-132">Request body</span></span>
<span data-ttu-id="1b4a6-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b4a6-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b4a6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b4a6-134">Response</span></span>

<span data-ttu-id="1b4a6-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b4a6-135">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b4a6-136">Пример</span><span class="sxs-lookup"><span data-stu-id="1b4a6-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b4a6-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b4a6-137">Request</span></span>
<span data-ttu-id="1b4a6-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b4a6-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="1b4a6-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b4a6-139">Response</span></span>
<span data-ttu-id="1b4a6-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b4a6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
