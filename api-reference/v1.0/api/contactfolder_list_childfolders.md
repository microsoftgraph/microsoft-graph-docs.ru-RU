# <a name="list-childfolders"></a><span data-ttu-id="b042a-101">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="b042a-101">List childFolders</span></span>

<span data-ttu-id="b042a-102">Получение коллекции дочерних папок в указанной папке контактов.</span><span class="sxs-lookup"><span data-stu-id="b042a-102">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="b042a-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b042a-103">Permissions</span></span>
<span data-ttu-id="b042a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b042a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b042a-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b042a-106">Permission type</span></span>      | <span data-ttu-id="b042a-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b042a-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b042a-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b042a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b042a-109">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b042a-109">Contacts.Read, Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="b042a-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b042a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b042a-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b042a-111">Contacts.Read, Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="b042a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b042a-112">Application</span></span> | <span data-ttu-id="b042a-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b042a-113">Contacts.Read, Contacts.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b042a-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b042a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b042a-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b042a-115">Optional query parameters</span></span>
<span data-ttu-id="b042a-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b042a-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b042a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b042a-117">Request headers</span></span>
| <span data-ttu-id="b042a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b042a-118">Name</span></span>       | <span data-ttu-id="b042a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b042a-119">Type</span></span> | <span data-ttu-id="b042a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b042a-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b042a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b042a-121">Authorization</span></span>  | <span data-ttu-id="b042a-122">string</span><span class="sxs-lookup"><span data-stu-id="b042a-122">string</span></span>  | <span data-ttu-id="b042a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b042a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b042a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b042a-125">Request body</span></span>
<span data-ttu-id="b042a-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b042a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b042a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b042a-127">Response</span></span>

<span data-ttu-id="b042a-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b042a-128">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b042a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b042a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b042a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b042a-130">Request</span></span>
<span data-ttu-id="b042a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b042a-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="b042a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="b042a-132">Response</span></span>
<span data-ttu-id="b042a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b042a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
