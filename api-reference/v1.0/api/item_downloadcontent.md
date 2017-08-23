# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="0128f-101">Загрузка содержимого ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="0128f-101">Download the contents of a DriveItem</span></span>

<span data-ttu-id="0128f-p101">Загрузка содержимого для ресурса driveItem. Можно скачать только ресурс driveItem со свойством **file**.</span><span class="sxs-lookup"><span data-stu-id="0128f-p101">Download the contents for a driveItem. Only driveItem with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="0128f-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0128f-104">Permissions</span></span>
<span data-ttu-id="0128f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0128f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0128f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0128f-107">Permission type</span></span>      | <span data-ttu-id="0128f-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0128f-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="0128f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0128f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="0128f-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0128f-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="0128f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0128f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0128f-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0128f-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="0128f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0128f-113">Application</span></span> | <span data-ttu-id="0128f-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0128f-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0128f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0128f-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /drives/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
```

## <a name="request-headers"></a><span data-ttu-id="0128f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0128f-116">Request headers</span></span>

| <span data-ttu-id="0128f-117">Имя</span><span class="sxs-lookup"><span data-stu-id="0128f-117">Name</span></span>          | <span data-ttu-id="0128f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="0128f-118">Value</span></span>  | <span data-ttu-id="0128f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0128f-119">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0128f-120">if-none-match</span><span class="sxs-lookup"><span data-stu-id="0128f-120">if-none-match</span></span> | <span data-ttu-id="0128f-121">String</span><span class="sxs-lookup"><span data-stu-id="0128f-121">String</span></span> | <span data-ttu-id="0128f-122">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то возвращается отклик `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="0128f-122">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0128f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0128f-123">Request body</span></span>
<span data-ttu-id="0128f-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0128f-124">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="0128f-125">Пример</span><span class="sxs-lookup"><span data-stu-id="0128f-125">Example</span></span>
<span data-ttu-id="0128f-126">Ниже приведен пример, в котором показано, как вызвать этот API.</span><span class="sxs-lookup"><span data-stu-id="0128f-126">Here is an example of how to call this API.</span></span>


<!-- { "blockType": "request", "name": "driveitem-download-contents" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/content
```

##### <a name="response"></a><span data-ttu-id="0128f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0128f-127">Response</span></span>
<span data-ttu-id="0128f-p103">Возвращает отклик `302 Found`, перенаправляя к URL-адресу загрузки файла, прошедшему предварительную проверку подлинности. Это такой же URL-адрес, доступный с помощью свойства `@microsoft.graph.downloadUrl` в ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="0128f-p103">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="0128f-p104">Чтобы загрузить содержимое файла, приложению необходимо будет следовать заголовку `Location` в отклике. Многие библиотеки клиентов HTTP будут автоматически следовать перенаправлению 302 и немедленно начинать загрузку файла.</span><span class="sxs-lookup"><span data-stu-id="0128f-p104">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="0128f-132">URL-адреса загрузки, прошедшие предварительную проверку подлинности, действительны только на протяжении короткого периода времени (несколько минут) и не требуют заголовка `Authorization` для загрузки.</span><span class="sxs-lookup"><span data-stu-id="0128f-132">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="0128f-133">Загрузка части заданного диапазона байтов</span><span class="sxs-lookup"><span data-stu-id="0128f-133">Partial range downloads</span></span>

<span data-ttu-id="0128f-p105">Чтобы загрузить из файла часть заданного диапазона байтов, приложение может использовать заголовок `Range`, как указано в документе [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Обратите внимание, что заголовок `Range` необходимо добавлять в фактический URL-адрес `@microsoft.graph.downloadUrl`, а не в запрос для `/content`.</span><span class="sxs-lookup"><span data-stu-id="0128f-p105">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "name": "driveitem-get-partial-content" } -->
```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="0128f-p106">Это позволит вернуть отклик `HTTP 206 Partial Content` с запрашиваемым диапазоном байтов из файла. Если не удается создать диапазон, можно проигнорировать заголовок диапазона, после чего отклик `HTTP 200` возвращается с полным содержимым файла.</span><span class="sxs-lookup"><span data-stu-id="0128f-p106">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->
```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048

<first 1024 bytes of file>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Download item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Download file"
}-->
