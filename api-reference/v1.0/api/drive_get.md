<span data-ttu-id="b7aad-p101">Получение свойств и отношений ресурса [Drive](../resources/drive.md). Drive — это контейнер верхнего уровня для файловой системы. API Graph позволяет получить доступ к ресурсу Drive для OneDrive, OneDrive для бизнеса и библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b7aad-p101">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource. A Drive is the top-level container for a file system. Graph API allows access to the Drive resource for a user's OneDrive or OneDrive for Business, or SharePoint document libraries.</span></span>

Получение свойств и отношений ресурса [Drive](../resources/drive.md). Drive — это контейнер верхнего уровня для файловой системы. API Graph позволяет получить доступ к ресурсу Drive для OneDrive, OneDrive для бизнеса и библиотек документов SharePoint.

## <a name="prerequisites"></a><span data-ttu-id="b7aad-105">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="b7aad-105">Prerequisites</span></span>

<span data-ttu-id="b7aad-106">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="b7aad-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="b7aad-107">Files.Read</span><span class="sxs-lookup"><span data-stu-id="b7aad-107">Files.Read</span></span>
* <span data-ttu-id="b7aad-108">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="b7aad-108">Files.ReadWrite</span></span>
* <span data-ttu-id="b7aad-109">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7aad-109">Files.Read.All</span></span>
* <span data-ttu-id="b7aad-110">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7aad-110">Files.ReadWrite.All</span></span>
* <span data-ttu-id="b7aad-111">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7aad-111">Sites.Read.All</span></span>
* <span data-ttu-id="b7aad-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7aad-112">Sites.ReadWrite.All</span></span>

## <a name="get-a-users-onedrive"></a><span data-ttu-id="b7aad-113">Получение доступа к OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="b7aad-113">Get a user's OneDrive</span></span>

<span data-ttu-id="b7aad-114">Чтобы получить доступ к хранилищу пользователя OneDrive или OneDrive для бизнеса, ваше приложение должно запросить отношение **drive** для ресурса [User](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="b7aad-114">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the [User](../resources/user.md) resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="b7aad-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7aad-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="b7aad-116">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="b7aad-116">Get the document library associated with a group</span></span>

<span data-ttu-id="b7aad-117">Для доступа к библиотеке документов [группы](../resources/group.md) по умолчанию приложение запрашивает отношение **drive** для объекта Group.</span><span class="sxs-lookup"><span data-stu-id="b7aad-117">To access a [Group's](../resources/group.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

## <a name="http-request"></a><span data-ttu-id="b7aad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7aad-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <a name="optional-query-parameters"></a><span data-ttu-id="b7aad-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7aad-119">Optional query parameters</span></span>

<span data-ttu-id="b7aad-120">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b7aad-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="b7aad-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7aad-121">Request body</span></span>

<span data-ttu-id="b7aad-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7aad-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7aad-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7aad-123">Response</span></span>

<span data-ttu-id="b7aad-124">В случае успеха этот метод возвращает код ответа `200 OK` и ресурс [Drive](../resources/drive.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b7aad-124">If successful, this method returns a `200 OK` response code and [Drive](../resources/drive.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7aad-125">Пример</span><span class="sxs-lookup"><span data-stu-id="b7aad-125">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b7aad-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7aad-126">Request</span></span>

<span data-ttu-id="b7aad-127">Ниже приведен пример запроса для получения сведений о хранилище OneDrive для бизнеса или OneDrive пользователя после входа.</span><span class="sxs-lookup"><span data-stu-id="b7aad-127">Here is an example of the request to get the sign-in user's OneDrive or OneDrive for Business.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <a name="response"></a><span data-ttu-id="b7aad-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7aad-128">Response</span></span>

<span data-ttu-id="b7aad-129">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b7aad-129">Here is an example of the response.</span></span>

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
