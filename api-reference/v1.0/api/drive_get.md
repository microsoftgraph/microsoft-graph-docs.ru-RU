<span data-ttu-id="5992a-p101">Получение свойств и отношений ресурса [Drive](../resources/drive.md). Drive — это контейнер верхнего уровня для файловой системы. API Graph позволяет получить доступ к ресурсу Drive для OneDrive, OneDrive для бизнеса и библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5992a-p101">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource. A Drive is the top-level container for a file system. Graph API allows access to the Drive resource for a user's OneDrive or OneDrive for Business, or SharePoint document libraries.</span></span>

Получение свойств и отношений ресурса [Drive](../resources/drive.md). Drive — это контейнер верхнего уровня для файловой системы. API Graph позволяет получить доступ к ресурсу Drive для OneDrive, OneDrive для бизнеса и библиотек документов SharePoint.

## <span data-ttu-id="5992a-105">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="5992a-105">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>

<span data-ttu-id="5992a-106">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="5992a-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="5992a-107">Files.Read</span><span class="sxs-lookup"><span data-stu-id="5992a-107">Files.Read</span></span>
* <span data-ttu-id="5992a-108">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="5992a-108">Files.ReadWrite</span></span>
* <span data-ttu-id="5992a-109">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="5992a-109">Files.Read.All</span></span>
* <span data-ttu-id="5992a-110">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5992a-110">Files.ReadWrite.All</span></span>
* <span data-ttu-id="5992a-111">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="5992a-111">Sites.Read.All</span></span>
* <span data-ttu-id="5992a-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5992a-112">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="5992a-113">Получение доступа к OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="5992a-113">Get a user's OneDrive</span></span>
<a id="get-a-users-onedrive" class="xliff"></a>

<span data-ttu-id="5992a-114">Чтобы получить доступ к хранилищу пользователя OneDrive или OneDrive для бизнеса, ваше приложение должно запросить отношение **drive** для ресурса [User](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="5992a-114">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the [User](../resources/user.md) resource.</span></span>

### <span data-ttu-id="5992a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5992a-115">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <span data-ttu-id="5992a-116">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="5992a-116">Get the document library associated with a group</span></span>
<a id="get-the-document-library-associated-with-a-group" class="xliff"></a>

<span data-ttu-id="5992a-117">Для доступа к библиотеке документов [группы](../resources/group.md) по умолчанию приложение запрашивает отношение **drive** для объекта Group.</span><span class="sxs-lookup"><span data-stu-id="5992a-117">To access a [Group's](../resources/group.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

### <span data-ttu-id="5992a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5992a-118">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <span data-ttu-id="5992a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5992a-119">Optional query parameters</span></span>
<a id="optional-query-parameters" class="xliff"></a>

<span data-ttu-id="5992a-120">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5992a-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <span data-ttu-id="5992a-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5992a-121">Request body</span></span>
<a id="request-body" class="xliff"></a>

<span data-ttu-id="5992a-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5992a-122">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="5992a-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="5992a-123">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="5992a-124">В случае успеха этот метод возвращает код ответа `200 OK` и ресурс [Drive](../resources/drive.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5992a-124">If successful, this method returns a `200 OK` response code and [Drive](../resources/drive.md) resource in the response body.</span></span>

## <span data-ttu-id="5992a-125">Пример</span><span class="sxs-lookup"><span data-stu-id="5992a-125">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="5992a-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="5992a-126">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="5992a-127">Ниже приведен пример запроса для получения сведений о хранилище OneDrive для бизнеса или OneDrive пользователя после входа.</span><span class="sxs-lookup"><span data-stu-id="5992a-127">Here is an example of the request to get the sign-in user's OneDrive or OneDrive for Business.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <span data-ttu-id="5992a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5992a-128">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="5992a-129">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5992a-129">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",    
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get Drive"
}-->
