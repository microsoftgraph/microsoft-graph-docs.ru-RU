---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Получение эскизов файла или папки
localization_priority: Normal
ms.openlocfilehash: 48ea0b1f876fff28affc68895aed58a063df1513
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813715"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="1827a-102">Список эскизов для ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="1827a-102">List thumbnails for a DriveItem</span></span>

> <span data-ttu-id="1827a-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1827a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1827a-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1827a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1827a-105">Получение коллекции ресурсов [ThumbnailSet](../resources/thumbnailset.md) для ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1827a-105">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="1827a-p102">Ресурс DriveItem представляют ресурсы [ThumbnailSet](../resources/thumbnailset.md), количество которых может быть нуль и более. Каждый ресурс **thumbnailSet** может включать один или несколько объектов [**thumbnail**](../resources/thumbnail.md) — изображений, представляющих элемент. К примеру, ресурс **thumbnailSet** может включать такие распространенные объекты **thumbnail**, как `small`, `medium` и `large`.</span><span class="sxs-lookup"><span data-stu-id="1827a-p102">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="1827a-p103">Работать с эскизами в OneDrive можно множеством способов. Ниже представлены наиболее распространенные из них.</span><span class="sxs-lookup"><span data-stu-id="1827a-p103">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="1827a-111">Перечисление доступных эскизов элемента</span><span class="sxs-lookup"><span data-stu-id="1827a-111">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="1827a-112">Получение одного эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="1827a-112">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="1827a-113">Получение содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="1827a-113">Retrieve thumbnail content</span></span>
* <span data-ttu-id="1827a-114">Получение эскизов нескольких элементов в одном запросе</span><span class="sxs-lookup"><span data-stu-id="1827a-114">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="1827a-115">Получение эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="1827a-115">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="1827a-116">Отправка пользовательского эскиза элемента</span><span class="sxs-lookup"><span data-stu-id="1827a-116">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="1827a-117">Определение того, существует ли отправленный пользовательский эскиз</span><span class="sxs-lookup"><span data-stu-id="1827a-117">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="1827a-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1827a-118">Permissions</span></span>

<span data-ttu-id="1827a-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1827a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1827a-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1827a-121">Permission type</span></span>      | <span data-ttu-id="1827a-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1827a-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1827a-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1827a-123">Delegated (work or school account)</span></span> | <span data-ttu-id="1827a-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1827a-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1827a-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1827a-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1827a-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1827a-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1827a-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1827a-127">Application</span></span> | <span data-ttu-id="1827a-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1827a-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1827a-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1827a-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1827a-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1827a-130">Optional query parameters</span></span>

<span data-ttu-id="1827a-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1827a-131">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="1827a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1827a-132">Response</span></span>

<span data-ttu-id="1827a-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ThumbnailSet](../resources/thumbnailset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1827a-133">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1827a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1827a-134">Example</span></span>

<span data-ttu-id="1827a-135">Ниже представлен пример запроса на получение доступных эскизов элемента в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="1827a-135">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

<span data-ttu-id="1827a-136">Этот запрос возвращает массив доступных объектов **thumbnailSet** для элемента.</span><span class="sxs-lookup"><span data-stu-id="1827a-136">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="1827a-137">У любого элемента в объекте drive может быть один или несколько эскизов (либо ни одного эскиза).</span><span class="sxs-lookup"><span data-stu-id="1827a-137">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="1827a-138">**Примечание.** С помощью параметра _select_ строки запроса вы можете указывать размеры эскизов, возвращаемых в объекте **ThumbnailSet**.</span><span class="sxs-lookup"><span data-stu-id="1827a-138">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**.</span></span>
<span data-ttu-id="1827a-139">Например, запрос `/thumbnails?select=medium` получает только эскизы среднего размера.</span><span class="sxs-lookup"><span data-stu-id="1827a-139">For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="1827a-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="1827a-140">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="1827a-141">Получение одного эскиза</span><span class="sxs-lookup"><span data-stu-id="1827a-141">Get a single thumbnail</span></span>

<span data-ttu-id="1827a-142">Получение метаданных для одного эскиза и размера с помощью прямого запроса.</span><span class="sxs-lookup"><span data-stu-id="1827a-142">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="1827a-143">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1827a-143">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a><span data-ttu-id="1827a-144">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="1827a-144">Path parameters</span></span>

| <span data-ttu-id="1827a-145">Имя</span><span class="sxs-lookup"><span data-stu-id="1827a-145">Name</span></span>         | <span data-ttu-id="1827a-146">Тип</span><span class="sxs-lookup"><span data-stu-id="1827a-146">Type</span></span>   | <span data-ttu-id="1827a-147">Описание</span><span class="sxs-lookup"><span data-stu-id="1827a-147">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="1827a-148">**item-id**</span><span class="sxs-lookup"><span data-stu-id="1827a-148">**item-id**</span></span>  | <span data-ttu-id="1827a-149">string</span><span class="sxs-lookup"><span data-stu-id="1827a-149">string</span></span> | <span data-ttu-id="1827a-150">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="1827a-150">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="1827a-151">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="1827a-151">**thumb-id**</span></span> | <span data-ttu-id="1827a-152">number</span><span class="sxs-lookup"><span data-stu-id="1827a-152">number</span></span> | <span data-ttu-id="1827a-153">Индекс эскиза (как правило, 0–4).</span><span class="sxs-lookup"><span data-stu-id="1827a-153">The index of the thumbnail, usually 0-4.</span></span> <span data-ttu-id="1827a-154">Если присутствует пользовательский эскиз, для него задается индекс 0.</span><span class="sxs-lookup"><span data-stu-id="1827a-154">If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="1827a-155">**size**</span><span class="sxs-lookup"><span data-stu-id="1827a-155">**size**</span></span>     | <span data-ttu-id="1827a-156">string</span><span class="sxs-lookup"><span data-stu-id="1827a-156">string</span></span> | <span data-ttu-id="1827a-157">Размер запрашиваемого эскиза.</span><span class="sxs-lookup"><span data-stu-id="1827a-157">The size of the thumbnail requested.</span></span> <span data-ttu-id="1827a-158">Это должен быть один из стандартных размеров, указанных ниже, либо пользовательский размер.</span><span class="sxs-lookup"><span data-stu-id="1827a-158">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="1827a-159">Получение двоичного содержимого эскиза</span><span class="sxs-lookup"><span data-stu-id="1827a-159">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="1827a-160">Вы можете получить содержимое эскиза напрямую, запросив свойство **content** этого эскиза.</span><span class="sxs-lookup"><span data-stu-id="1827a-160">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="1827a-161">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1827a-161">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a><span data-ttu-id="1827a-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="1827a-162">Response</span></span>

<span data-ttu-id="1827a-163">В ответ служба выполняет перенаправление на URL-адрес эскиза.</span><span class="sxs-lookup"><span data-stu-id="1827a-163">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="1827a-164">URL-адреса эскизов не кэшируются.</span><span class="sxs-lookup"><span data-stu-id="1827a-164">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="1827a-165">Если в результате изменения элемента потребуется создать новый эскиз, изменится его URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="1827a-165">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="1827a-166">Получение эскизов при перечислении ресурсов DriveItem</span><span class="sxs-lookup"><span data-stu-id="1827a-166">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="1827a-167">При получении списка отображаемых ресурсов DriveItem можно использовать параметр строки запроса _$expand_, чтобы также включить эскизы этих ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1827a-167">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="1827a-168">Благодаря этому приложение может получить эскизы и элементы в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="1827a-168">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="1827a-169">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1827a-169">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a><span data-ttu-id="1827a-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="1827a-170">Response</span></span>

<span data-ttu-id="1827a-171">Служба возвращает список ресурсов DriveItem и их эскизов.</span><span class="sxs-lookup"><span data-stu-id="1827a-171">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-values"></a><span data-ttu-id="1827a-172">Значения размера</span><span class="sxs-lookup"><span data-stu-id="1827a-172">Size values</span></span>

<span data-ttu-id="1827a-p111">В этой таблице определены возможные размеры эскизов. Хотя вы можете указать в запросе произвольный размер эскиза, определенные значения встречаются намного чаще и позволяют быстрее получить результат.</span><span class="sxs-lookup"><span data-stu-id="1827a-p111">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="1827a-175">Имя</span><span class="sxs-lookup"><span data-stu-id="1827a-175">Name</span></span>           | <span data-ttu-id="1827a-176">Разрешение</span><span class="sxs-lookup"><span data-stu-id="1827a-176">Resolution</span></span>  | <span data-ttu-id="1827a-177">Пропорции</span><span class="sxs-lookup"><span data-stu-id="1827a-177">Aspect Ratio</span></span> | <span data-ttu-id="1827a-178">Описание</span><span class="sxs-lookup"><span data-stu-id="1827a-178">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="1827a-179">96 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="1827a-179">96 longest</span></span>  | <span data-ttu-id="1827a-180">Исходные</span><span class="sxs-lookup"><span data-stu-id="1827a-180">Original</span></span>     | <span data-ttu-id="1827a-181">Небольшой эскиз с сильным сжатием, обрезанный до квадрата.</span><span class="sxs-lookup"><span data-stu-id="1827a-181">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="1827a-182">176 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="1827a-182">176 longest</span></span> | <span data-ttu-id="1827a-183">Исходные</span><span class="sxs-lookup"><span data-stu-id="1827a-183">Original</span></span>     | <span data-ttu-id="1827a-184">Обрезан до стандартного размера элемента для веб-представления OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1827a-184">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="1827a-185">800 для большей стороны</span><span class="sxs-lookup"><span data-stu-id="1827a-185">800 longest</span></span> | <span data-ttu-id="1827a-186">Исходные</span><span class="sxs-lookup"><span data-stu-id="1827a-186">Original</span></span>     | <span data-ttu-id="1827a-187">Эскиз, длина большей стороны которого изменена на 800 пикселей.</span><span class="sxs-lookup"><span data-stu-id="1827a-187">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="1827a-188">96x96</span><span class="sxs-lookup"><span data-stu-id="1827a-188">96x96</span></span>       | <span data-ttu-id="1827a-189">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="1827a-189">Square Crop</span></span>  | <span data-ttu-id="1827a-190">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="1827a-190">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="1827a-191">176x176</span><span class="sxs-lookup"><span data-stu-id="1827a-191">176x176</span></span>     | <span data-ttu-id="1827a-192">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="1827a-192">Square Crop</span></span>  | <span data-ttu-id="1827a-193">Небольшой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="1827a-193">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="1827a-194">800x800</span><span class="sxs-lookup"><span data-stu-id="1827a-194">800x800</span></span>     | <span data-ttu-id="1827a-195">Квадратная обрезка</span><span class="sxs-lookup"><span data-stu-id="1827a-195">Square Crop</span></span>  | <span data-ttu-id="1827a-196">Большой квадратный эскиз</span><span class="sxs-lookup"><span data-stu-id="1827a-196">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="1827a-197">Запрос эскизов настраиваемых размеров</span><span class="sxs-lookup"><span data-stu-id="1827a-197">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="1827a-198">Помимо определенных размеров, приложение может запрашивать эскизы настраиваемых размеров, указав ширину и высоту с префиксом `c`.</span><span class="sxs-lookup"><span data-stu-id="1827a-198">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="1827a-199">Например, если вашему приложению нужны эскизы размером 300x400, оно может запросить размер следующим образом:</span><span class="sxs-lookup"><span data-stu-id="1827a-199">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>

<!-- { "name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

<span data-ttu-id="1827a-200">В ответ вы получите только эскиз выбранного размера:</span><span class="sxs-lookup"><span data-stu-id="1827a-200">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="1827a-201">Запросив размер эскиза, вы можете указать следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="1827a-201">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="1827a-202">Примеры пользовательских идентификаторов</span><span class="sxs-lookup"><span data-stu-id="1827a-202">Examples of custom identifiers</span></span>

| <span data-ttu-id="1827a-203">Идентификатор эскиза</span><span class="sxs-lookup"><span data-stu-id="1827a-203">Thumbnail identifier</span></span> | <span data-ttu-id="1827a-204">Разрешение</span><span class="sxs-lookup"><span data-stu-id="1827a-204">Resolution</span></span>             | <span data-ttu-id="1827a-205">Пропорции</span><span class="sxs-lookup"><span data-stu-id="1827a-205">Aspect ratio</span></span> | <span data-ttu-id="1827a-206">Описание</span><span class="sxs-lookup"><span data-stu-id="1827a-206">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1827a-207">c300x400</span><span class="sxs-lookup"><span data-stu-id="1827a-207">c300x400</span></span>             | <span data-ttu-id="1827a-208">Заключен в прямоугольник размером 300x400</span><span class="sxs-lookup"><span data-stu-id="1827a-208">Bounded by 300x400 box</span></span> | <span data-ttu-id="1827a-209">Исходные</span><span class="sxs-lookup"><span data-stu-id="1827a-209">Original</span></span>     | <span data-ttu-id="1827a-210">Создается эскиз, который помещается в прямоугольник размером 300x400 пикселей с сохранением пропорций.</span><span class="sxs-lookup"><span data-stu-id="1827a-210">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="1827a-211">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="1827a-211">c300x400_Crop</span></span>        | <span data-ttu-id="1827a-212">300x400</span><span class="sxs-lookup"><span data-stu-id="1827a-212">300x400</span></span>                | <span data-ttu-id="1827a-213">Обрезанный</span><span class="sxs-lookup"><span data-stu-id="1827a-213">Cropped</span></span>      | <span data-ttu-id="1827a-214">Создается эскиз размером 300x400.</span><span class="sxs-lookup"><span data-stu-id="1827a-214">Generate a thumbnail that is 300x400 pixels.</span></span> <span data-ttu-id="1827a-215">Сначала размер изображения меняется так, чтобы оно помещалось в прямоугольник размером 300x400, а затем обрезается все, что выходит за пределы прямоугольника.</span><span class="sxs-lookup"><span data-stu-id="1827a-215">This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="1827a-216">**Примечание.** Размер возвращаемого эскиза в пикселях может не полностью совпадать с запрашиваемым, но его пропорции будут соответствовать запросу.</span><span class="sxs-lookup"><span data-stu-id="1827a-216">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="1827a-217">В некоторых случаях возвращаются эскизы большего размера, если эскиз уже существует и легко масштабируется до запрашиваемого разрешения.</span><span class="sxs-lookup"><span data-stu-id="1827a-217">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="1827a-218">Примечания</span><span class="sxs-lookup"><span data-stu-id="1827a-218">Remarks</span></span>

<span data-ttu-id="1827a-219">**Примечание.** В OneDrive для бизнеса и SharePoint:</span><span class="sxs-lookup"><span data-stu-id="1827a-219">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="1827a-220">С помощью таких вызовов невозможно дополнить коллекцию эскизов:</span><span class="sxs-lookup"><span data-stu-id="1827a-220">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="1827a-221">Эскизы не поддерживаются в SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="1827a-221">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="1827a-222">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="1827a-222">Error responses</span></span>

<span data-ttu-id="1827a-223">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="1827a-223">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails"
} -->
