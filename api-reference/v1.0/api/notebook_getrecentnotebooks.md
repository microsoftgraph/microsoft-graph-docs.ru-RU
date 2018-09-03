# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="516ce-101">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="516ce-101">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="516ce-102">Получите список экземпляров [recentNotebook](../resources/recentnotebook.md), которые недавно открывал вошедший в систему пользователь.</span><span class="sxs-lookup"><span data-stu-id="516ce-102">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="516ce-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="516ce-103">Permissions</span></span>
<span data-ttu-id="516ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="516ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="516ce-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="516ce-106">Permission type</span></span>      | <span data-ttu-id="516ce-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="516ce-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="516ce-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="516ce-108">Delegated (work or school account)</span></span> | <span data-ttu-id="516ce-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="516ce-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="516ce-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="516ce-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="516ce-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="516ce-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="516ce-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="516ce-112">Application</span></span> | <span data-ttu-id="516ce-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="516ce-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="516ce-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="516ce-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="516ce-115">Идентификатор `<id | userPrincipalName>` должен соответствовать пользователю, закодированному в токене авторизации, используемом для выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="516ce-115">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="516ce-116">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="516ce-116">Function parameters</span></span>

| <span data-ttu-id="516ce-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="516ce-117">Parameter</span></span>    | <span data-ttu-id="516ce-118">Тип</span><span class="sxs-lookup"><span data-stu-id="516ce-118">Type</span></span>   |<span data-ttu-id="516ce-119">Описание</span><span class="sxs-lookup"><span data-stu-id="516ce-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="516ce-120">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="516ce-120">includePersonalNotebooks</span></span>|<span data-ttu-id="516ce-121">Логический</span><span class="sxs-lookup"><span data-stu-id="516ce-121">Boolean</span></span>|<span data-ttu-id="516ce-122">Включите записные книжки, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="516ce-122">Include notebooks owned by the user.</span></span> <span data-ttu-id="516ce-123">Установите значение `true`, чтобы включить записные книжки, принадлежащие пользователю; в противном случае установите значение `false`.</span><span class="sxs-lookup"><span data-stu-id="516ce-123">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="516ce-124">Если вы не включите параметр `includePersonalNotebooks`, запрос вернет ошибку `400`.</span><span class="sxs-lookup"><span data-stu-id="516ce-124">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="516ce-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="516ce-125">Request headers</span></span>
| <span data-ttu-id="516ce-126">Имя</span><span class="sxs-lookup"><span data-stu-id="516ce-126">Name</span></span>       | <span data-ttu-id="516ce-127">Описание</span><span class="sxs-lookup"><span data-stu-id="516ce-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="516ce-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="516ce-128">Authorization</span></span>  | <span data-ttu-id="516ce-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="516ce-129">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="516ce-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="516ce-130">Request body</span></span>
<span data-ttu-id="516ce-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="516ce-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="516ce-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="516ce-132">Response</span></span>
<span data-ttu-id="516ce-133">В случае успеха возвращается ответ с кодом `200 OK`, который содержит JSON-коллекцию ресурсов **recentNotebook**.</span><span class="sxs-lookup"><span data-stu-id="516ce-133">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="516ce-134">Пример</span><span class="sxs-lookup"><span data-stu-id="516ce-134">Example</span></span>
<span data-ttu-id="516ce-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="516ce-135">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="516ce-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="516ce-136">Request</span></span>
<span data-ttu-id="516ce-137">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="516ce-137">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="516ce-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="516ce-138">Response</span></span>
<span data-ttu-id="516ce-139">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="516ce-139">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.recentNotebook)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "displayName":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "displayName":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
