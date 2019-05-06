---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение эскизов файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e220caed7a745caf7f75935ed9b47eb415173135
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590046"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="e7321-102">Список эскизов для ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="e7321-102">List thumbnails for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7321-103">Получение коллекции ресурсов [ThumbnailSet](../resources/thumbnailset.md) для ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e7321-103">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="e7321-p101">Ресурс DriveItem представляют ресурсы [ThumbnailSet](../resources/thumbnailset.md), количество которых может быть нуль и более. Каждый ресурс **thumbnailSet** может включать один или несколько объектов [**thumbnail**](../resources/thumbnail.md) — изображений, представляющих элемент. К примеру, ресурс **thumbnailSet** может включать такие распространенные объекты **thumbnail**, как `small`, `medium` и `large`.</span><span class="sxs-lookup"><span data-stu-id="e7321-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="e7321-p102">Работать с эскизами в OneDrive можно множеством способов. Ниже представлены наиболее распространенные из них.</span><span class="sxs-lookup"><span data-stu-id="e7321-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="e7321-109">Перечисление доступных эскизов элемента</span><span class="sxs-lookup"><span data-stu-id="e7321-109">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="e7321-110">Получение одного эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="e7321-110">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="e7321-111">Получение содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="e7321-111">Retrieve thumbnail content</span></span>
* <span data-ttu-id="e7321-112">Получение эскизов нескольких элементов в одном запросе</span><span class="sxs-lookup"><span data-stu-id="e7321-112">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="e7321-113">Получение эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="e7321-113">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="e7321-114">Отправка пользовательского эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="e7321-114">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="e7321-115">Определение того, существует ли отправленный пользовательский эскиз</span><span class="sxs-lookup"><span data-stu-id="e7321-115">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="e7321-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7321-116">Permissions</span></span>

<span data-ttu-id="e7321-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7321-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7321-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7321-119">Permission type</span></span>      | <span data-ttu-id="e7321-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7321-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7321-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7321-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e7321-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7321-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7321-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7321-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7321-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7321-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7321-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7321-125">Application</span></span> | <span data-ttu-id="e7321-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7321-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7321-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7321-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7321-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e7321-128">Optional query parameters</span></span>

<span data-ttu-id="e7321-129">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e7321-129">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="e7321-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7321-130">Response</span></span>

<span data-ttu-id="e7321-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ThumbnailSet](../resources/thumbnailset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e7321-131">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7321-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e7321-132">Example</span></span>

<span data-ttu-id="e7321-133">Ниже представлен пример запроса на получение доступных эскизов элемента в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="e7321-133">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

<span data-ttu-id="e7321-134">Этот запрос возвращает массив доступных объектов **thumbnailSet** для элемента.</span><span class="sxs-lookup"><span data-stu-id="e7321-134">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="e7321-135">У любого элемента в объекте drive может быть один или несколько эскизов (либо ни одного эскиза).</span><span class="sxs-lookup"><span data-stu-id="e7321-135">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="e7321-p105">**Примечание.** С помощью параметра _select_ строки запроса вы можете указывать размеры эскизов, возвращаемых в объекте **ThumbnailSet**. Например, запрос `/thumbnails?select=medium` получает только эскизы среднего размера.</span><span class="sxs-lookup"><span data-stu-id="e7321-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="e7321-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7321-138">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e7321-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="e7321-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e7321-140">Языках</span><span class="sxs-lookup"><span data-stu-id="e7321-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/enum-item-thumbnails-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7321-141">Язык</span><span class="sxs-lookup"><span data-stu-id="e7321-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/enum-item-thumbnails-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="e7321-142">Получение одного эскиза</span><span class="sxs-lookup"><span data-stu-id="e7321-142">Get a single thumbnail</span></span>

<span data-ttu-id="e7321-143">Получение метаданных для одного эскиза и размера с помощью прямого запроса.</span><span class="sxs-lookup"><span data-stu-id="e7321-143">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="e7321-144">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7321-144">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a><span data-ttu-id="e7321-145">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e7321-145">Path parameters</span></span>

| <span data-ttu-id="e7321-146">Имя</span><span class="sxs-lookup"><span data-stu-id="e7321-146">Name</span></span>         | <span data-ttu-id="e7321-147">Тип</span><span class="sxs-lookup"><span data-stu-id="e7321-147">Type</span></span>   | <span data-ttu-id="e7321-148">Описание</span><span class="sxs-lookup"><span data-stu-id="e7321-148">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="e7321-149">**item-id**</span><span class="sxs-lookup"><span data-stu-id="e7321-149">**item-id**</span></span>  | <span data-ttu-id="e7321-150">string</span><span class="sxs-lookup"><span data-stu-id="e7321-150">string</span></span> | <span data-ttu-id="e7321-151">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="e7321-151">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="e7321-152">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="e7321-152">**thumb-id**</span></span> | <span data-ttu-id="e7321-153">number</span><span class="sxs-lookup"><span data-stu-id="e7321-153">number</span></span> | <span data-ttu-id="e7321-p106">Индекс эскиза (как правило, 0–4). Если присутствует пользовательский эскиз, для него задается индекс 0.</span><span class="sxs-lookup"><span data-stu-id="e7321-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="e7321-156">**size**</span><span class="sxs-lookup"><span data-stu-id="e7321-156">**size**</span></span>     | <span data-ttu-id="e7321-157">string</span><span class="sxs-lookup"><span data-stu-id="e7321-157">string</span></span> | <span data-ttu-id="e7321-158">Размер запрашиваемого эскиза.</span><span class="sxs-lookup"><span data-stu-id="e7321-158">The size of the thumbnail requested.</span></span> <span data-ttu-id="e7321-159">Это должен быть один из стандартных размеров, указанных ниже, либо пользовательский размер.</span><span class="sxs-lookup"><span data-stu-id="e7321-159">This can be one of the standard sizes listed below or a custom size.</span></span> |

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e7321-160">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="e7321-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e7321-161">Языках</span><span class="sxs-lookup"><span data-stu-id="e7321-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-one-thumbnail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7321-162">Язык</span><span class="sxs-lookup"><span data-stu-id="e7321-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-one-thumbnail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="e7321-163">Получение двоичного содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="e7321-163">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="e7321-164">Вы можете получить содержимое эскиза напрямую, запросив свойство **content** этого эскиза.</span><span class="sxs-lookup"><span data-stu-id="e7321-164">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="e7321-165">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7321-165">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a><span data-ttu-id="e7321-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7321-166">Response</span></span>

<span data-ttu-id="e7321-167">В ответ служба перенаправляет на URL-адрес эскиза.</span><span class="sxs-lookup"><span data-stu-id="e7321-167">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e7321-168">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="e7321-168">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e7321-169">Языках</span><span class="sxs-lookup"><span data-stu-id="e7321-169">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-content-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7321-170">Язык</span><span class="sxs-lookup"><span data-stu-id="e7321-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-content-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e7321-171">URL-адреса эскизов не кэшируются.</span><span class="sxs-lookup"><span data-stu-id="e7321-171">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="e7321-172">Если в результате изменения элемента потребуется создать новый эскиз, изменится его URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="e7321-172">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="e7321-173">Получение эскизов при перечислении ресурсов DriveItem</span><span class="sxs-lookup"><span data-stu-id="e7321-173">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="e7321-174">При получении списка отображаемых ресурсов DriveItem можно использовать параметр строки запроса _$expand_, чтобы также включить эскизы этих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e7321-174">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="e7321-175">Благодаря этому приложение может получить эскизы и элементы в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="e7321-175">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="e7321-176">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7321-176">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a><span data-ttu-id="e7321-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7321-177">Response</span></span>

<span data-ttu-id="e7321-178">Служба возвращает список ресурсов DriveItem и их эскизов.</span><span class="sxs-lookup"><span data-stu-id="e7321-178">The service responses with the list of DriveItems and their thumbnails.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e7321-179">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="e7321-179">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e7321-180">Языках</span><span class="sxs-lookup"><span data-stu-id="e7321-180">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-while-listing-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7321-181">Язык</span><span class="sxs-lookup"><span data-stu-id="e7321-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-while-listing-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="size-values"></a><span data-ttu-id="e7321-182">Значения размера</span><span class="sxs-lookup"><span data-stu-id="e7321-182">Size values</span></span>

<span data-ttu-id="e7321-p110">В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.</span><span class="sxs-lookup"><span data-stu-id="e7321-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="e7321-185">Имя</span><span class="sxs-lookup"><span data-stu-id="e7321-185">Name</span></span>           | <span data-ttu-id="e7321-186">Разрешение</span><span class="sxs-lookup"><span data-stu-id="e7321-186">Resolution</span></span>  | <span data-ttu-id="e7321-187">Пропорции</span><span class="sxs-lookup"><span data-stu-id="e7321-187">Aspect Ratio</span></span> | <span data-ttu-id="e7321-188">Описание</span><span class="sxs-lookup"><span data-stu-id="e7321-188">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="e7321-189">96 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="e7321-189">96 longest</span></span>  | <span data-ttu-id="e7321-190">Исходные</span><span class="sxs-lookup"><span data-stu-id="e7321-190">Original</span></span>     | <span data-ttu-id="e7321-191">Небольшой эскиз с сильным сжатием, обрезанный до квадрата.</span><span class="sxs-lookup"><span data-stu-id="e7321-191">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="e7321-192">176 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="e7321-192">176 longest</span></span> | <span data-ttu-id="e7321-193">Исходные</span><span class="sxs-lookup"><span data-stu-id="e7321-193">Original</span></span>     | <span data-ttu-id="e7321-194">Обрезан до стандартного размера элемента для веб-представления OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e7321-194">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="e7321-195">800 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="e7321-195">800 longest</span></span> | <span data-ttu-id="e7321-196">Исходные</span><span class="sxs-lookup"><span data-stu-id="e7321-196">Original</span></span>     | <span data-ttu-id="e7321-197">Эскиз, длина большей стороны которого изменена на 800 пикселей.</span><span class="sxs-lookup"><span data-stu-id="e7321-197">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="e7321-198">96x96</span><span class="sxs-lookup"><span data-stu-id="e7321-198">96x96</span></span>       | <span data-ttu-id="e7321-199">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="e7321-199">Square Crop</span></span>  | <span data-ttu-id="e7321-200">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="e7321-200">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="e7321-201">176x176</span><span class="sxs-lookup"><span data-stu-id="e7321-201">176x176</span></span>     | <span data-ttu-id="e7321-202">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="e7321-202">Square Crop</span></span>  | <span data-ttu-id="e7321-203">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="e7321-203">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="e7321-204">800x800</span><span class="sxs-lookup"><span data-stu-id="e7321-204">800x800</span></span>     | <span data-ttu-id="e7321-205">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="e7321-205">Square Crop</span></span>  | <span data-ttu-id="e7321-206">Большой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="e7321-206">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="e7321-207">Запрос эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="e7321-207">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="e7321-208">Помимо определенных размеров, приложение может запрашивать эскизы настраиваемых размеров, указав ширину и высоту с префиксом `c`.</span><span class="sxs-lookup"><span data-stu-id="e7321-208">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="e7321-209">Например, если вашему приложению нужны эскизы размером 300x400, оно может запросить размер следующим образом:</span><span class="sxs-lookup"><span data-stu-id="e7321-209">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>

<!-- { "name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

<span data-ttu-id="e7321-210">В ответ вы получите только эскиз выбранного размера:</span><span class="sxs-lookup"><span data-stu-id="e7321-210">Which responds with just the custom thumbnail size selected:</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e7321-211">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="e7321-211">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e7321-212">Языках</span><span class="sxs-lookup"><span data-stu-id="e7321-212">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-custom-size-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7321-213">Язык</span><span class="sxs-lookup"><span data-stu-id="e7321-213">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-custom-size-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e7321-214">Запросив размер эскиза, вы можете указать следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="e7321-214">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="e7321-215">Примеры пользовательских идентификаторов</span><span class="sxs-lookup"><span data-stu-id="e7321-215">Examples of custom identifiers</span></span>

| <span data-ttu-id="e7321-216">Идентификатор эскиза</span><span class="sxs-lookup"><span data-stu-id="e7321-216">Thumbnail identifier</span></span> | <span data-ttu-id="e7321-217">Разрешение</span><span class="sxs-lookup"><span data-stu-id="e7321-217">Resolution</span></span>             | <span data-ttu-id="e7321-218">Пропорции</span><span class="sxs-lookup"><span data-stu-id="e7321-218">Aspect ratio</span></span> | <span data-ttu-id="e7321-219">Описание</span><span class="sxs-lookup"><span data-stu-id="e7321-219">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e7321-220">c300x400</span><span class="sxs-lookup"><span data-stu-id="e7321-220">c300x400</span></span>             | <span data-ttu-id="e7321-221">Заключен в прямоугольник размером 300x400</span><span class="sxs-lookup"><span data-stu-id="e7321-221">Bounded by 300x400 box</span></span> | <span data-ttu-id="e7321-222">Исходные</span><span class="sxs-lookup"><span data-stu-id="e7321-222">Original</span></span>     | <span data-ttu-id="e7321-223">Создается эскиз, который помещается в прямоугольник размером 300x400 пикселей с сохранением пропорций.</span><span class="sxs-lookup"><span data-stu-id="e7321-223">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="e7321-224">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="e7321-224">c300x400_Crop</span></span>        | <span data-ttu-id="e7321-225">300x400</span><span class="sxs-lookup"><span data-stu-id="e7321-225">300x400</span></span>                | <span data-ttu-id="e7321-226">Обрезанный</span><span class="sxs-lookup"><span data-stu-id="e7321-226">Cropped</span></span>      | <span data-ttu-id="e7321-p112">Создается эскиз размером 300x400. Сначала размер изображения меняется так, чтобы оно помещалось в прямоугольник размером 300x400, а затем обрезается все, что выходит за пределы прямоугольника.</span><span class="sxs-lookup"><span data-stu-id="e7321-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="e7321-229">**Примечание.** Размер возвращаемого эскиза в пикселях может не полностью совпадать с запрашиваемым, но его пропорции будут соответствовать запросу.</span><span class="sxs-lookup"><span data-stu-id="e7321-229">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="e7321-230">В некоторых случаях возвращаются эскизы большего размера, если эскиз уже существует и легко масштабируется до запрашиваемого разрешения.</span><span class="sxs-lookup"><span data-stu-id="e7321-230">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="e7321-231">Замечания</span><span class="sxs-lookup"><span data-stu-id="e7321-231">Remarks</span></span>

<span data-ttu-id="e7321-232">**Примечание.** В OneDrive для бизнеса и SharePoint:</span><span class="sxs-lookup"><span data-stu-id="e7321-232">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="e7321-233">С помощью таких вызовов невозможно дополнить коллекцию эскизов:</span><span class="sxs-lookup"><span data-stu-id="e7321-233">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="e7321-234">Эскизы не поддерживаются в SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="e7321-234">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="e7321-235">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="e7321-235">Error responses</span></span>

<span data-ttu-id="e7321-236">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="e7321-236">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
