# <a name="list-contacts"></a><span data-ttu-id="ce6ef-101">Список контактов</span><span class="sxs-lookup"><span data-stu-id="ce6ef-101">List contacts</span></span>

<span data-ttu-id="ce6ef-102">Получении коллекции контактов из папки контактов по умолчанию для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="ce6ef-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce6ef-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="ce6ef-103">Prerequisites</span></span>
<span data-ttu-id="ce6ef-104">Для применения этого API требуется одна из указанных **областей**: *Contacts.Read; Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="ce6ef-104">One of the following scopes is required to execute this API: Contacts.Read; Contacts.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="ce6ef-105">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce6ef-105">HTTP request</span></span>

<span data-ttu-id="ce6ef-106">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="ce6ef-106">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="ce6ef-107">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="ce6ef-107">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ce6ef-108">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ce6ef-108">Optional query parameters</span></span>
<span data-ttu-id="ce6ef-109">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ce6ef-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ce6ef-110">Например, с помощью параметра запроса `$filter` можно фильтровать контакты на основе домена, указанного в адресе электронной почты:</span><span class="sxs-lookup"><span data-stu-id="ce6ef-110">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="ce6ef-111">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce6ef-111">Request headers</span></span>
| <span data-ttu-id="ce6ef-112">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce6ef-112">Header</span></span>       | <span data-ttu-id="ce6ef-113">Значение</span><span class="sxs-lookup"><span data-stu-id="ce6ef-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce6ef-114">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce6ef-114">Authorization</span></span>  | <span data-ttu-id="ce6ef-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce6ef-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ce6ef-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce6ef-117">Content-Type</span></span>   | <span data-ttu-id="ce6ef-118">application/json</span><span class="sxs-lookup"><span data-stu-id="ce6ef-118">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="ce6ef-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce6ef-119">Request body</span></span>
<span data-ttu-id="ce6ef-120">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce6ef-120">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce6ef-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce6ef-121">Response</span></span>

<span data-ttu-id="ce6ef-122">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce6ef-122">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce6ef-123">Пример</span><span class="sxs-lookup"><span data-stu-id="ce6ef-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce6ef-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce6ef-124">Request</span></span>
<span data-ttu-id="ce6ef-125">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce6ef-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="ce6ef-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce6ef-126">Response</span></span>
<span data-ttu-id="ce6ef-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ce6ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
