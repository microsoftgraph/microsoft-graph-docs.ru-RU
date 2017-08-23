# <a name="list-contacts"></a><span data-ttu-id="fca66-101">Список контактов</span><span class="sxs-lookup"><span data-stu-id="fca66-101">List contacts</span></span>

<span data-ttu-id="fca66-102">Получение коллекции контактов из папки контактов по умолчанию для вошедшего пользователя (`.../me/contacts`) или из указанной папки контактов.</span><span class="sxs-lookup"><span data-stu-id="fca66-102">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="fca66-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fca66-103">Permissions</span></span>
<span data-ttu-id="fca66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fca66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fca66-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fca66-106">Permission type</span></span>      | <span data-ttu-id="fca66-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fca66-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="fca66-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fca66-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fca66-109">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fca66-109">Contacts.Read, Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="fca66-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fca66-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fca66-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fca66-111">Contacts.Read, Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="fca66-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fca66-112">Application</span></span> | <span data-ttu-id="fca66-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fca66-113">Contacts.Read, Contacts.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fca66-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fca66-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fca66-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fca66-115">Optional query parameters</span></span>
<span data-ttu-id="fca66-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fca66-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fca66-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fca66-117">Request headers</span></span>
| <span data-ttu-id="fca66-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fca66-118">Name</span></span>       | <span data-ttu-id="fca66-119">Тип</span><span class="sxs-lookup"><span data-stu-id="fca66-119">Type</span></span> | <span data-ttu-id="fca66-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fca66-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fca66-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fca66-121">Authorization</span></span>  | <span data-ttu-id="fca66-122">string</span><span class="sxs-lookup"><span data-stu-id="fca66-122">string</span></span>  | <span data-ttu-id="fca66-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fca66-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fca66-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fca66-125">Request body</span></span>
<span data-ttu-id="fca66-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fca66-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fca66-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fca66-127">Response</span></span>

<span data-ttu-id="fca66-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fca66-128">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fca66-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fca66-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fca66-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fca66-130">Request</span></span>
<span data-ttu-id="fca66-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fca66-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="fca66-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="fca66-132">Response</span></span>
<span data-ttu-id="fca66-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fca66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
