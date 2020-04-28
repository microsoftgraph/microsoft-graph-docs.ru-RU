---
author: JeremyKelley
description: Получение коллекции ресурсов ThumbnailSet для ресурса DriveItem.
ms.date: 09/10/2017
title: Получение эскизов файла или папки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: be3c85dd72410b84b7fac49fe1e8794d56beab05
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432525"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="367ee-103">Список эскизов для ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="367ee-103">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="367ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="367ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="367ee-105">Получение коллекции ресурсов [ThumbnailSet](../resources/thumbnailset.md) для ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="367ee-105">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="367ee-p101">Ресурс DriveItem представляют ресурсы [ThumbnailSet](../resources/thumbnailset.md), количество которых может быть нуль и более. Каждый ресурс **thumbnailSet** может включать один или несколько объектов [**thumbnail**](../resources/thumbnail.md) — изображений, представляющих элемент. К примеру, ресурс **thumbnailSet** может включать такие распространенные объекты **thumbnail**, как `small`, `medium` и `large`.</span><span class="sxs-lookup"><span data-stu-id="367ee-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="367ee-p102">Работать с эскизами в OneDrive можно множеством способов. Ниже представлены наиболее распространенные из них.</span><span class="sxs-lookup"><span data-stu-id="367ee-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="367ee-111">Перечисление доступных эскизов элемента</span><span class="sxs-lookup"><span data-stu-id="367ee-111">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="367ee-112">Получение одного эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="367ee-112">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="367ee-113">Получение содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="367ee-113">Retrieve thumbnail content</span></span>
* <span data-ttu-id="367ee-114">Получение эскизов нескольких элементов в одном запросе</span><span class="sxs-lookup"><span data-stu-id="367ee-114">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="367ee-115">Получение эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="367ee-115">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="367ee-116">Отправка пользовательского эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="367ee-116">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="367ee-117">Определение того, существует ли отправленный пользовательский эскиз</span><span class="sxs-lookup"><span data-stu-id="367ee-117">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="367ee-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="367ee-118">Permissions</span></span>

<span data-ttu-id="367ee-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="367ee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="367ee-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="367ee-121">Permission type</span></span>      | <span data-ttu-id="367ee-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="367ee-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="367ee-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="367ee-123">Delegated (work or school account)</span></span> | <span data-ttu-id="367ee-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="367ee-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="367ee-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="367ee-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="367ee-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="367ee-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="367ee-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="367ee-127">Application</span></span> | <span data-ttu-id="367ee-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="367ee-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="367ee-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="367ee-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="367ee-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="367ee-130">Optional query parameters</span></span>

<span data-ttu-id="367ee-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="367ee-131">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="367ee-132">Кроме того, этот метод поддерживает получение эскиза с исходным значением EXIF и без примененного вращения путем добавления параметра `originalOrientation=true` запроса.</span><span class="sxs-lookup"><span data-stu-id="367ee-132">Additionally, this method supports retrieving the thumbnail with the original orientation EXIF value and without the applied rotation by appending the `originalOrientation=true` query parameter.</span></span>
<span data-ttu-id="367ee-133">В настоящее время поддерживается только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="367ee-133">This is currently only supported on OneDrive Personal.</span></span>

## <a name="response"></a><span data-ttu-id="367ee-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="367ee-134">Response</span></span>

<span data-ttu-id="367ee-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ThumbnailSet](../resources/thumbnailset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="367ee-135">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="367ee-136">Пример</span><span class="sxs-lookup"><span data-stu-id="367ee-136">Example</span></span>

<span data-ttu-id="367ee-137">Ниже представлен пример запроса на получение доступных эскизов элемента в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="367ee-137">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="367ee-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="367ee-138">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="c"></a>[<span data-ttu-id="367ee-139">C#</span><span class="sxs-lookup"><span data-stu-id="367ee-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="367ee-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="367ee-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="367ee-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="367ee-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="367ee-142">Этот запрос возвращает массив доступных объектов **thumbnailSet** для элемента.</span><span class="sxs-lookup"><span data-stu-id="367ee-142">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="367ee-143">У любого элемента в объекте drive может быть один или несколько эскизов (либо ни одного эскиза).</span><span class="sxs-lookup"><span data-stu-id="367ee-143">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="367ee-p106">**Примечание.** С помощью параметра _select_ строки запроса вы можете указывать размеры эскизов, возвращаемых в объекте **ThumbnailSet**. Например, запрос `/thumbnails?select=medium` получает только эскизы среднего размера.</span><span class="sxs-lookup"><span data-stu-id="367ee-p106">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="367ee-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="367ee-146">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="367ee-147">Получение одного эскиза</span><span class="sxs-lookup"><span data-stu-id="367ee-147">Get a single thumbnail</span></span>

<span data-ttu-id="367ee-148">Получение метаданных для одного эскиза и размера с помощью прямого запроса.</span><span class="sxs-lookup"><span data-stu-id="367ee-148">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="367ee-149">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="367ee-149">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="367ee-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="367ee-150">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="c"></a>[<span data-ttu-id="367ee-151">C#</span><span class="sxs-lookup"><span data-stu-id="367ee-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="367ee-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="367ee-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="367ee-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="367ee-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="367ee-154">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="367ee-154">Path parameters</span></span>

| <span data-ttu-id="367ee-155">Имя</span><span class="sxs-lookup"><span data-stu-id="367ee-155">Name</span></span>         | <span data-ttu-id="367ee-156">Тип</span><span class="sxs-lookup"><span data-stu-id="367ee-156">Type</span></span>   | <span data-ttu-id="367ee-157">Описание</span><span class="sxs-lookup"><span data-stu-id="367ee-157">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="367ee-158">**item-id**</span><span class="sxs-lookup"><span data-stu-id="367ee-158">**item-id**</span></span>  | <span data-ttu-id="367ee-159">string</span><span class="sxs-lookup"><span data-stu-id="367ee-159">string</span></span> | <span data-ttu-id="367ee-160">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="367ee-160">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="367ee-161">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="367ee-161">**thumb-id**</span></span> | <span data-ttu-id="367ee-162">число</span><span class="sxs-lookup"><span data-stu-id="367ee-162">number</span></span> | <span data-ttu-id="367ee-p107">Индекс эскиза (как правило, 0–4). Если присутствует пользовательский эскиз, для него задается индекс 0.</span><span class="sxs-lookup"><span data-stu-id="367ee-p107">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="367ee-165">**size**</span><span class="sxs-lookup"><span data-stu-id="367ee-165">**size**</span></span>     | <span data-ttu-id="367ee-166">string</span><span class="sxs-lookup"><span data-stu-id="367ee-166">string</span></span> | <span data-ttu-id="367ee-167">Размер запрашиваемого эскиза.</span><span class="sxs-lookup"><span data-stu-id="367ee-167">The size of the thumbnail requested.</span></span> <span data-ttu-id="367ee-168">Это должен быть один из стандартных размеров, указанных ниже, либо пользовательский размер.</span><span class="sxs-lookup"><span data-stu-id="367ee-168">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="367ee-169">Получение двоичного содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="367ee-169">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="367ee-170">Вы можете получить содержимое эскиза напрямую, запросив свойство **content** этого эскиза.</span><span class="sxs-lookup"><span data-stu-id="367ee-170">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="367ee-171">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="367ee-171">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="367ee-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="367ee-172">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="c"></a>[<span data-ttu-id="367ee-173">C#</span><span class="sxs-lookup"><span data-stu-id="367ee-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="367ee-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="367ee-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="367ee-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="367ee-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="367ee-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="367ee-176">Response</span></span>

<span data-ttu-id="367ee-177">В ответ служба выполняет перенаправление на URL-адрес эскиза.</span><span class="sxs-lookup"><span data-stu-id="367ee-177">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="367ee-178">URL-адреса эскизов не кэшируются.</span><span class="sxs-lookup"><span data-stu-id="367ee-178">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="367ee-179">Если в результате изменения элемента потребуется создать новый эскиз, изменится его URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="367ee-179">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="367ee-180">Получение эскизов при перечислении ресурсов DriveItem</span><span class="sxs-lookup"><span data-stu-id="367ee-180">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="367ee-181">При получении списка отображаемых ресурсов DriveItem можно использовать параметр строки запроса _$expand_, чтобы также включить эскизы этих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="367ee-181">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="367ee-182">Благодаря этому приложение может получить эскизы и элементы в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="367ee-182">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="367ee-183">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="367ee-183">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="367ee-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="367ee-184">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="c"></a>[<span data-ttu-id="367ee-185">C#</span><span class="sxs-lookup"><span data-stu-id="367ee-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="367ee-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="367ee-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="367ee-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="367ee-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="367ee-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="367ee-188">Response</span></span>

<span data-ttu-id="367ee-189">Служба возвращает список ресурсов DriveItem и их эскизов.</span><span class="sxs-lookup"><span data-stu-id="367ee-189">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-values"></a><span data-ttu-id="367ee-190">Значения размера</span><span class="sxs-lookup"><span data-stu-id="367ee-190">Size values</span></span>

<span data-ttu-id="367ee-p111">В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.</span><span class="sxs-lookup"><span data-stu-id="367ee-p111">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="367ee-193">Имя</span><span class="sxs-lookup"><span data-stu-id="367ee-193">Name</span></span>           | <span data-ttu-id="367ee-194">Разрешение</span><span class="sxs-lookup"><span data-stu-id="367ee-194">Resolution</span></span>  | <span data-ttu-id="367ee-195">Пропорции</span><span class="sxs-lookup"><span data-stu-id="367ee-195">Aspect Ratio</span></span> | <span data-ttu-id="367ee-196">Описание</span><span class="sxs-lookup"><span data-stu-id="367ee-196">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="367ee-197">96 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="367ee-197">96 longest</span></span>  | <span data-ttu-id="367ee-198">Исходные</span><span class="sxs-lookup"><span data-stu-id="367ee-198">Original</span></span>     | <span data-ttu-id="367ee-199">Небольшой эскиз с сильным сжатием, обрезанный до квадрата.</span><span class="sxs-lookup"><span data-stu-id="367ee-199">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="367ee-200">176 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="367ee-200">176 longest</span></span> | <span data-ttu-id="367ee-201">Исходные</span><span class="sxs-lookup"><span data-stu-id="367ee-201">Original</span></span>     | <span data-ttu-id="367ee-202">Обрезан до стандартного размера элемента для веб-представления OneDrive.</span><span class="sxs-lookup"><span data-stu-id="367ee-202">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="367ee-203">800 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="367ee-203">800 longest</span></span> | <span data-ttu-id="367ee-204">Исходные</span><span class="sxs-lookup"><span data-stu-id="367ee-204">Original</span></span>     | <span data-ttu-id="367ee-205">Эскиз, длина большей стороны которого изменена на 800 пикселей.</span><span class="sxs-lookup"><span data-stu-id="367ee-205">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="367ee-206">96x96</span><span class="sxs-lookup"><span data-stu-id="367ee-206">96x96</span></span>       | <span data-ttu-id="367ee-207">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="367ee-207">Square Crop</span></span>  | <span data-ttu-id="367ee-208">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="367ee-208">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="367ee-209">176x176</span><span class="sxs-lookup"><span data-stu-id="367ee-209">176x176</span></span>     | <span data-ttu-id="367ee-210">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="367ee-210">Square Crop</span></span>  | <span data-ttu-id="367ee-211">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="367ee-211">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="367ee-212">800x800</span><span class="sxs-lookup"><span data-stu-id="367ee-212">800x800</span></span>     | <span data-ttu-id="367ee-213">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="367ee-213">Square Crop</span></span>  | <span data-ttu-id="367ee-214">Большой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="367ee-214">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="367ee-215">Запрос эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="367ee-215">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="367ee-216">Помимо определенных размеров, приложение может запрашивать эскизы пользовательских размеров, указав ширину и высоту с префиксом `c`.</span><span class="sxs-lookup"><span data-stu-id="367ee-216">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="367ee-217">Например, если вашему приложению нужны эскизы размером 300x400, оно может запросить размер следующим образом:</span><span class="sxs-lookup"><span data-stu-id="367ee-217">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="http"></a>[<span data-ttu-id="367ee-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="367ee-218">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request","name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="c"></a>[<span data-ttu-id="367ee-219">C#</span><span class="sxs-lookup"><span data-stu-id="367ee-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="367ee-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="367ee-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="367ee-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="367ee-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="367ee-222">В ответ вы получите только эскиз выбранного размера:</span><span class="sxs-lookup"><span data-stu-id="367ee-222">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="367ee-223">Запросив размер эскиза, вы можете указать следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="367ee-223">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="367ee-224">Примеры пользовательских идентификаторов</span><span class="sxs-lookup"><span data-stu-id="367ee-224">Examples of custom identifiers</span></span>

| <span data-ttu-id="367ee-225">Идентификатор эскиза</span><span class="sxs-lookup"><span data-stu-id="367ee-225">Thumbnail identifier</span></span> | <span data-ttu-id="367ee-226">Разрешение</span><span class="sxs-lookup"><span data-stu-id="367ee-226">Resolution</span></span>             | <span data-ttu-id="367ee-227">Пропорции</span><span class="sxs-lookup"><span data-stu-id="367ee-227">Aspect ratio</span></span> | <span data-ttu-id="367ee-228">Описание</span><span class="sxs-lookup"><span data-stu-id="367ee-228">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="367ee-229">c300x400</span><span class="sxs-lookup"><span data-stu-id="367ee-229">c300x400</span></span>             | <span data-ttu-id="367ee-230">Заключен в прямоугольник размером 300x400</span><span class="sxs-lookup"><span data-stu-id="367ee-230">Bounded by 300x400 box</span></span> | <span data-ttu-id="367ee-231">Исходные</span><span class="sxs-lookup"><span data-stu-id="367ee-231">Original</span></span>     | <span data-ttu-id="367ee-232">Создается эскиз, который помещается в прямоугольник размером 300x400 пикселей с сохранением пропорций.</span><span class="sxs-lookup"><span data-stu-id="367ee-232">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="367ee-233">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="367ee-233">c300x400_Crop</span></span>        | <span data-ttu-id="367ee-234">300x400</span><span class="sxs-lookup"><span data-stu-id="367ee-234">300x400</span></span>                | <span data-ttu-id="367ee-235">Обрезанный</span><span class="sxs-lookup"><span data-stu-id="367ee-235">Cropped</span></span>      | <span data-ttu-id="367ee-p113">Создается эскиз размером 300x400. Сначала размер изображения меняется так, чтобы оно помещалось в прямоугольник размером 300x400, а затем обрезается все, что выходит за пределы прямоугольника.</span><span class="sxs-lookup"><span data-stu-id="367ee-p113">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="367ee-238">**Примечание.** Размер возвращаемого эскиза в пикселях может не полностью совпадать с запрашиваемым, но его пропорции будут соответствовать запросу.</span><span class="sxs-lookup"><span data-stu-id="367ee-238">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="367ee-239">В некоторых случаях возвращаются эскизы большего размера, если эскиз уже существует и легко масштабируется до запрашиваемого разрешения.</span><span class="sxs-lookup"><span data-stu-id="367ee-239">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="367ee-240">Примечания</span><span class="sxs-lookup"><span data-stu-id="367ee-240">Remarks</span></span>

<span data-ttu-id="367ee-241">**Примечание.** В OneDrive для бизнеса и SharePoint:</span><span class="sxs-lookup"><span data-stu-id="367ee-241">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="367ee-242">С помощью таких вызовов невозможно дополнить коллекцию эскизов:</span><span class="sxs-lookup"><span data-stu-id="367ee-242">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="367ee-243">Эскизы не поддерживаются в SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="367ee-243">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="367ee-244">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="367ee-244">Error responses</span></span>

<span data-ttu-id="367ee-245">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="367ee-245">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
