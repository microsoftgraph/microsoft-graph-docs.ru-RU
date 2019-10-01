---
author: JeremyKelley
description: Получение коллекции ресурсов ThumbnailSet для ресурса DriveItem.
ms.date: 09/10/2017
title: Получение эскизов файла или папки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2bed97e65a57c4a7d46336e9dcd845780e9e8d30
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333229"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="71a07-103">Список эскизов для ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="71a07-103">List thumbnails for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71a07-104">Получение коллекции ресурсов [ThumbnailSet](../resources/thumbnailset.md) для ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="71a07-104">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="71a07-p101">Ресурс DriveItem представляют ресурсы [ThumbnailSet](../resources/thumbnailset.md), количество которых может быть нуль и более. Каждый ресурс **thumbnailSet** может включать один или несколько объектов [**thumbnail**](../resources/thumbnail.md) — изображений, представляющих элемент. К примеру, ресурс **thumbnailSet** может включать такие распространенные объекты **thumbnail**, как `small`, `medium` и `large`.</span><span class="sxs-lookup"><span data-stu-id="71a07-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="71a07-p102">Работать с эскизами в OneDrive можно множеством способов. Ниже представлены наиболее распространенные из них.</span><span class="sxs-lookup"><span data-stu-id="71a07-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="71a07-110">Перечисление доступных эскизов элемента</span><span class="sxs-lookup"><span data-stu-id="71a07-110">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="71a07-111">Получение одного эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="71a07-111">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="71a07-112">Получение содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="71a07-112">Retrieve thumbnail content</span></span>
* <span data-ttu-id="71a07-113">Получение эскизов нескольких элементов в одном запросе</span><span class="sxs-lookup"><span data-stu-id="71a07-113">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="71a07-114">Получение эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="71a07-114">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="71a07-115">Отправка пользовательского эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="71a07-115">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="71a07-116">Определение того, существует ли отправленный пользовательский эскиз</span><span class="sxs-lookup"><span data-stu-id="71a07-116">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="71a07-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71a07-117">Permissions</span></span>

<span data-ttu-id="71a07-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71a07-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71a07-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71a07-120">Permission type</span></span>      | <span data-ttu-id="71a07-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71a07-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71a07-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71a07-122">Delegated (work or school account)</span></span> | <span data-ttu-id="71a07-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71a07-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="71a07-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71a07-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71a07-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71a07-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="71a07-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71a07-126">Application</span></span> | <span data-ttu-id="71a07-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71a07-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71a07-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71a07-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71a07-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71a07-129">Optional query parameters</span></span>

<span data-ttu-id="71a07-130">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="71a07-130">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="71a07-131">Кроме того, этот метод поддерживает получение эскиза с исходным значением EXIF и без примененного вращения путем добавления параметра `originalOrientation=true` запроса.</span><span class="sxs-lookup"><span data-stu-id="71a07-131">Additionally, this method supports retrieving the thumbnail with the original orientation EXIF value and without the applied rotation by appending the `originalOrientation=true` query parameter.</span></span>
<span data-ttu-id="71a07-132">В настоящее время поддерживается только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="71a07-132">This is currently only supported on OneDrive Personal.</span></span>

## <a name="response"></a><span data-ttu-id="71a07-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="71a07-133">Response</span></span>

<span data-ttu-id="71a07-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ThumbnailSet](../resources/thumbnailset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71a07-134">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71a07-135">Пример</span><span class="sxs-lookup"><span data-stu-id="71a07-135">Example</span></span>

<span data-ttu-id="71a07-136">Ниже представлен пример запроса на получение доступных эскизов элемента в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="71a07-136">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="71a07-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="71a07-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71a07-138">C#</span><span class="sxs-lookup"><span data-stu-id="71a07-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71a07-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71a07-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71a07-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71a07-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="71a07-141">Этот запрос возвращает массив доступных объектов **thumbnailSet** для элемента.</span><span class="sxs-lookup"><span data-stu-id="71a07-141">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="71a07-142">У любого элемента в объекте drive может быть один или несколько эскизов (либо ни одного эскиза).</span><span class="sxs-lookup"><span data-stu-id="71a07-142">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="71a07-p106">**Примечание.** С помощью параметра _select_ строки запроса вы можете указывать размеры эскизов, возвращаемых в объекте **ThumbnailSet**. Например, запрос `/thumbnails?select=medium` получает только эскизы среднего размера.</span><span class="sxs-lookup"><span data-stu-id="71a07-p106">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="71a07-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="71a07-145">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="71a07-146">Получение одного эскиза</span><span class="sxs-lookup"><span data-stu-id="71a07-146">Get a single thumbnail</span></span>

<span data-ttu-id="71a07-147">Получение метаданных для одного эскиза и размера с помощью прямого запроса.</span><span class="sxs-lookup"><span data-stu-id="71a07-147">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="71a07-148">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71a07-148">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="71a07-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="71a07-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71a07-150">C#</span><span class="sxs-lookup"><span data-stu-id="71a07-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71a07-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71a07-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71a07-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71a07-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="71a07-153">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="71a07-153">Path parameters</span></span>

| <span data-ttu-id="71a07-154">Имя</span><span class="sxs-lookup"><span data-stu-id="71a07-154">Name</span></span>         | <span data-ttu-id="71a07-155">Тип</span><span class="sxs-lookup"><span data-stu-id="71a07-155">Type</span></span>   | <span data-ttu-id="71a07-156">Описание</span><span class="sxs-lookup"><span data-stu-id="71a07-156">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="71a07-157">**item-id**</span><span class="sxs-lookup"><span data-stu-id="71a07-157">**item-id**</span></span>  | <span data-ttu-id="71a07-158">string</span><span class="sxs-lookup"><span data-stu-id="71a07-158">string</span></span> | <span data-ttu-id="71a07-159">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="71a07-159">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="71a07-160">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="71a07-160">**thumb-id**</span></span> | <span data-ttu-id="71a07-161">number</span><span class="sxs-lookup"><span data-stu-id="71a07-161">number</span></span> | <span data-ttu-id="71a07-p107">Индекс эскиза (как правило, 0–4). Если присутствует пользовательский эскиз, для него задается индекс 0.</span><span class="sxs-lookup"><span data-stu-id="71a07-p107">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="71a07-164">**size**</span><span class="sxs-lookup"><span data-stu-id="71a07-164">**size**</span></span>     | <span data-ttu-id="71a07-165">string</span><span class="sxs-lookup"><span data-stu-id="71a07-165">string</span></span> | <span data-ttu-id="71a07-166">Размер запрашиваемого эскиза.</span><span class="sxs-lookup"><span data-stu-id="71a07-166">The size of the thumbnail requested.</span></span> <span data-ttu-id="71a07-167">Это должен быть один из стандартных размеров, указанных ниже, либо пользовательский размер.</span><span class="sxs-lookup"><span data-stu-id="71a07-167">This can be one of the standard sizes listed below or a custom size.</span></span> |

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "https://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="71a07-168">Получение двоичного содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="71a07-168">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="71a07-169">Вы можете получить содержимое эскиза напрямую, запросив свойство **content** этого эскиза.</span><span class="sxs-lookup"><span data-stu-id="71a07-169">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="71a07-170">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71a07-170">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="71a07-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="71a07-171">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71a07-172">C#</span><span class="sxs-lookup"><span data-stu-id="71a07-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71a07-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71a07-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71a07-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71a07-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="71a07-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="71a07-175">Response</span></span>

<span data-ttu-id="71a07-176">В ответ служба выполняет перенаправление на URL-адрес эскиза.</span><span class="sxs-lookup"><span data-stu-id="71a07-176">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="71a07-177">URL-адреса эскизов не кэшируются.</span><span class="sxs-lookup"><span data-stu-id="71a07-177">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="71a07-178">Если в результате изменения элемента потребуется создать новый эскиз, изменится его URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="71a07-178">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="71a07-179">Получение эскизов при перечислении ресурсов DriveItem</span><span class="sxs-lookup"><span data-stu-id="71a07-179">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="71a07-180">При получении списка отображаемых ресурсов DriveItem можно использовать параметр строки запроса _$expand_, чтобы также включить эскизы этих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="71a07-180">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="71a07-181">Благодаря этому приложение может получить эскизы и элементы в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="71a07-181">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="71a07-182">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71a07-182">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="71a07-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="71a07-183">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71a07-184">C#</span><span class="sxs-lookup"><span data-stu-id="71a07-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71a07-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71a07-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71a07-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71a07-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="71a07-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="71a07-187">Response</span></span>

<span data-ttu-id="71a07-188">Служба возвращает список ресурсов DriveItem и их эскизов.</span><span class="sxs-lookup"><span data-stu-id="71a07-188">The service responses with the list of DriveItems and their thumbnails.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "182331E8-2788-4932-B52A-A6550577043F",
      "name": "my photo.jpg",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    },
    {
      "id": "2D223953-A56B-4D9B-ADF3-13E7820673A2",
      "name": "presentation.pptx",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    }
  ]
}
```

## <a name="size-values"></a><span data-ttu-id="71a07-189">Значения размера</span><span class="sxs-lookup"><span data-stu-id="71a07-189">Size values</span></span>

<span data-ttu-id="71a07-p111">В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.</span><span class="sxs-lookup"><span data-stu-id="71a07-p111">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="71a07-192">Имя</span><span class="sxs-lookup"><span data-stu-id="71a07-192">Name</span></span>           | <span data-ttu-id="71a07-193">Разрешение</span><span class="sxs-lookup"><span data-stu-id="71a07-193">Resolution</span></span>  | <span data-ttu-id="71a07-194">Пропорции</span><span class="sxs-lookup"><span data-stu-id="71a07-194">Aspect Ratio</span></span> | <span data-ttu-id="71a07-195">Описание</span><span class="sxs-lookup"><span data-stu-id="71a07-195">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="71a07-196">96 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="71a07-196">96 longest</span></span>  | <span data-ttu-id="71a07-197">Исходные</span><span class="sxs-lookup"><span data-stu-id="71a07-197">Original</span></span>     | <span data-ttu-id="71a07-198">Небольшой эскиз с сильным сжатием, обрезанный до квадрата.</span><span class="sxs-lookup"><span data-stu-id="71a07-198">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="71a07-199">176 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="71a07-199">176 longest</span></span> | <span data-ttu-id="71a07-200">Исходные</span><span class="sxs-lookup"><span data-stu-id="71a07-200">Original</span></span>     | <span data-ttu-id="71a07-201">Обрезан до стандартного размера элемента для веб-представления OneDrive.</span><span class="sxs-lookup"><span data-stu-id="71a07-201">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="71a07-202">800 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="71a07-202">800 longest</span></span> | <span data-ttu-id="71a07-203">Исходные</span><span class="sxs-lookup"><span data-stu-id="71a07-203">Original</span></span>     | <span data-ttu-id="71a07-204">Эскиз, длина большей стороны которого изменена на 800 пикселей.</span><span class="sxs-lookup"><span data-stu-id="71a07-204">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="71a07-205">96x96</span><span class="sxs-lookup"><span data-stu-id="71a07-205">96x96</span></span>       | <span data-ttu-id="71a07-206">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="71a07-206">Square Crop</span></span>  | <span data-ttu-id="71a07-207">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="71a07-207">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="71a07-208">176x176</span><span class="sxs-lookup"><span data-stu-id="71a07-208">176x176</span></span>     | <span data-ttu-id="71a07-209">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="71a07-209">Square Crop</span></span>  | <span data-ttu-id="71a07-210">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="71a07-210">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="71a07-211">800x800</span><span class="sxs-lookup"><span data-stu-id="71a07-211">800x800</span></span>     | <span data-ttu-id="71a07-212">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="71a07-212">Square Crop</span></span>  | <span data-ttu-id="71a07-213">Большой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="71a07-213">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="71a07-214">Запрос эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="71a07-214">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="71a07-215">Помимо определенных размеров, приложение может запрашивать эскизы настраиваемых размеров, указав ширину и высоту с префиксом `c`.</span><span class="sxs-lookup"><span data-stu-id="71a07-215">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="71a07-216">Например, если вашему приложению нужны эскизы размером 300x400, оно может запросить размер следующим образом:</span><span class="sxs-lookup"><span data-stu-id="71a07-216">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="71a07-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="71a07-217">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request","name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71a07-218">C#</span><span class="sxs-lookup"><span data-stu-id="71a07-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71a07-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71a07-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71a07-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71a07-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="71a07-221">В ответ вы получите только эскиз выбранного размера:</span><span class="sxs-lookup"><span data-stu-id="71a07-221">Which responds with just the custom thumbnail size selected:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0",
      "c300x400_Crop": { "height": 300, "width": 400, "url": "https://sn3302files.onedrive.com/123"},
    }
  ]
}
```

<span data-ttu-id="71a07-222">Запросив размер эскиза, вы можете указать следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="71a07-222">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="71a07-223">Примеры пользовательских идентификаторов</span><span class="sxs-lookup"><span data-stu-id="71a07-223">Examples of custom identifiers</span></span>

| <span data-ttu-id="71a07-224">Идентификатор эскиза</span><span class="sxs-lookup"><span data-stu-id="71a07-224">Thumbnail identifier</span></span> | <span data-ttu-id="71a07-225">Разрешение</span><span class="sxs-lookup"><span data-stu-id="71a07-225">Resolution</span></span>             | <span data-ttu-id="71a07-226">Пропорции</span><span class="sxs-lookup"><span data-stu-id="71a07-226">Aspect ratio</span></span> | <span data-ttu-id="71a07-227">Описание</span><span class="sxs-lookup"><span data-stu-id="71a07-227">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="71a07-228">c300x400</span><span class="sxs-lookup"><span data-stu-id="71a07-228">c300x400</span></span>             | <span data-ttu-id="71a07-229">Заключен в прямоугольник размером 300x400</span><span class="sxs-lookup"><span data-stu-id="71a07-229">Bounded by 300x400 box</span></span> | <span data-ttu-id="71a07-230">Исходные</span><span class="sxs-lookup"><span data-stu-id="71a07-230">Original</span></span>     | <span data-ttu-id="71a07-231">Создается эскиз, который помещается в прямоугольник размером 300x400 пикселей с сохранением пропорций.</span><span class="sxs-lookup"><span data-stu-id="71a07-231">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="71a07-232">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="71a07-232">c300x400_Crop</span></span>        | <span data-ttu-id="71a07-233">300x400</span><span class="sxs-lookup"><span data-stu-id="71a07-233">300x400</span></span>                | <span data-ttu-id="71a07-234">Обрезанный</span><span class="sxs-lookup"><span data-stu-id="71a07-234">Cropped</span></span>      | <span data-ttu-id="71a07-p113">Создается эскиз размером 300x400. Сначала размер изображения меняется так, чтобы оно помещалось в прямоугольник размером 300x400, а затем обрезается все, что выходит за пределы прямоугольника.</span><span class="sxs-lookup"><span data-stu-id="71a07-p113">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="71a07-237">**Примечание.** Размер возвращаемого эскиза в пикселях может не полностью совпадать с запрашиваемым, но его пропорции будут соответствовать запросу.</span><span class="sxs-lookup"><span data-stu-id="71a07-237">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="71a07-238">В некоторых случаях возвращаются эскизы большего размера, если эскиз уже существует и легко масштабируется до запрашиваемого разрешения.</span><span class="sxs-lookup"><span data-stu-id="71a07-238">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="71a07-239">Замечания</span><span class="sxs-lookup"><span data-stu-id="71a07-239">Remarks</span></span>

<span data-ttu-id="71a07-240">**Примечание.** В OneDrive для бизнеса и SharePoint:</span><span class="sxs-lookup"><span data-stu-id="71a07-240">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="71a07-241">С помощью таких вызовов невозможно дополнить коллекцию эскизов:</span><span class="sxs-lookup"><span data-stu-id="71a07-241">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="71a07-242">Эскизы не поддерживаются в SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="71a07-242">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="71a07-243">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="71a07-243">Error responses</span></span>

<span data-ttu-id="71a07-244">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="71a07-244">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails",
  "suppressions": [
  ]
}
-->
