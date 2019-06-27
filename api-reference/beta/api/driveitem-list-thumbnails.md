---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение эскизов файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a8d53ba41fda9c915e8eec799e1cd96805e4dc0c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260104"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="c6265-102">Список эскизов для ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="c6265-102">List thumbnails for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6265-103">Получение коллекции ресурсов [ThumbnailSet](../resources/thumbnailset.md) для ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c6265-103">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="c6265-p101">Ресурс DriveItem представляют ресурсы [ThumbnailSet](../resources/thumbnailset.md), количество которых может быть нуль и более. Каждый ресурс **thumbnailSet** может включать один или несколько объектов [**thumbnail**](../resources/thumbnail.md) — изображений, представляющих элемент. К примеру, ресурс **thumbnailSet** может включать такие распространенные объекты **thumbnail**, как `small`, `medium` и `large`.</span><span class="sxs-lookup"><span data-stu-id="c6265-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="c6265-p102">Работать с эскизами в OneDrive можно множеством способов. Ниже представлены наиболее распространенные из них.</span><span class="sxs-lookup"><span data-stu-id="c6265-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="c6265-109">Перечисление доступных эскизов элемента</span><span class="sxs-lookup"><span data-stu-id="c6265-109">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="c6265-110">Получение одного эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="c6265-110">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="c6265-111">Получение содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="c6265-111">Retrieve thumbnail content</span></span>
* <span data-ttu-id="c6265-112">Получение эскизов нескольких элементов в одном запросе</span><span class="sxs-lookup"><span data-stu-id="c6265-112">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="c6265-113">Получение эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="c6265-113">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="c6265-114">Отправка пользовательского эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="c6265-114">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="c6265-115">Определение того, существует ли отправленный пользовательский эскиз</span><span class="sxs-lookup"><span data-stu-id="c6265-115">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="c6265-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6265-116">Permissions</span></span>

<span data-ttu-id="c6265-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6265-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6265-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6265-119">Permission type</span></span>      | <span data-ttu-id="c6265-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6265-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6265-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6265-121">Delegated (work or school account)</span></span> | <span data-ttu-id="c6265-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6265-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c6265-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6265-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6265-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6265-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c6265-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6265-125">Application</span></span> | <span data-ttu-id="c6265-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6265-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6265-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6265-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c6265-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c6265-128">Optional query parameters</span></span>

<span data-ttu-id="c6265-129">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c6265-129">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="c6265-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6265-130">Response</span></span>

<span data-ttu-id="c6265-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ThumbnailSet](../resources/thumbnailset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c6265-131">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6265-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c6265-132">Example</span></span>

<span data-ttu-id="c6265-133">Ниже представлен пример запроса на получение доступных эскизов элемента в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="c6265-133">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

<span data-ttu-id="c6265-134">Этот запрос возвращает массив доступных объектов **thumbnailSet** для элемента.</span><span class="sxs-lookup"><span data-stu-id="c6265-134">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="c6265-135">У любого элемента в объекте drive может быть один или несколько эскизов (либо ни одного эскиза).</span><span class="sxs-lookup"><span data-stu-id="c6265-135">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="c6265-p105">**Примечание.** С помощью параметра _select_ строки запроса вы можете указывать размеры эскизов, возвращаемых в объекте **ThumbnailSet**. Например, запрос `/thumbnails?select=medium` получает только эскизы среднего размера.</span><span class="sxs-lookup"><span data-stu-id="c6265-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="c6265-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6265-138">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6265-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c6265-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6265-140">C#</span><span class="sxs-lookup"><span data-stu-id="c6265-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/enum-item-thumbnails-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6265-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6265-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/enum-item-thumbnails-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c6265-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c6265-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/enum-item-thumbnails-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="c6265-143">Получение одного эскиза</span><span class="sxs-lookup"><span data-stu-id="c6265-143">Get a single thumbnail</span></span>

<span data-ttu-id="c6265-144">Получение метаданных для одного эскиза и размера с помощью прямого запроса.</span><span class="sxs-lookup"><span data-stu-id="c6265-144">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="c6265-145">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6265-145">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a><span data-ttu-id="c6265-146">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c6265-146">Path parameters</span></span>

| <span data-ttu-id="c6265-147">Имя</span><span class="sxs-lookup"><span data-stu-id="c6265-147">Name</span></span>         | <span data-ttu-id="c6265-148">Тип</span><span class="sxs-lookup"><span data-stu-id="c6265-148">Type</span></span>   | <span data-ttu-id="c6265-149">Описание</span><span class="sxs-lookup"><span data-stu-id="c6265-149">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="c6265-150">**item-id**</span><span class="sxs-lookup"><span data-stu-id="c6265-150">**item-id**</span></span>  | <span data-ttu-id="c6265-151">string</span><span class="sxs-lookup"><span data-stu-id="c6265-151">string</span></span> | <span data-ttu-id="c6265-152">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="c6265-152">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="c6265-153">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="c6265-153">**thumb-id**</span></span> | <span data-ttu-id="c6265-154">number</span><span class="sxs-lookup"><span data-stu-id="c6265-154">number</span></span> | <span data-ttu-id="c6265-p106">Индекс эскиза (как правило, 0–4). Если присутствует пользовательский эскиз, для него задается индекс 0.</span><span class="sxs-lookup"><span data-stu-id="c6265-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="c6265-157">**size**</span><span class="sxs-lookup"><span data-stu-id="c6265-157">**size**</span></span>     | <span data-ttu-id="c6265-158">string</span><span class="sxs-lookup"><span data-stu-id="c6265-158">string</span></span> | <span data-ttu-id="c6265-159">Размер запрашиваемого эскиза.</span><span class="sxs-lookup"><span data-stu-id="c6265-159">The size of the thumbnail requested.</span></span> <span data-ttu-id="c6265-160">Это должен быть один из стандартных размеров, указанных ниже, либо пользовательский размер.</span><span class="sxs-lookup"><span data-stu-id="c6265-160">This can be one of the standard sizes listed below or a custom size.</span></span> |

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6265-161">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c6265-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6265-162">C#</span><span class="sxs-lookup"><span data-stu-id="c6265-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-one-thumbnail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6265-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6265-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-one-thumbnail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c6265-164">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c6265-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-one-thumbnail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="c6265-165">Получение двоичного содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="c6265-165">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="c6265-166">Вы можете получить содержимое эскиза напрямую, запросив свойство **content** этого эскиза.</span><span class="sxs-lookup"><span data-stu-id="c6265-166">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="c6265-167">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6265-167">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a><span data-ttu-id="c6265-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6265-168">Response</span></span>

<span data-ttu-id="c6265-169">В ответ служба перенаправляет на URL-адрес эскиза.</span><span class="sxs-lookup"><span data-stu-id="c6265-169">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6265-170">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c6265-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6265-171">C#</span><span class="sxs-lookup"><span data-stu-id="c6265-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-content-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6265-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6265-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-content-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c6265-173">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c6265-173">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-thumbnail-content-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="c6265-174">URL-адреса эскизов не кэшируются.</span><span class="sxs-lookup"><span data-stu-id="c6265-174">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="c6265-175">Если в результате изменения элемента потребуется создать новый эскиз, изменится его URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="c6265-175">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="c6265-176">Получение эскизов при перечислении ресурсов DriveItem</span><span class="sxs-lookup"><span data-stu-id="c6265-176">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="c6265-177">При получении списка отображаемых ресурсов DriveItem можно использовать параметр строки запроса _$expand_, чтобы также включить эскизы этих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c6265-177">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="c6265-178">Благодаря этому приложение может получить эскизы и элементы в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="c6265-178">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="c6265-179">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6265-179">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a><span data-ttu-id="c6265-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6265-180">Response</span></span>

<span data-ttu-id="c6265-181">Служба возвращает список ресурсов DriveItem и их эскизов.</span><span class="sxs-lookup"><span data-stu-id="c6265-181">The service responses with the list of DriveItems and their thumbnails.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6265-182">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c6265-182">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6265-183">C#</span><span class="sxs-lookup"><span data-stu-id="c6265-183">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-while-listing-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6265-184">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6265-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-while-listing-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c6265-185">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c6265-185">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-thumbnail-while-listing-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="size-values"></a><span data-ttu-id="c6265-186">Значения размера</span><span class="sxs-lookup"><span data-stu-id="c6265-186">Size values</span></span>

<span data-ttu-id="c6265-p110">В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.</span><span class="sxs-lookup"><span data-stu-id="c6265-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="c6265-189">Имя</span><span class="sxs-lookup"><span data-stu-id="c6265-189">Name</span></span>           | <span data-ttu-id="c6265-190">Разрешение</span><span class="sxs-lookup"><span data-stu-id="c6265-190">Resolution</span></span>  | <span data-ttu-id="c6265-191">Пропорции</span><span class="sxs-lookup"><span data-stu-id="c6265-191">Aspect Ratio</span></span> | <span data-ttu-id="c6265-192">Описание</span><span class="sxs-lookup"><span data-stu-id="c6265-192">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="c6265-193">96 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="c6265-193">96 longest</span></span>  | <span data-ttu-id="c6265-194">Исходные</span><span class="sxs-lookup"><span data-stu-id="c6265-194">Original</span></span>     | <span data-ttu-id="c6265-195">Небольшой эскиз с сильным сжатием, обрезанный до квадрата.</span><span class="sxs-lookup"><span data-stu-id="c6265-195">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="c6265-196">176 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="c6265-196">176 longest</span></span> | <span data-ttu-id="c6265-197">Исходные</span><span class="sxs-lookup"><span data-stu-id="c6265-197">Original</span></span>     | <span data-ttu-id="c6265-198">Обрезан до стандартного размера элемента для веб-представления OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c6265-198">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="c6265-199">800 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="c6265-199">800 longest</span></span> | <span data-ttu-id="c6265-200">Исходные</span><span class="sxs-lookup"><span data-stu-id="c6265-200">Original</span></span>     | <span data-ttu-id="c6265-201">Эскиз, длина большей стороны которого изменена на 800 пикселей.</span><span class="sxs-lookup"><span data-stu-id="c6265-201">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="c6265-202">96x96</span><span class="sxs-lookup"><span data-stu-id="c6265-202">96x96</span></span>       | <span data-ttu-id="c6265-203">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="c6265-203">Square Crop</span></span>  | <span data-ttu-id="c6265-204">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="c6265-204">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="c6265-205">176x176</span><span class="sxs-lookup"><span data-stu-id="c6265-205">176x176</span></span>     | <span data-ttu-id="c6265-206">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="c6265-206">Square Crop</span></span>  | <span data-ttu-id="c6265-207">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="c6265-207">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="c6265-208">800x800</span><span class="sxs-lookup"><span data-stu-id="c6265-208">800x800</span></span>     | <span data-ttu-id="c6265-209">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="c6265-209">Square Crop</span></span>  | <span data-ttu-id="c6265-210">Большой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="c6265-210">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="c6265-211">Запрос эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="c6265-211">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="c6265-212">Помимо определенных размеров, приложение может запрашивать эскизы настраиваемых размеров, указав ширину и высоту с префиксом `c`.</span><span class="sxs-lookup"><span data-stu-id="c6265-212">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="c6265-213">Например, если вашему приложению нужны эскизы размером 300x400, оно может запросить размер следующим образом:</span><span class="sxs-lookup"><span data-stu-id="c6265-213">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>

<!-- { "name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

<span data-ttu-id="c6265-214">В ответ вы получите только эскиз выбранного размера:</span><span class="sxs-lookup"><span data-stu-id="c6265-214">Which responds with just the custom thumbnail size selected:</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6265-215">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c6265-215">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6265-216">C#</span><span class="sxs-lookup"><span data-stu-id="c6265-216">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-custom-size-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6265-217">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6265-217">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-custom-size-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c6265-218">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c6265-218">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-thumbnail-custom-size-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="c6265-219">Запросив размер эскиза, вы можете указать следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="c6265-219">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="c6265-220">Примеры пользовательских идентификаторов</span><span class="sxs-lookup"><span data-stu-id="c6265-220">Examples of custom identifiers</span></span>

| <span data-ttu-id="c6265-221">Идентификатор эскиза</span><span class="sxs-lookup"><span data-stu-id="c6265-221">Thumbnail identifier</span></span> | <span data-ttu-id="c6265-222">Разрешение</span><span class="sxs-lookup"><span data-stu-id="c6265-222">Resolution</span></span>             | <span data-ttu-id="c6265-223">Пропорции</span><span class="sxs-lookup"><span data-stu-id="c6265-223">Aspect ratio</span></span> | <span data-ttu-id="c6265-224">Описание</span><span class="sxs-lookup"><span data-stu-id="c6265-224">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c6265-225">c300x400</span><span class="sxs-lookup"><span data-stu-id="c6265-225">c300x400</span></span>             | <span data-ttu-id="c6265-226">Заключен в прямоугольник размером 300x400</span><span class="sxs-lookup"><span data-stu-id="c6265-226">Bounded by 300x400 box</span></span> | <span data-ttu-id="c6265-227">Исходные</span><span class="sxs-lookup"><span data-stu-id="c6265-227">Original</span></span>     | <span data-ttu-id="c6265-228">Создается эскиз, который помещается в прямоугольник размером 300x400 пикселей с сохранением пропорций.</span><span class="sxs-lookup"><span data-stu-id="c6265-228">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="c6265-229">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="c6265-229">c300x400_Crop</span></span>        | <span data-ttu-id="c6265-230">300x400</span><span class="sxs-lookup"><span data-stu-id="c6265-230">300x400</span></span>                | <span data-ttu-id="c6265-231">Обрезанный</span><span class="sxs-lookup"><span data-stu-id="c6265-231">Cropped</span></span>      | <span data-ttu-id="c6265-p112">Создается эскиз размером 300x400. Сначала размер изображения меняется так, чтобы оно помещалось в прямоугольник размером 300x400, а затем обрезается все, что выходит за пределы прямоугольника.</span><span class="sxs-lookup"><span data-stu-id="c6265-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="c6265-234">**Примечание.** Размер возвращаемого эскиза в пикселях может не полностью совпадать с запрашиваемым, но его пропорции будут соответствовать запросу.</span><span class="sxs-lookup"><span data-stu-id="c6265-234">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="c6265-235">В некоторых случаях возвращаются эскизы большего размера, если эскиз уже существует и легко масштабируется до запрашиваемого разрешения.</span><span class="sxs-lookup"><span data-stu-id="c6265-235">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="c6265-236">Замечания</span><span class="sxs-lookup"><span data-stu-id="c6265-236">Remarks</span></span>

<span data-ttu-id="c6265-237">**Примечание.** В OneDrive для бизнеса и SharePoint:</span><span class="sxs-lookup"><span data-stu-id="c6265-237">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="c6265-238">С помощью таких вызовов невозможно дополнить коллекцию эскизов:</span><span class="sxs-lookup"><span data-stu-id="c6265-238">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="c6265-239">Эскизы не поддерживаются в SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="c6265-239">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="c6265-240">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="c6265-240">Error responses</span></span>

<span data-ttu-id="c6265-241">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="c6265-241">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
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
