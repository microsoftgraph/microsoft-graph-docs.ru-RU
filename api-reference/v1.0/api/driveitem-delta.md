---
author: JeremyKelley
ms.date: 09/10/2017
title: Синхронизация содержимого ресурса drive
localization_priority: Priority
ms.prod: sharepoint
description: С помощью этого метода приложение может отслеживать изменения drive и соответствующих дочерних элементов.
doc_type: apiPageType
ms.openlocfilehash: f247e643d29e0e7e4b601cbf284a94310c49b5d7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240355"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="459d1-103">Отслеживание изменений для Drive</span><span class="sxs-lookup"><span data-stu-id="459d1-103">Track changes for a Drive</span></span>

<span data-ttu-id="459d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="459d1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="459d1-105">С помощью этого метода приложение может отслеживать изменения drive и соответствующих дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="459d1-105">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="459d1-p101">Для начала приложение вызывает `delta` без параметров. Служба начинает перечислять иерархию диска, возвращая страницы элементов и `@odata.nextLink` или `@odata.deltaLink`, как показано ниже. Приложению следует выполнять вызовы с использованием `@odata.nextLink`, пока не будет возвращен отклик без `@odata.nextLink` или с пустым набором изменений.</span><span class="sxs-lookup"><span data-stu-id="459d1-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="459d1-p102">Завершив получать изменения, вы можете применить их к локальному состоянию. Для проверки наличия изменений в будущем снова вызовите `delta` с использованием `@odata.deltaLink` из предыдущего отклика.</span><span class="sxs-lookup"><span data-stu-id="459d1-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="459d1-p103">Удаленные элементы возвращаются с [аспектом `deleted`](../resources/deleted.md). Элементы с этим набором свойств следует удалить из локального состояния.</span><span class="sxs-lookup"><span data-stu-id="459d1-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

><span data-ttu-id="459d1-113">**Примечание.** Локально удалять папку следует, только если после синхронизации всех изменений она пуста.</span><span class="sxs-lookup"><span data-stu-id="459d1-113">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="459d1-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="459d1-114">Permissions</span></span>

<span data-ttu-id="459d1-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="459d1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="459d1-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="459d1-117">Permission type</span></span>      | <span data-ttu-id="459d1-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="459d1-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="459d1-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="459d1-119">Delegated (work or school account)</span></span> | <span data-ttu-id="459d1-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="459d1-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="459d1-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="459d1-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="459d1-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="459d1-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="459d1-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="459d1-123">Application</span></span> | <span data-ttu-id="459d1-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="459d1-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="459d1-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="459d1-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="459d1-126">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="459d1-126">Function parameters</span></span>

| <span data-ttu-id="459d1-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="459d1-127">Parameter</span></span>   | <span data-ttu-id="459d1-128">Тип</span><span class="sxs-lookup"><span data-stu-id="459d1-128">Type</span></span>  | <span data-ttu-id="459d1-129">Описание</span><span class="sxs-lookup"><span data-stu-id="459d1-129">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="459d1-130">token</span><span class="sxs-lookup"><span data-stu-id="459d1-130">token</span></span>  | <span data-ttu-id="459d1-131">string</span><span class="sxs-lookup"><span data-stu-id="459d1-131">string</span></span> | <span data-ttu-id="459d1-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="459d1-132">Optional.</span></span> <span data-ttu-id="459d1-133">Если не указан, перечисляет текущее состояние иерархии.</span><span class="sxs-lookup"><span data-stu-id="459d1-133">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="459d1-134">Если используется значение `latest`, возвращает пустой ответ с последним разностным маркером.</span><span class="sxs-lookup"><span data-stu-id="459d1-134">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="459d1-135">Если используется предыдущий разностный маркер, возвращает новое состояние с момента того маркера.</span><span class="sxs-lookup"><span data-stu-id="459d1-135">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="459d1-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="459d1-136">Optional query parameters</span></span>

<span data-ttu-id="459d1-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select`, `$expand` и `$top` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="459d1-137">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="459d1-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="459d1-138">Response</span></span>

<span data-ttu-id="459d1-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию ресурсов [DriveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="459d1-139">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="459d1-140">Помимо коллекции ресурсов DriveItem, отклик также включает одно из указанных ниже свойств.</span><span class="sxs-lookup"><span data-stu-id="459d1-140">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="459d1-141">Имя</span><span class="sxs-lookup"><span data-stu-id="459d1-141">Name</span></span>                 | <span data-ttu-id="459d1-142">Значение</span><span class="sxs-lookup"><span data-stu-id="459d1-142">Value</span></span>  | <span data-ttu-id="459d1-143">Описание</span><span class="sxs-lookup"><span data-stu-id="459d1-143">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="459d1-144">**\@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="459d1-144">**\@odata.nextLink**</span></span>  | <span data-ttu-id="459d1-145">url</span><span class="sxs-lookup"><span data-stu-id="459d1-145">url</span></span>    | <span data-ttu-id="459d1-146">URL-адрес для получения следующей доступной страницы изменений, если в текущем наборе есть дополнительные изменения.</span><span class="sxs-lookup"><span data-stu-id="459d1-146">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="459d1-147">**\@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="459d1-147">**\@odata.deltaLink**</span></span> | <span data-ttu-id="459d1-148">url</span><span class="sxs-lookup"><span data-stu-id="459d1-148">url</span></span>    | <span data-ttu-id="459d1-149">URL-адрес, возвращаемый вместо **\@odata.nextLink** после возврата всех текущих изменений.</span><span class="sxs-lookup"><span data-stu-id="459d1-149">A URL returned instead of **\@odata.nextLink** after all current changes have been returned.</span></span> <span data-ttu-id="459d1-150">Используется для считывания следующего набора изменений в будущем.</span><span class="sxs-lookup"><span data-stu-id="459d1-150">Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="459d1-151">Пример (первоначальный запрос)</span><span class="sxs-lookup"><span data-stu-id="459d1-151">Example (Initial Request)</span></span>

<span data-ttu-id="459d1-152">Ниже приведен пример вызова этого API для определения локального состояния.</span><span class="sxs-lookup"><span data-stu-id="459d1-152">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="459d1-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="459d1-153">Request</span></span>

<span data-ttu-id="459d1-154">Ниже приведен пример первоначального запроса.</span><span class="sxs-lookup"><span data-stu-id="459d1-154">Here is an example of the initial request.</span></span>


# <a name="http"></a>[<span data-ttu-id="459d1-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="459d1-155">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_first", "tags": "service.graph" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```
# <a name="c"></a>[<span data-ttu-id="459d1-156">C#</span><span class="sxs-lookup"><span data-stu-id="459d1-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-first-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="459d1-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="459d1-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-first-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="459d1-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="459d1-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-first-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="459d1-159">Java</span><span class="sxs-lookup"><span data-stu-id="459d1-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-first-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="459d1-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="459d1-160">Response</span></span>

<span data-ttu-id="459d1-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="459d1-161">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true, "scope": "file.read" } -->

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

<span data-ttu-id="459d1-162">Этот отклик включает первую страницу изменений, а свойство **\@odata.nextLink** указывает, что в текущем наборе доступны дополнительные элементы.</span><span class="sxs-lookup"><span data-stu-id="459d1-162">This response includes the first page of changes, and the **\@odata.nextLink** property indicates that there are more items available in the current set of items.</span></span>
<span data-ttu-id="459d1-163">Ваше приложение должно запрашивать значение URL-адреса, указанного в свойстве **\@odata.nextLink**, пока не будут восстановлены все страницы элементов.</span><span class="sxs-lookup"><span data-stu-id="459d1-163">Your app should continue to request the URL value of **\@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="459d1-164">Пример (последняя страница в наборе)</span><span class="sxs-lookup"><span data-stu-id="459d1-164">Example (Last page in a set)</span></span>

<span data-ttu-id="459d1-165">Ниже приведен пример вызова этого API для обновления локального состояния.</span><span class="sxs-lookup"><span data-stu-id="459d1-165">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="459d1-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="459d1-166">Request</span></span>

<span data-ttu-id="459d1-167">Ниже приведен пример запроса, выполненного после первоначального.</span><span class="sxs-lookup"><span data-stu-id="459d1-167">Here is an example request after the initial request.</span></span>


# <a name="http"></a>[<span data-ttu-id="459d1-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="459d1-168">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-delta-last", "tags": "service.graph" }-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```
# <a name="c"></a>[<span data-ttu-id="459d1-169">C#</span><span class="sxs-lookup"><span data-stu-id="459d1-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-last-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="459d1-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="459d1-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-last-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="459d1-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="459d1-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-last-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="459d1-172">Java</span><span class="sxs-lookup"><span data-stu-id="459d1-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-last-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="459d1-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="459d1-173">Response</span></span>

<span data-ttu-id="459d1-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="459d1-174">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)", "scope": "file.read" } -->

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

<span data-ttu-id="459d1-175">Такой отклик означает, что между отправками первоначального запроса и данного запроса (на обновление локального состояния) был удален элемент `folder2`, а элемент `file.txt` был добавлен или изменен.</span><span class="sxs-lookup"><span data-stu-id="459d1-175">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="459d1-176">Последняя страница элементов включает свойство **\@odata.deltaLink**, содержащее URL-адрес, с помощью которого можно в дальнейшем восстановить изменения относительно текущего набора элементов.</span><span class="sxs-lookup"><span data-stu-id="459d1-176">The final page of items will include the **\@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="459d1-p108">В некоторых случаях службе не удается предоставить список изменений для определенного маркера (например, если клиент пытается повторно использовать старый маркер после долгого отключения, а также если из-за измененного состояния сервера требуется новый маркер). В таких случаях служба возвращает ошибку `HTTP 410 Gone` с откликом, содержащим один из представленных ниже кодов ошибок, и заголовком `Location`, содержащим новый аргумент nextLink, который начинает новое перечисление delta. По завершении полного перечисления сравните возвращенные элементы с локальным состоянием и выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="459d1-p108">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="459d1-180">Тип ошибки</span><span class="sxs-lookup"><span data-stu-id="459d1-180">Error Type</span></span>                       | <span data-ttu-id="459d1-181">Инструкции</span><span class="sxs-lookup"><span data-stu-id="459d1-181">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="459d1-p109">Замените все локальные элементы (в том числе удаленные) соответствующими элементами с сервера, если вы уверены, что при последней синхронизации в службу были внесены все локальные изменения. Отправьте все локальные изменения, не загруженные на сервер.</span><span class="sxs-lookup"><span data-stu-id="459d1-p109">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="459d1-184">Отправьте все локальные элементы, не возвращенные службой, и все файлы, отличающиеся от соответствующих файлов на сервере (сохраняйте обе копии, если вы не знаете, какая из них более актуальна).</span><span class="sxs-lookup"><span data-stu-id="459d1-184">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="459d1-185">Получение текущего значения deltaLink</span><span class="sxs-lookup"><span data-stu-id="459d1-185">Retrieving the current deltaLink</span></span>

<span data-ttu-id="459d1-186">В некоторых случаях может быть удобно запросить текущее значение deltaLink, не перечисляя перед этим все элементы, уже хранящиеся в объекте drive.</span><span class="sxs-lookup"><span data-stu-id="459d1-186">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="459d1-187">Это может быть полезно, если приложению достаточно узнать об изменениях и ему не нужны сведения о существующих элементах.</span><span class="sxs-lookup"><span data-stu-id="459d1-187">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items.</span></span>
<span data-ttu-id="459d1-188">Чтобы получить последнее значение deltaLink, вызовите функцию `delta` с параметром `?token=latest` в строке запроса.</span><span class="sxs-lookup"><span data-stu-id="459d1-188">To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="459d1-189">**Примечание. Если вы пытаетесь поддерживать полное локальное представление элементов в папке или на диске, необходимо использовать `delta` для исходного перечисления. Другие подходы, например постраничный просмотр коллекции `children` для папки, не гарантируют возврата всех элементов, если во время перечисления выполняются операции записи. Только с помощью функции `delta` можно гарантировать, что считываются все необходимые данные.**</span><span class="sxs-lookup"><span data-stu-id="459d1-189">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="459d1-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="459d1-190">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="459d1-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="459d1-191">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-latest", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```msgraph-interactive
GET /me/drive/root/delta?token=latest
```
# <a name="c"></a>[<span data-ttu-id="459d1-192">C#</span><span class="sxs-lookup"><span data-stu-id="459d1-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-latest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="459d1-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="459d1-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-latest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="459d1-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="459d1-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-latest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="459d1-195">Java</span><span class="sxs-lookup"><span data-stu-id="459d1-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-latest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="459d1-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="459d1-196">Response</span></span>

<!-- { "blockType": "response", "isEmpty": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="459d1-197">Примечания</span><span class="sxs-lookup"><span data-stu-id="459d1-197">Remarks</span></span>

* <span data-ttu-id="459d1-p111">В разностном канале показано последнее состояние каждого элемента, а не каждое изменение. Если элемент был переименован дважды, он будет указан только один раз, но с последним именем.</span><span class="sxs-lookup"><span data-stu-id="459d1-p111">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="459d1-p112">По ряду причин один и тот же элемент может отображаться в разностном канале несколько раз. Следует использовать последний представленный вариант.</span><span class="sxs-lookup"><span data-stu-id="459d1-p112">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="459d1-p113">Свойство `parentReference` элементов не включает значение **path**. Это вызвано тем, что при переименовании папки ее потомки не возвращаются с помощью **delta**. **При использовании delta следует всегда отслеживать элементы по идентификатору**.</span><span class="sxs-lookup"><span data-stu-id="459d1-p113">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="459d1-205">В OneDrive для бизнеса и SharePoint функция `delta` поддерживается только для папки `root`.</span><span class="sxs-lookup"><span data-stu-id="459d1-205">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders within a drive.</span></span>

* <span data-ttu-id="459d1-206">Запрос изменений не возвращает некоторые свойства DriveItem, в зависимости от типа операции и службы, как показано в таблицах ниже.</span><span class="sxs-lookup"><span data-stu-id="459d1-206">Delta query will not return some DriveItem properties, depending on the operation and service type, as shown in the following tables.</span></span>

    <span data-ttu-id="459d1-207">**OneDrive для бизнеса**</span><span class="sxs-lookup"><span data-stu-id="459d1-207">**OneDrive for Business**</span></span>
    
    | <span data-ttu-id="459d1-208">Тип операции</span><span class="sxs-lookup"><span data-stu-id="459d1-208">Operation type</span></span> | <span data-ttu-id="459d1-209">Свойства, опущенные запросом изменений</span><span class="sxs-lookup"><span data-stu-id="459d1-209">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="459d1-210">Создание или изменение</span><span class="sxs-lookup"><span data-stu-id="459d1-210">Create/Modify</span></span> | <span data-ttu-id="459d1-211">`ctag`, `lastModifiedBy`</span><span class="sxs-lookup"><span data-stu-id="459d1-211">`ctag`, `lastModifiedBy`</span></span> |
    | <span data-ttu-id="459d1-212">Удаление</span><span class="sxs-lookup"><span data-stu-id="459d1-212">Delete</span></span> | <span data-ttu-id="459d1-213">`ctag`, `lastModifiedBy`, `name`</span><span class="sxs-lookup"><span data-stu-id="459d1-213">`ctag`, `lastModifiedBy`, `name`</span></span> |


    <span data-ttu-id="459d1-214">**OneDrive (для потребителей)**</span><span class="sxs-lookup"><span data-stu-id="459d1-214">**OneDrive (consumer)**</span></span>
    
    | <span data-ttu-id="459d1-215">Тип операции</span><span class="sxs-lookup"><span data-stu-id="459d1-215">Operation type</span></span> | <span data-ttu-id="459d1-216">Свойства, опущенные запросом изменений</span><span class="sxs-lookup"><span data-stu-id="459d1-216">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="459d1-217">Создание или изменение</span><span class="sxs-lookup"><span data-stu-id="459d1-217">Create/Modify</span></span> | <span data-ttu-id="459d1-218">н/д</span><span class="sxs-lookup"><span data-stu-id="459d1-218">n/a</span></span> |
    | <span data-ttu-id="459d1-219">Удаление</span><span class="sxs-lookup"><span data-stu-id="459d1-219">Delete</span></span> | <span data-ttu-id="459d1-220">`ctag`, `size`</span><span class="sxs-lookup"><span data-stu-id="459d1-220">`ctag`, `size`</span></span> |

## <a name="scanning-permissions-hierarchies"></a><span data-ttu-id="459d1-221">Сканирование иерархии разрешений</span><span class="sxs-lookup"><span data-stu-id="459d1-221">Scanning permissions hierarchies</span></span>
<span data-ttu-id="459d1-222">По умолчанию ответ на запрос изменений включает информацию об общем доступе для всех изменившихся элементов в запросе, даже если они наследуют разрешения от родительского элемента и сами непосредственно не имеют изменений общего доступа.</span><span class="sxs-lookup"><span data-stu-id="459d1-222">By default, the delta query response will include sharing information for all items in the query that changed even if they inherit their permissions from their parent and did not have direct sharing changes themselves.</span></span> <span data-ttu-id="459d1-223">Обычно за этим следует дополнительный запрос на получение сведений о разрешениях для каждого элемента, а не только для тех, которые имеют изменения общего доступа.</span><span class="sxs-lookup"><span data-stu-id="459d1-223">This typically then results in a follow up call to get the permission details for every item rather than just the ones whose sharing information changed.</span></span> <span data-ttu-id="459d1-224">Чтобы получить более детальные сведения о произошедших изменениях разрешений, добавьте в запрос заголовок `Prefer: hierarchicalsharing`.</span><span class="sxs-lookup"><span data-stu-id="459d1-224">You can optimize your understanding of how permission changes happen by adding the `Prefer: hierarchicalsharing` header to your delta query request.</span></span>

<span data-ttu-id="459d1-225">При наличии заголовка `Prefer: hierarchicalsharing` возвращается информация об общем доступе для корневого элемента иерархии разрешений, а также для элементов с изменениями общего доступа.</span><span class="sxs-lookup"><span data-stu-id="459d1-225">When the `Prefer: hierarchicalsharing` header is provided, sharing information will be returned for the root of the permissions hierarchy, as well as items that explicitly have sharing changes.</span></span> <span data-ttu-id="459d1-226">В случае когда изменения состоят в отмене общего доступа для элемента, отображается пустой аспект общего доступа, что позволяет отличать элементы, наследующие разрешения от родителя, и уникальные элементы, не имеющие ссылок для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="459d1-226">In cases where the sharing change is to remove sharing from an item, you will find an empty sharing facet to differentiate between items that inherit from their parent and those that are unique but have no sharing links.</span></span> <span data-ttu-id="459d1-227">Пустой аспект общего доступа также отображается для корневого элемента иерархии разрешений, который не имеет общего доступа.</span><span class="sxs-lookup"><span data-stu-id="459d1-227">You will also see this empty sharing facet on the root of a permission hierarchy that is not shared to establish the initial scope.</span></span>

<span data-ttu-id="459d1-228">Во многих сценариях сканирования интерес представляют именно изменения разрешений.</span><span class="sxs-lookup"><span data-stu-id="459d1-228">In many scanning scenarios, you might be interested specifically in changes to permissions.</span></span> <span data-ttu-id="459d1-229">Чтобы получить сведения о том, какие изменения являются следствием изменений разрешений, можно использовать в запросе заголовок `Prefer: deltashowsharingchanges`.</span><span class="sxs-lookup"><span data-stu-id="459d1-229">To make it clear in the delta query response which changes are the result of permissions being changed, you can provide the `Prefer: deltashowsharingchanges` header.</span></span> <span data-ttu-id="459d1-230">В этом случае для всех элементов, включенных в ответ на запрос в связи с изменениями разрешений, будет отображаться примечание OData `@microsoft.graph.sharedChanged":"True"`.</span><span class="sxs-lookup"><span data-stu-id="459d1-230">When this header is provided, all items that appear in the delta query response due to permission changes will have the `@microsoft.graph.sharedChanged":"True"` OData annotation.</span></span> <span data-ttu-id="459d1-231">Эта функция применима к SharePoint и OneDrive для бизнеса, но не к личным учетным записям OneDrive.</span><span class="sxs-lookup"><span data-stu-id="459d1-231">This feature is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

> <span data-ttu-id="459d1-232">**Примечание.** При включении в запрос заголовка `Prefer: deltashowsharingchanges` требуется использовать `Prefer: deltashowremovedasdeleted` и `Prefer: deltatraversepermissiongaps`.</span><span class="sxs-lookup"><span data-stu-id="459d1-232">**Note:** The use of `Prefer: deltashowsharingchanges` header requires you to use `Prefer: deltashowremovedasdeleted` and `Prefer: deltatraversepermissiongaps`.</span></span> <span data-ttu-id="459d1-233">Эти значения заголовка можно объединить в один общий заголовок: `Prefer: deltashowremovedasdeleted, deltatraversepermissiongaps, deltashowsharingchanges`.</span><span class="sxs-lookup"><span data-stu-id="459d1-233">These header values can be joined together in a single header: `Prefer: deltashowremovedasdeleted, deltatraversepermissiongaps, deltashowsharingchanges`.</span></span>

## <a name="error-responses"></a><span data-ttu-id="459d1-234">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="459d1-234">Error responses</span></span>

<span data-ttu-id="459d1-235">Помимо вышеописанных ошибок повторной синхронизации, в статье [Ответы с ошибками][error-response] представлены сведения о том, как возвращаются ошибки.</span><span class="sxs-lookup"><span data-stu-id="459d1-235">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": [
  ]
} -->

