---
author: JeremyKelley
description: Получение коллекции ресурсов ThumbnailSet для ресурса DriveItem.
ms.date: 09/10/2017
title: Получение эскизов файла или папки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: de4c9ce69083eecc1c6b9279ca6e648d9fde68ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957089"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="687fd-103">Список эскизов для ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="687fd-103">List thumbnails for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="687fd-104">Получение коллекции ресурсов [ThumbnailSet](../resources/thumbnailset.md) для ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="687fd-104">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="687fd-p101">Ресурс DriveItem представляют ресурсы [ThumbnailSet](../resources/thumbnailset.md), количество которых может быть нуль и более. Каждый ресурс **thumbnailSet** может включать один или несколько объектов [**thumbnail**](../resources/thumbnail.md) — изображений, представляющих элемент. К примеру, ресурс **thumbnailSet** может включать такие распространенные объекты **thumbnail**, как `small`, `medium` и `large`.</span><span class="sxs-lookup"><span data-stu-id="687fd-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="687fd-p102">Работать с эскизами в OneDrive можно множеством способов. Ниже представлены наиболее распространенные из них.</span><span class="sxs-lookup"><span data-stu-id="687fd-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="687fd-110">Перечисление доступных эскизов элемента</span><span class="sxs-lookup"><span data-stu-id="687fd-110">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="687fd-111">Получение одного эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="687fd-111">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="687fd-112">Получение содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="687fd-112">Retrieve thumbnail content</span></span>
* <span data-ttu-id="687fd-113">Получение эскизов нескольких элементов в одном запросе</span><span class="sxs-lookup"><span data-stu-id="687fd-113">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="687fd-114">Получение эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="687fd-114">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="687fd-115">Отправка пользовательского эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="687fd-115">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="687fd-116">Определение того, существует ли отправленный пользовательский эскиз</span><span class="sxs-lookup"><span data-stu-id="687fd-116">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="687fd-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="687fd-117">Permissions</span></span>

<span data-ttu-id="687fd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="687fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="687fd-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="687fd-120">Permission type</span></span>      | <span data-ttu-id="687fd-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="687fd-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="687fd-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="687fd-122">Delegated (work or school account)</span></span> | <span data-ttu-id="687fd-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="687fd-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="687fd-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="687fd-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="687fd-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="687fd-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="687fd-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="687fd-126">Application</span></span> | <span data-ttu-id="687fd-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="687fd-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="687fd-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="687fd-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="687fd-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="687fd-129">Optional query parameters</span></span>

<span data-ttu-id="687fd-130">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="687fd-130">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="687fd-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="687fd-131">Response</span></span>

<span data-ttu-id="687fd-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ThumbnailSet](../resources/thumbnailset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="687fd-132">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="687fd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="687fd-133">Example</span></span>

<span data-ttu-id="687fd-134">Ниже представлен пример запроса на получение доступных эскизов элемента в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="687fd-134">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="687fd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="687fd-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="687fd-136">C#</span><span class="sxs-lookup"><span data-stu-id="687fd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="687fd-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="687fd-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="687fd-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="687fd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="687fd-139">Java</span><span class="sxs-lookup"><span data-stu-id="687fd-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-item-thumbnails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="687fd-140">Этот запрос возвращает массив доступных объектов **thumbnailSet** для элемента.</span><span class="sxs-lookup"><span data-stu-id="687fd-140">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="687fd-141">У любого элемента в объекте drive может быть один или несколько эскизов (либо ни одного эскиза).</span><span class="sxs-lookup"><span data-stu-id="687fd-141">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="687fd-p105">**Примечание.** С помощью параметра _select_ строки запроса вы можете указывать размеры эскизов, возвращаемых в объекте **ThumbnailSet**. Например, запрос `/thumbnails?select=medium` получает только эскизы среднего размера.</span><span class="sxs-lookup"><span data-stu-id="687fd-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="687fd-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="687fd-144">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="687fd-145">Получение одного эскиза</span><span class="sxs-lookup"><span data-stu-id="687fd-145">Get a single thumbnail</span></span>

<span data-ttu-id="687fd-146">Получение метаданных для одного эскиза и размера с помощью прямого запроса.</span><span class="sxs-lookup"><span data-stu-id="687fd-146">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="687fd-147">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="687fd-147">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="687fd-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="687fd-148">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="687fd-149">C#</span><span class="sxs-lookup"><span data-stu-id="687fd-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="687fd-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="687fd-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="687fd-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="687fd-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="687fd-152">Java</span><span class="sxs-lookup"><span data-stu-id="687fd-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-one-thumbnail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="687fd-153">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="687fd-153">Path parameters</span></span>

| <span data-ttu-id="687fd-154">Имя</span><span class="sxs-lookup"><span data-stu-id="687fd-154">Name</span></span>         | <span data-ttu-id="687fd-155">Тип</span><span class="sxs-lookup"><span data-stu-id="687fd-155">Type</span></span>   | <span data-ttu-id="687fd-156">Описание</span><span class="sxs-lookup"><span data-stu-id="687fd-156">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="687fd-157">**item-id**</span><span class="sxs-lookup"><span data-stu-id="687fd-157">**item-id**</span></span>  | <span data-ttu-id="687fd-158">string</span><span class="sxs-lookup"><span data-stu-id="687fd-158">string</span></span> | <span data-ttu-id="687fd-159">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="687fd-159">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="687fd-160">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="687fd-160">**thumb-id**</span></span> | <span data-ttu-id="687fd-161">number</span><span class="sxs-lookup"><span data-stu-id="687fd-161">number</span></span> | <span data-ttu-id="687fd-p106">Индекс эскиза (как правило, 0–4). Если присутствует пользовательский эскиз, для него задается индекс 0.</span><span class="sxs-lookup"><span data-stu-id="687fd-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="687fd-164">**size**</span><span class="sxs-lookup"><span data-stu-id="687fd-164">**size**</span></span>     | <span data-ttu-id="687fd-165">string</span><span class="sxs-lookup"><span data-stu-id="687fd-165">string</span></span> | <span data-ttu-id="687fd-166">Размер запрашиваемого эскиза.</span><span class="sxs-lookup"><span data-stu-id="687fd-166">The size of the thumbnail requested.</span></span> <span data-ttu-id="687fd-167">Это должен быть один из стандартных размеров, указанных ниже, либо пользовательский размер.</span><span class="sxs-lookup"><span data-stu-id="687fd-167">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="687fd-168">Получение двоичного содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="687fd-168">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="687fd-169">Вы можете получить содержимое эскиза напрямую, запросив свойство **content** этого эскиза.</span><span class="sxs-lookup"><span data-stu-id="687fd-169">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="687fd-170">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="687fd-170">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="687fd-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="687fd-171">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="687fd-172">C#</span><span class="sxs-lookup"><span data-stu-id="687fd-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="687fd-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="687fd-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="687fd-174">Цель — C</span><span class="sxs-lookup"><span data-stu-id="687fd-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="687fd-175">Java</span><span class="sxs-lookup"><span data-stu-id="687fd-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="687fd-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="687fd-176">Response</span></span>

<span data-ttu-id="687fd-177">В ответ служба выполняет перенаправление на URL-адрес эскиза.</span><span class="sxs-lookup"><span data-stu-id="687fd-177">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="687fd-178">URL-адреса эскизов не кэшируются.</span><span class="sxs-lookup"><span data-stu-id="687fd-178">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="687fd-179">Если в результате изменения элемента потребуется создать новый эскиз, изменится его URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="687fd-179">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="687fd-180">Получение эскизов при перечислении ресурсов DriveItem</span><span class="sxs-lookup"><span data-stu-id="687fd-180">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="687fd-181">При получении списка отображаемых ресурсов DriveItem можно использовать параметр строки запроса _$expand_, чтобы также включить эскизы этих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="687fd-181">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="687fd-182">Благодаря этому приложение может получить эскизы и элементы в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="687fd-182">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="687fd-183">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="687fd-183">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="687fd-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="687fd-184">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="687fd-185">C#</span><span class="sxs-lookup"><span data-stu-id="687fd-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="687fd-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="687fd-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="687fd-187">Цель — C</span><span class="sxs-lookup"><span data-stu-id="687fd-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="687fd-188">Java</span><span class="sxs-lookup"><span data-stu-id="687fd-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-while-listing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="687fd-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="687fd-189">Response</span></span>

<span data-ttu-id="687fd-190">Служба возвращает список ресурсов DriveItem и их эскизов.</span><span class="sxs-lookup"><span data-stu-id="687fd-190">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-values"></a><span data-ttu-id="687fd-191">Значения размера</span><span class="sxs-lookup"><span data-stu-id="687fd-191">Size values</span></span>

<span data-ttu-id="687fd-p110">В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.</span><span class="sxs-lookup"><span data-stu-id="687fd-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="687fd-194">Имя</span><span class="sxs-lookup"><span data-stu-id="687fd-194">Name</span></span>           | <span data-ttu-id="687fd-195">Разрешение</span><span class="sxs-lookup"><span data-stu-id="687fd-195">Resolution</span></span>  | <span data-ttu-id="687fd-196">Пропорции</span><span class="sxs-lookup"><span data-stu-id="687fd-196">Aspect Ratio</span></span> | <span data-ttu-id="687fd-197">Описание</span><span class="sxs-lookup"><span data-stu-id="687fd-197">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="687fd-198">96 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="687fd-198">96 longest</span></span>  | <span data-ttu-id="687fd-199">Исходные</span><span class="sxs-lookup"><span data-stu-id="687fd-199">Original</span></span>     | <span data-ttu-id="687fd-200">Небольшой эскиз с сильным сжатием, обрезанный до квадрата.</span><span class="sxs-lookup"><span data-stu-id="687fd-200">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="687fd-201">176 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="687fd-201">176 longest</span></span> | <span data-ttu-id="687fd-202">Исходные</span><span class="sxs-lookup"><span data-stu-id="687fd-202">Original</span></span>     | <span data-ttu-id="687fd-203">Обрезан до стандартного размера элемента для веб-представления OneDrive.</span><span class="sxs-lookup"><span data-stu-id="687fd-203">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="687fd-204">800 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="687fd-204">800 longest</span></span> | <span data-ttu-id="687fd-205">Исходные</span><span class="sxs-lookup"><span data-stu-id="687fd-205">Original</span></span>     | <span data-ttu-id="687fd-206">Эскиз, длина большей стороны которого изменена на 800 пикселей.</span><span class="sxs-lookup"><span data-stu-id="687fd-206">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="687fd-207">96x96</span><span class="sxs-lookup"><span data-stu-id="687fd-207">96x96</span></span>       | <span data-ttu-id="687fd-208">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="687fd-208">Square Crop</span></span>  | <span data-ttu-id="687fd-209">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="687fd-209">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="687fd-210">176x176</span><span class="sxs-lookup"><span data-stu-id="687fd-210">176x176</span></span>     | <span data-ttu-id="687fd-211">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="687fd-211">Square Crop</span></span>  | <span data-ttu-id="687fd-212">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="687fd-212">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="687fd-213">800x800</span><span class="sxs-lookup"><span data-stu-id="687fd-213">800x800</span></span>     | <span data-ttu-id="687fd-214">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="687fd-214">Square Crop</span></span>  | <span data-ttu-id="687fd-215">Большой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="687fd-215">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="687fd-216">Запрос эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="687fd-216">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="687fd-217">Помимо определенных размеров, приложение может запрашивать эскизы настраиваемых размеров, указав ширину и высоту с префиксом `c`.</span><span class="sxs-lookup"><span data-stu-id="687fd-217">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="687fd-218">Например, если вашему приложению нужны эскизы размером 300x400, оно может запросить размер следующим образом:</span><span class="sxs-lookup"><span data-stu-id="687fd-218">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="687fd-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="687fd-219">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request","name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="687fd-220">C#</span><span class="sxs-lookup"><span data-stu-id="687fd-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="687fd-221">Javascript</span><span class="sxs-lookup"><span data-stu-id="687fd-221">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="687fd-222">Цель — C</span><span class="sxs-lookup"><span data-stu-id="687fd-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="687fd-223">Java</span><span class="sxs-lookup"><span data-stu-id="687fd-223">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-custom-size-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="687fd-224">В ответ вы получите только эскиз выбранного размера:</span><span class="sxs-lookup"><span data-stu-id="687fd-224">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="687fd-225">Запросив размер эскиза, вы можете указать следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="687fd-225">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="687fd-226">Примеры пользовательских идентификаторов</span><span class="sxs-lookup"><span data-stu-id="687fd-226">Examples of custom identifiers</span></span>

| <span data-ttu-id="687fd-227">Идентификатор эскиза</span><span class="sxs-lookup"><span data-stu-id="687fd-227">Thumbnail identifier</span></span> | <span data-ttu-id="687fd-228">Разрешение</span><span class="sxs-lookup"><span data-stu-id="687fd-228">Resolution</span></span>             | <span data-ttu-id="687fd-229">Пропорции</span><span class="sxs-lookup"><span data-stu-id="687fd-229">Aspect ratio</span></span> | <span data-ttu-id="687fd-230">Описание</span><span class="sxs-lookup"><span data-stu-id="687fd-230">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="687fd-231">c300x400</span><span class="sxs-lookup"><span data-stu-id="687fd-231">c300x400</span></span>             | <span data-ttu-id="687fd-232">Заключен в прямоугольник размером 300x400</span><span class="sxs-lookup"><span data-stu-id="687fd-232">Bounded by 300x400 box</span></span> | <span data-ttu-id="687fd-233">Исходные</span><span class="sxs-lookup"><span data-stu-id="687fd-233">Original</span></span>     | <span data-ttu-id="687fd-234">Создается эскиз, который помещается в прямоугольник размером 300x400 пикселей с сохранением пропорций.</span><span class="sxs-lookup"><span data-stu-id="687fd-234">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="687fd-235">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="687fd-235">c300x400_Crop</span></span>        | <span data-ttu-id="687fd-236">300x400</span><span class="sxs-lookup"><span data-stu-id="687fd-236">300x400</span></span>                | <span data-ttu-id="687fd-237">Обрезанный</span><span class="sxs-lookup"><span data-stu-id="687fd-237">Cropped</span></span>      | <span data-ttu-id="687fd-p112">Создается эскиз размером 300x400. Сначала размер изображения меняется так, чтобы оно помещалось в прямоугольник размером 300x400, а затем обрезается все, что выходит за пределы прямоугольника.</span><span class="sxs-lookup"><span data-stu-id="687fd-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="687fd-240">**Примечание.** Размер возвращаемого эскиза в пикселях может не полностью совпадать с запрашиваемым, но его пропорции будут соответствовать запросу.</span><span class="sxs-lookup"><span data-stu-id="687fd-240">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="687fd-241">В некоторых случаях возвращаются эскизы большего размера, если эскиз уже существует и легко масштабируется до запрашиваемого разрешения.</span><span class="sxs-lookup"><span data-stu-id="687fd-241">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="687fd-242">Замечания</span><span class="sxs-lookup"><span data-stu-id="687fd-242">Remarks</span></span>

<span data-ttu-id="687fd-243">**Примечание.** В OneDrive для бизнеса и SharePoint:</span><span class="sxs-lookup"><span data-stu-id="687fd-243">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="687fd-244">С помощью таких вызовов невозможно дополнить коллекцию эскизов:</span><span class="sxs-lookup"><span data-stu-id="687fd-244">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="687fd-245">Эскизы не поддерживаются в SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="687fd-245">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="687fd-246">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="687fd-246">Error responses</span></span>

<span data-ttu-id="687fd-247">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="687fd-247">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
