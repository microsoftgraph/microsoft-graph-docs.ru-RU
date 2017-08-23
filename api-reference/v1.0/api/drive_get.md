# <a name="get-drive"></a><span data-ttu-id="bbdce-101">Получение доступа к ресурсу Drive</span><span class="sxs-lookup"><span data-stu-id="bbdce-101">Get Drive</span></span>

<span data-ttu-id="bbdce-p101">Получение свойств и отношений ресурса [Drive](../resources/drive.md). Drive — это контейнер верхнего уровня для файловой системы. API Graph позволяет получить доступ к ресурсу Drive для OneDrive, OneDrive для бизнеса и библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bbdce-p101">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource. A Drive is the top-level container for a file system. Graph API allows access to the Drive resource for a user's OneDrive or OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbdce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbdce-105">Permissions</span></span>

<span data-ttu-id="bbdce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bbdce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bbdce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbdce-108">Permission type</span></span>      | <span data-ttu-id="bbdce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbdce-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="bbdce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbdce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bbdce-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbdce-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="bbdce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbdce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbdce-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbdce-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="bbdce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbdce-114">Application</span></span> | <span data-ttu-id="bbdce-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbdce-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="get-a-users-onedrive"></a><span data-ttu-id="bbdce-116">Получение OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="bbdce-116">Get a user's OneDrive</span></span>

<span data-ttu-id="bbdce-117">Чтобы получить доступ к хранилищу пользователя OneDrive или OneDrive для бизнеса, ваше приложение должно запросить отношение **drive** для ресурса [User](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="bbdce-117">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the [User](../resources/user.md) resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="bbdce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbdce-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="bbdce-119">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="bbdce-119">Get the document library associated with a group</span></span>

<span data-ttu-id="bbdce-120">Для доступа к библиотеке документов [группы](../resources/group.md) по умолчанию приложение запрашивает отношение **drive** для объекта Group.</span><span class="sxs-lookup"><span data-stu-id="bbdce-120">To access a [Group's](../resources/group.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

## <a name="http-request"></a><span data-ttu-id="bbdce-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbdce-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <a name="optional-query-parameters"></a><span data-ttu-id="bbdce-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bbdce-122">Optional query parameters</span></span>

<span data-ttu-id="bbdce-123">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bbdce-123">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="bbdce-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bbdce-124">Request body</span></span>

<span data-ttu-id="bbdce-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bbdce-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbdce-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="bbdce-126">Response</span></span>

<span data-ttu-id="bbdce-127">В случае успеха этот метод возвращает код ответа `200 OK` и ресурс [Drive](../resources/drive.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bbdce-127">If successful, this method returns a `200 OK` response code and [Drive](../resources/drive.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbdce-128">Пример</span><span class="sxs-lookup"><span data-stu-id="bbdce-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bbdce-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbdce-129">Request</span></span>

<span data-ttu-id="bbdce-130">Ниже приведен пример запроса для получения сведений о хранилище OneDrive для бизнеса или OneDrive пользователя после входа.</span><span class="sxs-lookup"><span data-stu-id="bbdce-130">Here is an example of the request to get the sign-in user's OneDrive or OneDrive for Business.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <a name="response"></a><span data-ttu-id="bbdce-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bbdce-131">Response</span></span>

<span data-ttu-id="bbdce-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bbdce-132">Here is an example of the response.</span></span>

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
