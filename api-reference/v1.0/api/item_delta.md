# <a name="track-changes-for-a-drive"></a><span data-ttu-id="d0e2c-101">Отслеживание изменений для Drive</span><span class="sxs-lookup"><span data-stu-id="d0e2c-101">Track changes for a Drive</span></span>

<span data-ttu-id="d0e2c-102">С помощью этого метода приложение может отслеживать изменения drive и соответствующих дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-102">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="d0e2c-p101">Для начала приложение вызывает `delta` без параметров. Служба начинает перечислять иерархию диска, возвращая страницы элементов и `@odata.nextLink` или `@odata.deltaLink`, как показано ниже. Приложению следует выполнять вызовы с использованием `@odata.nextLink`, пока не будет возвращен отклик без `@odata.nextLink` или с пустым набором изменений.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="d0e2c-p102">Завершив получать изменения, вы можете применить их к локальному состоянию. Для проверки наличия изменений в будущем снова вызовите `delta` с использованием `@odata.deltaLink` из предыдущего отклика.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="d0e2c-p103">Удаленные элементы возвращаются с [аспектом `deleted`](../resources/deleted.md). Элементы с этим набором свойств следует удалить из локального состояния.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="d0e2c-110">**Примечание.** Локально удалять папку следует, только если после синхронизации всех изменений она пуста.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-110">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0e2c-111">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d0e2c-111">Prerequisites</span></span>
<span data-ttu-id="d0e2c-112">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="d0e2c-112">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="d0e2c-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="d0e2c-113">Files.Read</span></span>
* <span data-ttu-id="d0e2c-114">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-114">Files.ReadWrite</span></span>
* <span data-ttu-id="d0e2c-115">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0e2c-115">Files.Read.All</span></span>
* <span data-ttu-id="d0e2c-116">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0e2c-116">Files.ReadWrite.All</span></span>
* <span data-ttu-id="d0e2c-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0e2c-117">Sites.Read.All</span></span>
* <span data-ttu-id="d0e2c-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0e2c-118">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d0e2c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0e2c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/delta
GET /drives/{drive-id}/root/delta
GET /groups/{group-id}/drive/root/delta
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0e2c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d0e2c-120">Optional query parameters</span></span>
<span data-ttu-id="d0e2c-121">Этот метод поддерживает `$select`, `$expand` и `$top` [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-121">This method supports `$select`, `$expand`, and `$top` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="d0e2c-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0e2c-122">Request body</span></span>
<span data-ttu-id="d0e2c-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0e2c-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0e2c-124">Response</span></span>

<span data-ttu-id="d0e2c-125">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию ресурсов [DriveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-125">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="d0e2c-126">Помимо коллекции ресурсов DriveItem, отклик также включает одно из указанных ниже свойств.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-126">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="d0e2c-127">Имя</span><span class="sxs-lookup"><span data-stu-id="d0e2c-127">Name</span></span>                 | <span data-ttu-id="d0e2c-128">Значение</span><span class="sxs-lookup"><span data-stu-id="d0e2c-128">Value</span></span>  | <span data-ttu-id="d0e2c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d0e2c-129">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d0e2c-130">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="d0e2c-130">**@odata.nextLink**</span></span>  | <span data-ttu-id="d0e2c-131">url</span><span class="sxs-lookup"><span data-stu-id="d0e2c-131">url</span></span>    | <span data-ttu-id="d0e2c-132">URL-адрес для получения следующей доступной страницы изменений, если в текущем наборе есть дополнительные изменения.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-132">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="d0e2c-133">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="d0e2c-133">**@odata.deltaLink**</span></span> | <span data-ttu-id="d0e2c-134">url</span><span class="sxs-lookup"><span data-stu-id="d0e2c-134">url</span></span>    | <span data-ttu-id="d0e2c-p104">URL-адрес, возвращаемый вместо **@odata.nextLink** после возврата всех текущих изменений. Используется для считывания следующего набора изменений в будущем.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-p104">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |


## <a name="example-initial-request"></a><span data-ttu-id="d0e2c-137">Пример (первоначальный запрос)</span><span class="sxs-lookup"><span data-stu-id="d0e2c-137">Example (Initial Request)</span></span>
<span data-ttu-id="d0e2c-138">Ниже приведен пример вызова этого API для определения локального состояния.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-138">Here is an example of how to call this API to establish your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="d0e2c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0e2c-139">Request</span></span>
<span data-ttu-id="d0e2c-140">Ниже приведен пример первоначального запроса.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-140">Here is an example of the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

##### <a name="response"></a><span data-ttu-id="d0e2c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0e2c-141">Response</span></span>
<span data-ttu-id="d0e2c-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-142">Here is an example of the response.</span></span>

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
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        },
        {
            "id": "2353010204ddgg",
            "name": "file5.txt",
            "deleted": { }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/delta(token=1230919asd190410jlka)"
}
```

<span data-ttu-id="d0e2c-p105">Этот отклик включает первую страницу изменений, а свойство **@odata.nextLink** указывает, что в текущем наборе доступны дополнительные элементы. Ваше приложение должно запрашивать значение URL-адреса, указанного в свойстве **@odata.nextLink**, пока не будут получены все страницы элементов.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-p105">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="d0e2c-145">Пример (последняя страница в наборе)</span><span class="sxs-lookup"><span data-stu-id="d0e2c-145">Example (Last page in a set)</span></span>
<span data-ttu-id="d0e2c-146">Ниже приведен пример вызова этого API для обновления локального состояния.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-146">Here is an example of how to call this API to update your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="d0e2c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0e2c-147">Request</span></span>
<span data-ttu-id="d0e2c-148">Ниже приведен пример запроса, выполненного после первоначального.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-148">Here is an example request after the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

##### <a name="response"></a><span data-ttu-id="d0e2c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0e2c-149">Response</span></span>
<span data-ttu-id="d0e2c-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-150">Here is an example of the response.</span></span>

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
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { },
            "deleted": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?(token='1230919asd190410jlka')"
}
```

<span data-ttu-id="d0e2c-151">Такой отклик означает, что между отправками первоначального запроса и данного запроса (на обновление локального состояния) был удален элемент `folder2`, а элемент `file.txt` был добавлен или изменен.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-151">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="d0e2c-152">На последней странице элементов указано свойство **@odata.deltaLink**, содержащее URL-адрес, с помощью которого можно будет получить изменения относительно текущего набора элементов.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-152">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

## <a name="remarks"></a><span data-ttu-id="d0e2c-153">Заметки</span><span class="sxs-lookup"><span data-stu-id="d0e2c-153">Remarks</span></span>

* <span data-ttu-id="d0e2c-p106">В разностном канале показано последнее состояние каждого элемента, а не каждое изменение. Если элемент был переименован дважды, он будет указан только один раз, но с последним именем.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-p106">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="d0e2c-p107">По ряду причин один и тот же элемент может отображаться в разностном канале несколько раз. Следует использовать последний представленный вариант.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-p107">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="d0e2c-p108">Свойство `parentReference` элементов не включает значение **path**. Это вызвано тем, что при переименовании папки ее потомки не возвращаются с помощью **delta**. **При использовании delta следует всегда отслеживать элементы по идентификатору**.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-p108">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>

<span data-ttu-id="d0e2c-p109">В некоторых случаях службе не удается предоставить список изменений для определенного маркера (например, если клиент пытается повторно использовать старый маркер после долгого отключения, а также если из-за измененного состояния сервера требуется новый маркер). В таких случаях служба возвращает ошибку `HTTP 410 Gone` с откликом, содержащим один из представленных ниже кодов ошибок, и заголовком `Location`, содержащим новый аргумент nextLink, который начинает новое перечисление delta. По завершении полного перечисления сравните возвращенные элементы с локальным состоянием и выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-p109">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="d0e2c-164">Тип ошибки</span><span class="sxs-lookup"><span data-stu-id="d0e2c-164">Error Type</span></span>                       | <span data-ttu-id="d0e2c-165">Инструкции</span><span class="sxs-lookup"><span data-stu-id="d0e2c-165">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="d0e2c-p110">Замените все локальные элементы (в том числе удаленные) соответствующими элементами с сервера, если вы уверены, что при последней синхронизации в службу были внесены все локальные изменения. Отправьте все локальные изменения, не загруженные на сервер.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-p110">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="d0e2c-168">Отправьте все локальные элементы, не возвращенные службой, и все файлы, отличающиеся от соответствующих файлов на сервере (сохраняйте обе копии, если вы не знаете, какая из них более актуальна).</span><span class="sxs-lookup"><span data-stu-id="d0e2c-168">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |


<span data-ttu-id="d0e2c-p111">В OneDrive для бизнеса и SharePoint `delta` поддерживается только для папки `root`. Кроме того, не возвращаются следующие свойства ресурса DriveItem:</span><span class="sxs-lookup"><span data-stu-id="d0e2c-p111">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders. It also will not return the following DriveItem properties:</span></span>

* <span data-ttu-id="d0e2c-171">**createdBy**;</span><span class="sxs-lookup"><span data-stu-id="d0e2c-171">**createdBy**</span></span>
* <span data-ttu-id="d0e2c-172">**cTag**;</span><span class="sxs-lookup"><span data-stu-id="d0e2c-172">**cTag**</span></span>
* <span data-ttu-id="d0e2c-173">**eTag**;</span><span class="sxs-lookup"><span data-stu-id="d0e2c-173">**etag**</span></span>
* <span data-ttu-id="d0e2c-174">**fileSystemInfo**;</span><span class="sxs-lookup"><span data-stu-id="d0e2c-174">**fileSystemInfo**</span></span>
* <span data-ttu-id="d0e2c-175">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="d0e2c-175">**lastModifiedBy**</span></span>
* <span data-ttu-id="d0e2c-176">**parentReference**;</span><span class="sxs-lookup"><span data-stu-id="d0e2c-176">**parentReference**</span></span>
* <span data-ttu-id="d0e2c-177">**size**.</span><span class="sxs-lookup"><span data-stu-id="d0e2c-177">**size**</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "Get item delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
