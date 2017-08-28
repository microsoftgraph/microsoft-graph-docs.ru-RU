# <a name="list-contacts"></a><span data-ttu-id="10300-101">Список контактов</span><span class="sxs-lookup"><span data-stu-id="10300-101">List contacts</span></span>

<span data-ttu-id="10300-102">Получение коллекции контактов из папки контактов по умолчанию для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="10300-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="10300-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10300-103">Permissions</span></span>
<span data-ttu-id="10300-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="10300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="10300-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10300-106">Permission type</span></span>      | <span data-ttu-id="10300-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10300-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10300-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10300-108">Delegated (work or school account)</span></span> | <span data-ttu-id="10300-109">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10300-109">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="10300-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10300-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10300-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10300-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="10300-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10300-112">Application</span></span> | <span data-ttu-id="10300-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10300-113">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="10300-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10300-114">HTTP request</span></span>

<span data-ttu-id="10300-115">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="10300-115">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="10300-116">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="10300-116">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10300-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10300-117">Optional query parameters</span></span>
<span data-ttu-id="10300-118">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="10300-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="10300-119">Например, с помощью параметра запроса `$filter` можно фильтровать контакты на основе домена, указанного в адресе электронной почты:</span><span class="sxs-lookup"><span data-stu-id="10300-119">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="10300-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10300-120">Request headers</span></span>
| <span data-ttu-id="10300-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10300-121">Header</span></span>       | <span data-ttu-id="10300-122">Значение</span><span class="sxs-lookup"><span data-stu-id="10300-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="10300-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10300-123">Authorization</span></span>  | <span data-ttu-id="10300-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10300-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="10300-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10300-126">Content-Type</span></span>   | <span data-ttu-id="10300-127">application/json</span><span class="sxs-lookup"><span data-stu-id="10300-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="10300-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10300-128">Request body</span></span>
<span data-ttu-id="10300-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10300-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10300-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="10300-130">Response</span></span>

<span data-ttu-id="10300-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10300-131">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10300-132">Пример</span><span class="sxs-lookup"><span data-stu-id="10300-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10300-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="10300-133">Request</span></span>
<span data-ttu-id="10300-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10300-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="10300-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="10300-135">Response</span></span>
<span data-ttu-id="10300-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="10300-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
