# <a name="search-for-a-driveitem-within-a-drive"></a><span data-ttu-id="5eea5-101">Поиск элемента DriveItem на диске</span><span class="sxs-lookup"><span data-stu-id="5eea5-101">Search for a DriveItem within a drive</span></span>

<span data-ttu-id="5eea5-p101">Поиск элементов, соответствующих запросу, в иерархии элементов. Вы можете выполнить поиск в иерархии папок, на всем диске или среди файлов, к которым текущему пользователю предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="5eea5-p101">Search the hierarchy of items for items matching a query. You can search within a folder hierarhcy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eea5-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5eea5-104">Permissions</span></span>
<span data-ttu-id="5eea5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5eea5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5eea5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5eea5-107">Permission type</span></span>      | <span data-ttu-id="5eea5-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5eea5-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="5eea5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5eea5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5eea5-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eea5-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="5eea5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5eea5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eea5-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eea5-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="5eea5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5eea5-113">Application</span></span> | <span data-ttu-id="5eea5-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eea5-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5eea5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5eea5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```
GET /me/drive/root/search(q='{search-text}')
GET /me/drive/items/{item-id}/search(q='{search-text}')
GET /me/drive/root:/{item-path}:/search(q='{search-text}')
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5eea5-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5eea5-116">Optional query parameters</span></span>
<span data-ttu-id="5eea5-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5eea5-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="5eea5-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5eea5-118">Request body</span></span>
<span data-ttu-id="5eea5-119">Не указывайте основной текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5eea5-119">Do not supply a request body for this method.</span></span>

#### <a name="function-parameters"></a><span data-ttu-id="5eea5-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5eea5-120">Function parameters</span></span>

| <span data-ttu-id="5eea5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5eea5-121">Name</span></span> | <span data-ttu-id="5eea5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5eea5-122">Value</span></span>  | <span data-ttu-id="5eea5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5eea5-123">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| `q`  | <span data-ttu-id="5eea5-124">string</span><span class="sxs-lookup"><span data-stu-id="5eea5-124">string</span></span> | <span data-ttu-id="5eea5-p103">Текст запроса, используемый для поиска элементов. Для поиска можно использовать несколько полей, включая поля имени файла, метаданных и содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="5eea5-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="5eea5-127">Пример</span><span class="sxs-lookup"><span data-stu-id="5eea5-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5eea5-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="5eea5-128">Request</span></span>

<span data-ttu-id="5eea5-129">Вот пример запроса, выполняющего поиск в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="5eea5-129">Here is an example of the request searching the current user's OneDrive</span></span>
<!-- {
  "blockType": "request",
  "name": "item_search"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/search(q='{search-query}')
```

##### <a name="response"></a><span data-ttu-id="5eea5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eea5-130">Response</span></span>
<span data-ttu-id="5eea5-p104">Этот метод возвращает объект, который содержит коллекцию элементов [DriveItem](../resources/driveitem.md), соответствующих условиям поиска. Если не будет найдено ни одного элемента, то будет возвращена пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="5eea5-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="5eea5-p105">Если будет найдено слишком много совпадений, отклик будет разбит на страницы, а свойство **@odata.nextLink** будет содержать URL-адрес на следующую страницу с результатами. Чтобы указать количество элементов на странице, вы можете использовать параметр запроса `$top`.</span><span class="sxs-lookup"><span data-stu-id="5eea5-p105">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="5eea5-135">Поиск элементов, к которым пользователь может получить доступ</span><span class="sxs-lookup"><span data-stu-id="5eea5-135">Searching for items a user can access</span></span>

<span data-ttu-id="5eea5-p106">Помимо поиска элементов на диске ваше приложение может выполнять более широкий поиск и включать элементы, к которым текущему пользователю предоставлен доступ. Чтобы расширить область поиска, используйте метод **search** в ресурсе [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="5eea5-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

##### <a name="request"></a><span data-ttu-id="5eea5-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5eea5-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "item_search_all"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/search(q='{search-query}')
```

##### <a name="response"></a><span data-ttu-id="5eea5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eea5-139">Response</span></span>
<span data-ttu-id="5eea5-p107">Отклики при поиске на ресурсе **Drive** могут включать элементы, расположенные за пределами диска (элементы, к которым текущему пользователю предоставлен доступ). Эти элементы будут содержать аспект [**remoteItem**](../resources/remoteitem.md), который указывает, что они хранятся не на целевом диске.</span><span class="sxs-lookup"><span data-stu-id="5eea5-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "driveId": "s!1020101jlkjl12lx" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```




<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: search",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Items/Search items"
}-->
