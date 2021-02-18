---
author: JeremyKelley
ms.date: 09/10/2017
title: Извлечение эскизов файла или папки
localization_priority: Normal
ms.prod: sharepoint
description: Получение коллекции ресурсов ThumbnailSet для ресурса DriveItem.
doc_type: apiPageType
ms.openlocfilehash: 9746221fe0aed4b606019250bd63f65d3972ebc3
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293045"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="1723a-103">Список эскизов для ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="1723a-103">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="1723a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1723a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1723a-105">Получение коллекции ресурсов [ThumbnailSet](../resources/thumbnailset.md) для ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1723a-105">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="1723a-p101">Ресурс DriveItem представляют ресурсы [ThumbnailSet](../resources/thumbnailset.md), количество которых может быть нуль и более. Каждый ресурс **thumbnailSet** может включать один или несколько объектов [**thumbnail**](../resources/thumbnail.md) — изображений, представляющих элемент. К примеру, ресурс **thumbnailSet** может включать такие распространенные объекты **thumbnail**, как `small`, `medium` и `large`.</span><span class="sxs-lookup"><span data-stu-id="1723a-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="1723a-p102">Работать с эскизами в OneDrive можно множеством способов. Ниже представлены наиболее распространенные из них.</span><span class="sxs-lookup"><span data-stu-id="1723a-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="1723a-111">Перечисление доступных эскизов элемента</span><span class="sxs-lookup"><span data-stu-id="1723a-111">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="1723a-112">Получение одного эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="1723a-112">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="1723a-113">Получение содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="1723a-113">Retrieve thumbnail content</span></span>
* <span data-ttu-id="1723a-114">Получение эскизов нескольких элементов в одном запросе</span><span class="sxs-lookup"><span data-stu-id="1723a-114">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="1723a-115">Получение эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="1723a-115">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="1723a-116">Отправка пользовательского эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="1723a-116">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="1723a-117">Определение того, существует ли отправленный пользовательский эскиз</span><span class="sxs-lookup"><span data-stu-id="1723a-117">Determine if a custom uploaded thumbnail exists</span></span>

## <a name="permissions"></a><span data-ttu-id="1723a-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1723a-118">Permissions</span></span>

<span data-ttu-id="1723a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1723a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1723a-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1723a-121">Permission type</span></span>      | <span data-ttu-id="1723a-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1723a-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1723a-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1723a-123">Delegated (work or school account)</span></span> | <span data-ttu-id="1723a-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1723a-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1723a-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1723a-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1723a-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1723a-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1723a-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1723a-127">Application</span></span> | <span data-ttu-id="1723a-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1723a-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1723a-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1723a-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1723a-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1723a-130">Optional query parameters</span></span>

<span data-ttu-id="1723a-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1723a-131">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="1723a-132">Кроме того, этот метод поддерживает искомый эскиз с исходным значением EXIF ориентации и без примененного поворота путем добавления `originalOrientation=true` параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="1723a-132">Additionally, this method supports retrieving the thumbnail with the original orientation EXIF value and without the applied rotation by appending the `originalOrientation=true` query parameter.</span></span>
<span data-ttu-id="1723a-133">В настоящее время этот параметр поддерживается только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="1723a-133">This is currently only supported on OneDrive Personal.</span></span>

## <a name="response"></a><span data-ttu-id="1723a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1723a-134">Response</span></span>

<span data-ttu-id="1723a-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ThumbnailSet](../resources/thumbnailset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1723a-135">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1723a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="1723a-136">Example</span></span>

<span data-ttu-id="1723a-137">Ниже представлен пример запроса на получение доступных эскизов элемента в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="1723a-137">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="1723a-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="1723a-138">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="c"></a>[<span data-ttu-id="1723a-139">C#</span><span class="sxs-lookup"><span data-stu-id="1723a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1723a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1723a-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1723a-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1723a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1723a-142">Java</span><span class="sxs-lookup"><span data-stu-id="1723a-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-item-thumbnails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="1723a-143">Этот запрос возвращает массив доступных объектов **thumbnailSet** для элемента.</span><span class="sxs-lookup"><span data-stu-id="1723a-143">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="1723a-144">У любого элемента в объекте drive может быть один или несколько эскизов (либо ни одного эскиза).</span><span class="sxs-lookup"><span data-stu-id="1723a-144">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="1723a-p106">**Примечание.** С помощью параметра _select_ строки запроса вы можете указывать размеры эскизов, возвращаемых в объекте **ThumbnailSet**. Например, запрос `/thumbnails?select=medium` получает только эскизы среднего размера.</span><span class="sxs-lookup"><span data-stu-id="1723a-p106">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="1723a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1723a-147">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="1723a-148">Получение одного эскиза</span><span class="sxs-lookup"><span data-stu-id="1723a-148">Get a single thumbnail</span></span>

<span data-ttu-id="1723a-149">Получение метаданных для одного эскиза и размера с помощью прямого запроса.</span><span class="sxs-lookup"><span data-stu-id="1723a-149">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="1723a-150">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1723a-150">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="1723a-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="1723a-151">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="c"></a>[<span data-ttu-id="1723a-152">C#</span><span class="sxs-lookup"><span data-stu-id="1723a-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1723a-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1723a-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1723a-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1723a-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1723a-155">Java</span><span class="sxs-lookup"><span data-stu-id="1723a-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-one-thumbnail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="1723a-156">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="1723a-156">Path parameters</span></span>

| <span data-ttu-id="1723a-157">Имя</span><span class="sxs-lookup"><span data-stu-id="1723a-157">Name</span></span>         | <span data-ttu-id="1723a-158">Тип</span><span class="sxs-lookup"><span data-stu-id="1723a-158">Type</span></span>   | <span data-ttu-id="1723a-159">Описание</span><span class="sxs-lookup"><span data-stu-id="1723a-159">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="1723a-160">**item-id**</span><span class="sxs-lookup"><span data-stu-id="1723a-160">**item-id**</span></span>  | <span data-ttu-id="1723a-161">string</span><span class="sxs-lookup"><span data-stu-id="1723a-161">string</span></span> | <span data-ttu-id="1723a-162">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="1723a-162">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="1723a-163">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="1723a-163">**thumb-id**</span></span> | <span data-ttu-id="1723a-164">число</span><span class="sxs-lookup"><span data-stu-id="1723a-164">number</span></span> | <span data-ttu-id="1723a-p107">Индекс эскиза (как правило, 0–4). Если присутствует пользовательский эскиз, для него задается индекс 0.</span><span class="sxs-lookup"><span data-stu-id="1723a-p107">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="1723a-167">**size**</span><span class="sxs-lookup"><span data-stu-id="1723a-167">**size**</span></span>     | <span data-ttu-id="1723a-168">string</span><span class="sxs-lookup"><span data-stu-id="1723a-168">string</span></span> | <span data-ttu-id="1723a-169">Размер запрашиваемого эскиза.</span><span class="sxs-lookup"><span data-stu-id="1723a-169">The size of the thumbnail requested.</span></span> <span data-ttu-id="1723a-170">Это должен быть один из стандартных размеров, указанных ниже, либо пользовательский размер.</span><span class="sxs-lookup"><span data-stu-id="1723a-170">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="1723a-171">Получение двоичного содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="1723a-171">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="1723a-172">Вы можете получить содержимое эскиза напрямую, запросив свойство **content** этого эскиза.</span><span class="sxs-lookup"><span data-stu-id="1723a-172">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="1723a-173">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1723a-173">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="1723a-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="1723a-174">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="c"></a>[<span data-ttu-id="1723a-175">C#</span><span class="sxs-lookup"><span data-stu-id="1723a-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1723a-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1723a-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1723a-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1723a-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1723a-178">Java</span><span class="sxs-lookup"><span data-stu-id="1723a-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1723a-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="1723a-179">Response</span></span>

<span data-ttu-id="1723a-180">В ответ служба выполняет перенаправление на URL-адрес эскиза.</span><span class="sxs-lookup"><span data-stu-id="1723a-180">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="1723a-181">URL-адреса эскизов не кэшируются.</span><span class="sxs-lookup"><span data-stu-id="1723a-181">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="1723a-182">Если в результате изменения элемента потребуется создать новый эскиз, изменится его URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="1723a-182">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="1723a-183">Получение эскизов при перечислении ресурсов DriveItem</span><span class="sxs-lookup"><span data-stu-id="1723a-183">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="1723a-184">При получении списка отображаемых ресурсов DriveItem можно использовать параметр строки запроса _$expand_, чтобы также включить эскизы этих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1723a-184">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="1723a-185">Благодаря этому приложение может получить эскизы и элементы в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="1723a-185">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="1723a-186">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1723a-186">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="1723a-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="1723a-187">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="c"></a>[<span data-ttu-id="1723a-188">C#</span><span class="sxs-lookup"><span data-stu-id="1723a-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1723a-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1723a-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1723a-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1723a-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1723a-191">Java</span><span class="sxs-lookup"><span data-stu-id="1723a-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-while-listing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1723a-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="1723a-192">Response</span></span>

<span data-ttu-id="1723a-193">Служба возвращает список ресурсов DriveItem и их эскизов.</span><span class="sxs-lookup"><span data-stu-id="1723a-193">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-options"></a><span data-ttu-id="1723a-194">Параметры размера</span><span class="sxs-lookup"><span data-stu-id="1723a-194">Size options</span></span>

<span data-ttu-id="1723a-p111">В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.</span><span class="sxs-lookup"><span data-stu-id="1723a-p111">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="1723a-197">Имя</span><span class="sxs-lookup"><span data-stu-id="1723a-197">Name</span></span>           | <span data-ttu-id="1723a-198">Разрешение</span><span class="sxs-lookup"><span data-stu-id="1723a-198">Resolution</span></span>  | <span data-ttu-id="1723a-199">Пропорции</span><span class="sxs-lookup"><span data-stu-id="1723a-199">Aspect Ratio</span></span> | <span data-ttu-id="1723a-200">Описание</span><span class="sxs-lookup"><span data-stu-id="1723a-200">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="1723a-201">96 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="1723a-201">96 longest</span></span>  | <span data-ttu-id="1723a-202">Исходные</span><span class="sxs-lookup"><span data-stu-id="1723a-202">Original</span></span>     | <span data-ttu-id="1723a-203">Небольшой эскиз с сильным сжатием, обрезанный до квадрата.</span><span class="sxs-lookup"><span data-stu-id="1723a-203">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="1723a-204">176 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="1723a-204">176 longest</span></span> | <span data-ttu-id="1723a-205">Исходные</span><span class="sxs-lookup"><span data-stu-id="1723a-205">Original</span></span>     | <span data-ttu-id="1723a-206">Обрезан до стандартного размера элемента для веб-представления OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1723a-206">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="1723a-207">800 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="1723a-207">800 longest</span></span> | <span data-ttu-id="1723a-208">Исходные</span><span class="sxs-lookup"><span data-stu-id="1723a-208">Original</span></span>     | <span data-ttu-id="1723a-209">Эскиз, длина большей стороны которого изменена на 800 пикселей.</span><span class="sxs-lookup"><span data-stu-id="1723a-209">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="1723a-210">96x96</span><span class="sxs-lookup"><span data-stu-id="1723a-210">96x96</span></span>       | <span data-ttu-id="1723a-211">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="1723a-211">Square Crop</span></span>  | <span data-ttu-id="1723a-212">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="1723a-212">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="1723a-213">176x176</span><span class="sxs-lookup"><span data-stu-id="1723a-213">176x176</span></span>     | <span data-ttu-id="1723a-214">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="1723a-214">Square Crop</span></span>  | <span data-ttu-id="1723a-215">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="1723a-215">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="1723a-216">800x800</span><span class="sxs-lookup"><span data-stu-id="1723a-216">800x800</span></span>     | <span data-ttu-id="1723a-217">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="1723a-217">Square Crop</span></span>  | <span data-ttu-id="1723a-218">Большой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="1723a-218">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="1723a-219">Запрос эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="1723a-219">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="1723a-220">Помимо определенных размеров, приложение может запрашивать эскизы пользовательских размеров, указав ширину и высоту с префиксом `c`.</span><span class="sxs-lookup"><span data-stu-id="1723a-220">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="1723a-221">Например, если вашему приложению нужны эскизы размером 300x400, оно может запросить размер следующим образом:</span><span class="sxs-lookup"><span data-stu-id="1723a-221">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="http"></a>[<span data-ttu-id="1723a-222">HTTP</span><span class="sxs-lookup"><span data-stu-id="1723a-222">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-thumbnail-custom-size", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="c"></a>[<span data-ttu-id="1723a-223">C#</span><span class="sxs-lookup"><span data-stu-id="1723a-223">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1723a-224">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1723a-224">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1723a-225">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1723a-225">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1723a-226">Java</span><span class="sxs-lookup"><span data-stu-id="1723a-226">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-custom-size-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="1723a-227">В ответ вы получите только эскиз выбранного размера:</span><span class="sxs-lookup"><span data-stu-id="1723a-227">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="1723a-228">Запросив размер эскиза, вы можете указать следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="1723a-228">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="1723a-229">Примеры пользовательских идентификаторов</span><span class="sxs-lookup"><span data-stu-id="1723a-229">Examples of custom identifiers</span></span>

| <span data-ttu-id="1723a-230">Идентификатор эскиза</span><span class="sxs-lookup"><span data-stu-id="1723a-230">Thumbnail identifier</span></span> | <span data-ttu-id="1723a-231">Разрешение</span><span class="sxs-lookup"><span data-stu-id="1723a-231">Resolution</span></span>             | <span data-ttu-id="1723a-232">Пропорции</span><span class="sxs-lookup"><span data-stu-id="1723a-232">Aspect ratio</span></span> | <span data-ttu-id="1723a-233">Описание</span><span class="sxs-lookup"><span data-stu-id="1723a-233">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1723a-234">c300x400</span><span class="sxs-lookup"><span data-stu-id="1723a-234">c300x400</span></span>             | <span data-ttu-id="1723a-235">Заключен в прямоугольник размером 300x400</span><span class="sxs-lookup"><span data-stu-id="1723a-235">Bounded by 300x400 box</span></span> | <span data-ttu-id="1723a-236">Исходные</span><span class="sxs-lookup"><span data-stu-id="1723a-236">Original</span></span>     | <span data-ttu-id="1723a-237">Создается эскиз, который помещается в прямоугольник размером 300x400 пикселей с сохранением пропорций.</span><span class="sxs-lookup"><span data-stu-id="1723a-237">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="1723a-238">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="1723a-238">c300x400_Crop</span></span>        | <span data-ttu-id="1723a-239">300x400</span><span class="sxs-lookup"><span data-stu-id="1723a-239">300x400</span></span>                | <span data-ttu-id="1723a-240">Обрезанный</span><span class="sxs-lookup"><span data-stu-id="1723a-240">Cropped</span></span>      | <span data-ttu-id="1723a-p113">Создается эскиз размером 300x400. Сначала размер изображения меняется так, чтобы оно помещалось в прямоугольник размером 300x400, а затем обрезается все, что выходит за пределы прямоугольника.</span><span class="sxs-lookup"><span data-stu-id="1723a-p113">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="1723a-243">**Примечание.** Размер возвращаемого эскиза в пикселях может не полностью совпадать с запрашиваемым, но его пропорции будут соответствовать запросу.</span><span class="sxs-lookup"><span data-stu-id="1723a-243">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="1723a-244">В некоторых случаях возвращаются эскизы большего размера, если эскиз уже существует и легко масштабируется до запрашиваемого разрешения.</span><span class="sxs-lookup"><span data-stu-id="1723a-244">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="1723a-245">Примечания</span><span class="sxs-lookup"><span data-stu-id="1723a-245">Remarks</span></span>

<span data-ttu-id="1723a-246">**Примечание.** В OneDrive для бизнеса и SharePoint:</span><span class="sxs-lookup"><span data-stu-id="1723a-246">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="1723a-247">С помощью таких вызовов невозможно дополнить коллекцию эскизов:</span><span class="sxs-lookup"><span data-stu-id="1723a-247">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="1723a-248">Эскизы не поддерживаются в SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="1723a-248">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="1723a-249">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="1723a-249">Error responses</span></span>

<span data-ttu-id="1723a-250">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="1723a-250">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": "Items/Thumbnails"
} -->

