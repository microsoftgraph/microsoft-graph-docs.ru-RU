# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="45c5c-101">Список эскизов для ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="45c5c-101">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="45c5c-102">Получение коллекции ресурсов [ThumbnailSet](../resources/thumbnailset.md) для ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="45c5c-102">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="45c5c-p101">Ресурс DriveItem представляют ресурсы [ThumbnailSet](../resources/thumbnailset.md), количество которых может быть нуль и более. Каждый ресурс **thumbnailSet** может включать один или несколько объектов [**thumbnail**](../resources/thumbnail.md) — изображений, представляющих элемент. К примеру, ресурс **thumbnailSet** может включать такие распространенные объекты **thumbnail**, как `small`, `medium` и `large`.</span><span class="sxs-lookup"><span data-stu-id="45c5c-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="45c5c-p102">Работать с эскизами в OneDrive можно множеством способов. Ниже представлены наиболее распространенные из них.</span><span class="sxs-lookup"><span data-stu-id="45c5c-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="45c5c-108">Перечисление доступных эскизов элемента</span><span class="sxs-lookup"><span data-stu-id="45c5c-108">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="45c5c-109">Получение одного эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="45c5c-109">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="45c5c-110">Получение содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="45c5c-110">Retrieve thumbnail content</span></span>
* <span data-ttu-id="45c5c-111">Получение эскизов нескольких элементов в одном запросе</span><span class="sxs-lookup"><span data-stu-id="45c5c-111">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="45c5c-112">Получение эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="45c5c-112">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="45c5c-113">Отправка пользовательского эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="45c5c-113">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="45c5c-114">Определение того, существует ли отправленный пользовательский эскиз</span><span class="sxs-lookup"><span data-stu-id="45c5c-114">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="45c5c-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45c5c-115">Permissions</span></span>
<span data-ttu-id="45c5c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="45c5c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="45c5c-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45c5c-118">Permission type</span></span>      | <span data-ttu-id="45c5c-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45c5c-119">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="45c5c-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45c5c-120">Delegated (work or school account)</span></span> | <span data-ttu-id="45c5c-121">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c5c-121">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="45c5c-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45c5c-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45c5c-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c5c-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="45c5c-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45c5c-124">Application</span></span> | <span data-ttu-id="45c5c-125">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c5c-125">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="45c5c-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45c5c-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45c5c-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="45c5c-127">Optional query parameters</span></span>
<span data-ttu-id="45c5c-128">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="45c5c-128">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="45c5c-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45c5c-129">Request body</span></span>
<span data-ttu-id="45c5c-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45c5c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45c5c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="45c5c-131">Response</span></span>

<span data-ttu-id="45c5c-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ThumbnailSet](../resources/thumbnailset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="45c5c-132">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45c5c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="45c5c-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="45c5c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="45c5c-134">Request</span></span>

<span data-ttu-id="45c5c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45c5c-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a><span data-ttu-id="45c5c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="45c5c-136">Response</span></span>
<span data-ttu-id="45c5c-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="45c5c-137">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0",
      "small": { "height": 64, "width": 96, "url": "https://sn3302files..."},
      "medium": { "height": 117, "width": 176, "url": "https://sn3302files..."},
      "large": { "height": 533, "width": 800, "url": "https://sn3302files..."}
    }
  ]
}
```

## <a name="retrieve-a-single-thumbnail"></a><span data-ttu-id="45c5c-138">Получение одного эскиза</span><span class="sxs-lookup"><span data-stu-id="45c5c-138">Retrieve a single thumbnail</span></span>

<span data-ttu-id="45c5c-139">Получение метаданных для одного эскиза и размера с помощью прямого запроса.</span><span class="sxs-lookup"><span data-stu-id="45c5c-139">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

## <a name="http-request"></a><span data-ttu-id="45c5c-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45c5c-140">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="45c5c-141">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="45c5c-141">Path parameters</span></span>

| <span data-ttu-id="45c5c-142">Имя</span><span class="sxs-lookup"><span data-stu-id="45c5c-142">Name</span></span>         | <span data-ttu-id="45c5c-143">Тип</span><span class="sxs-lookup"><span data-stu-id="45c5c-143">Type</span></span>   | <span data-ttu-id="45c5c-144">Описание</span><span class="sxs-lookup"><span data-stu-id="45c5c-144">Description</span></span>                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="45c5c-145">**item-id**</span><span class="sxs-lookup"><span data-stu-id="45c5c-145">**item-id**</span></span>  | <span data-ttu-id="45c5c-146">string</span><span class="sxs-lookup"><span data-stu-id="45c5c-146">string</span></span> | <span data-ttu-id="45c5c-147">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="45c5c-147">The unique identifier for the item referenced.</span></span>                                      |
| <span data-ttu-id="45c5c-148">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="45c5c-148">**thumb-id**</span></span> | <span data-ttu-id="45c5c-149">number</span><span class="sxs-lookup"><span data-stu-id="45c5c-149">number</span></span> | <span data-ttu-id="45c5c-150">Индекс эскиза (как правило, 0–4).</span><span class="sxs-lookup"><span data-stu-id="45c5c-150">The index of the thumbnail, usually 0-4.</span></span>                                            |
| <span data-ttu-id="45c5c-151">**size**</span><span class="sxs-lookup"><span data-stu-id="45c5c-151">**size**</span></span>     | <span data-ttu-id="45c5c-152">string</span><span class="sxs-lookup"><span data-stu-id="45c5c-152">string</span></span> | <span data-ttu-id="45c5c-p104">Размер запрашиваемого эскиза. Это должен быть один из указанных стандартных размеров.</span><span class="sxs-lookup"><span data-stu-id="45c5c-p104">The size of the thumbnail requested. This must be one of the standard sizes listed.</span></span> |


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "http://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-content"></a><span data-ttu-id="45c5c-155">Получение содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="45c5c-155">Retrieve thumbnail content</span></span>

<span data-ttu-id="45c5c-156">Вы можете получить содержимое эскиза напрямую, запросив свойство **content** этого эскиза.</span><span class="sxs-lookup"><span data-stu-id="45c5c-156">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

## <a name="http-request"></a><span data-ttu-id="45c5c-157">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45c5c-157">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a><span data-ttu-id="45c5c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="45c5c-158">Response</span></span>

<span data-ttu-id="45c5c-159">В ответ служба перенаправляет на URL-адрес эскиза.</span><span class="sxs-lookup"><span data-stu-id="45c5c-159">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="45c5c-p105">Для URL-адресов содержимого эскизов выполняется предварительная проверка подлинности, поэтому они не требуют скачивания заголовка авторизации. Эти URL-адреса действительны в течение нескольких часов, поэтому их не следует кэшировать в приложениях.</span><span class="sxs-lookup"><span data-stu-id="45c5c-p105">Thumbnail content URLs are pre-authenticated and do not require an authorization header to be downloaded. These URLs are short lived and only valid for a few hours and should not be cached by apps.</span></span>


## <a name="size-values"></a><span data-ttu-id="45c5c-162">Значения размера</span><span class="sxs-lookup"><span data-stu-id="45c5c-162">Size values</span></span>

<span data-ttu-id="45c5c-p106">В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.</span><span class="sxs-lookup"><span data-stu-id="45c5c-p106">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="45c5c-165">Имя</span><span class="sxs-lookup"><span data-stu-id="45c5c-165">Name</span></span>           | <span data-ttu-id="45c5c-166">Разрешение</span><span class="sxs-lookup"><span data-stu-id="45c5c-166">Resolution</span></span>  | <span data-ttu-id="45c5c-167">Пропорции</span><span class="sxs-lookup"><span data-stu-id="45c5c-167">Aspect Ratio</span></span> | <span data-ttu-id="45c5c-168">Описание</span><span class="sxs-lookup"><span data-stu-id="45c5c-168">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="45c5c-169">96 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="45c5c-169">96 longest</span></span>  | <span data-ttu-id="45c5c-170">Исходные</span><span class="sxs-lookup"><span data-stu-id="45c5c-170">Original</span></span>     | <span data-ttu-id="45c5c-171">Небольшой эскиз с сильным сжатием, обрезанный до квадрата.</span><span class="sxs-lookup"><span data-stu-id="45c5c-171">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="45c5c-172">176 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="45c5c-172">176 longest</span></span> | <span data-ttu-id="45c5c-173">Исходные</span><span class="sxs-lookup"><span data-stu-id="45c5c-173">Original</span></span>     | <span data-ttu-id="45c5c-174">Обрезан до стандартного размера элемента для веб-представления OneDrive.</span><span class="sxs-lookup"><span data-stu-id="45c5c-174">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="45c5c-175">800 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="45c5c-175">800 longest</span></span> | <span data-ttu-id="45c5c-176">Исходные</span><span class="sxs-lookup"><span data-stu-id="45c5c-176">Original</span></span>     | <span data-ttu-id="45c5c-177">Эскиз, длина большей стороны которого изменена на 800 пикселей.</span><span class="sxs-lookup"><span data-stu-id="45c5c-177">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <a name="remarks"></a><span data-ttu-id="45c5c-178">Заметки</span><span class="sxs-lookup"><span data-stu-id="45c5c-178">Remarks</span></span>

<span data-ttu-id="45c5c-179">**Примечание.** В OneDrive для бизнеса и SharePoint:</span><span class="sxs-lookup"><span data-stu-id="45c5c-179">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="45c5c-180">С помощью таких вызовов невозможно дополнить коллекцию эскизов: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`.</span><span class="sxs-lookup"><span data-stu-id="45c5c-180">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
