---
author: JeremyKelley
description: С помощью этого метода приложение может отслеживать изменения drive и соответствующих дочерних элементов.
ms.date: 09/10/2017
title: Синхронизация содержимого ресурса drive
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 05fd3409d18ad872a4b61d55e1aa66f6a4f44c85
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416825"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="7cccb-103">Отслеживание изменений для Drive</span><span class="sxs-lookup"><span data-stu-id="7cccb-103">Track changes for a Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cccb-104">С помощью этого метода приложение может отслеживать изменения drive и соответствующих дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="7cccb-104">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="7cccb-p101">Для начала приложение вызывает `delta` без параметров. Служба начинает перечислять иерархию диска, возвращая страницы элементов и `@odata.nextLink` или `@odata.deltaLink`, как показано ниже. Приложению следует выполнять вызовы с использованием `@odata.nextLink`, пока не будет возвращен отклик без `@odata.nextLink` или с пустым набором изменений.</span><span class="sxs-lookup"><span data-stu-id="7cccb-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="7cccb-p102">Завершив получать изменения, вы можете применить их к локальному состоянию. Для проверки наличия изменений в будущем снова вызовите `delta` с использованием `@odata.deltaLink` из предыдущего отклика.</span><span class="sxs-lookup"><span data-stu-id="7cccb-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="7cccb-p103">Удаленные элементы возвращаются с [аспектом `deleted`](../resources/deleted.md). Элементы с этим набором свойств следует удалить из локального состояния.</span><span class="sxs-lookup"><span data-stu-id="7cccb-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="7cccb-112">**Примечание.** Локально удалять папку следует, только если после синхронизации всех изменений она пуста.</span><span class="sxs-lookup"><span data-stu-id="7cccb-112">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cccb-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7cccb-113">Permissions</span></span>

<span data-ttu-id="7cccb-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cccb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cccb-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cccb-116">Permission type</span></span>      | <span data-ttu-id="7cccb-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cccb-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cccb-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cccb-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7cccb-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cccb-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7cccb-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cccb-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cccb-121">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cccb-121">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7cccb-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cccb-122">Application</span></span> | <span data-ttu-id="7cccb-123">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cccb-123">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cccb-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cccb-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="7cccb-125">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="7cccb-125">Function parameters</span></span>

| <span data-ttu-id="7cccb-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="7cccb-126">Parameter</span></span>   | <span data-ttu-id="7cccb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7cccb-127">Type</span></span>  | <span data-ttu-id="7cccb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7cccb-128">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7cccb-129">token</span><span class="sxs-lookup"><span data-stu-id="7cccb-129">token</span></span>  | <span data-ttu-id="7cccb-130">string</span><span class="sxs-lookup"><span data-stu-id="7cccb-130">string</span></span> | <span data-ttu-id="7cccb-131">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7cccb-131">Optional.</span></span> <span data-ttu-id="7cccb-132">Если не указан, перечисляет текущее состояние иерархии.</span><span class="sxs-lookup"><span data-stu-id="7cccb-132">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="7cccb-133">Если используется значение `latest`, возвращает пустой ответ с последним разностным маркером.</span><span class="sxs-lookup"><span data-stu-id="7cccb-133">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="7cccb-134">Если используется предыдущий разностный маркер, возвращает новое состояние с момента того маркера.</span><span class="sxs-lookup"><span data-stu-id="7cccb-134">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="7cccb-135">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7cccb-135">Optional query parameters</span></span>

<span data-ttu-id="7cccb-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select`, `$expand` и `$top` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7cccb-136">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="7cccb-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cccb-137">Response</span></span>

<span data-ttu-id="7cccb-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию ресурсов [DriveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7cccb-138">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="7cccb-139">Помимо коллекции ресурсов DriveItem, отклик также включает одно из указанных ниже свойств.</span><span class="sxs-lookup"><span data-stu-id="7cccb-139">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="7cccb-140">Имя</span><span class="sxs-lookup"><span data-stu-id="7cccb-140">Name</span></span>                 | <span data-ttu-id="7cccb-141">Значение</span><span class="sxs-lookup"><span data-stu-id="7cccb-141">Value</span></span>  | <span data-ttu-id="7cccb-142">Описание</span><span class="sxs-lookup"><span data-stu-id="7cccb-142">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7cccb-143">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="7cccb-143">**@odata.nextLink**</span></span>  | <span data-ttu-id="7cccb-144">url</span><span class="sxs-lookup"><span data-stu-id="7cccb-144">url</span></span>    | <span data-ttu-id="7cccb-145">URL-адрес для получения следующей доступной страницы изменений, если в текущем наборе есть дополнительные изменения.</span><span class="sxs-lookup"><span data-stu-id="7cccb-145">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="7cccb-146">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="7cccb-146">**@odata.deltaLink**</span></span> | <span data-ttu-id="7cccb-147">url</span><span class="sxs-lookup"><span data-stu-id="7cccb-147">url</span></span>    | <span data-ttu-id="7cccb-p106">URL-адрес, возвращаемый вместо **@odata.nextLink** после возврата всех текущих изменений. Используется для считывания следующего набора изменений в будущем.</span><span class="sxs-lookup"><span data-stu-id="7cccb-p106">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="7cccb-150">Пример (первоначальный запрос)</span><span class="sxs-lookup"><span data-stu-id="7cccb-150">Example (Initial Request)</span></span>

<span data-ttu-id="7cccb-151">Ниже приведен пример вызова этого API для определения локального состояния.</span><span class="sxs-lookup"><span data-stu-id="7cccb-151">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="7cccb-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cccb-152">Request</span></span>

<span data-ttu-id="7cccb-153">Ниже приведен пример первоначального запроса.</span><span class="sxs-lookup"><span data-stu-id="7cccb-153">Here is an example of the initial request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7cccb-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cccb-154">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_first" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/root/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7cccb-155">C#</span><span class="sxs-lookup"><span data-stu-id="7cccb-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-first-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7cccb-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cccb-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-first-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7cccb-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7cccb-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-first-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7cccb-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cccb-158">Response</span></span>

<span data-ttu-id="7cccb-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7cccb-159">Here is an example of the response.</span></span>

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

<span data-ttu-id="7cccb-p107">Этот отклик включает первую страницу изменений, а свойство **@odata.nextLink** указывает, что в текущем наборе доступны дополнительные элементы. Ваше приложение должно запрашивать значение URL-адреса, указанного в свойстве **@odata.nextLink**, пока не будут получены все страницы элементов.</span><span class="sxs-lookup"><span data-stu-id="7cccb-p107">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="7cccb-162">Пример (последняя страница в наборе)</span><span class="sxs-lookup"><span data-stu-id="7cccb-162">Example (Last page in a set)</span></span>

<span data-ttu-id="7cccb-163">Ниже приведен пример вызова этого API для обновления локального состояния.</span><span class="sxs-lookup"><span data-stu-id="7cccb-163">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="7cccb-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cccb-164">Request</span></span>

<span data-ttu-id="7cccb-165">Ниже приведен пример запроса, выполненного после первоначального.</span><span class="sxs-lookup"><span data-stu-id="7cccb-165">Here is an example request after the initial request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7cccb-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cccb-166">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_last" }-->

```http
GET https://graph.microsoft.com/beta/me/drive/root/delta(token='1230919asd190410jlka')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7cccb-167">C#</span><span class="sxs-lookup"><span data-stu-id="7cccb-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-last-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7cccb-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cccb-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-last-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7cccb-169">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7cccb-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-last-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7cccb-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cccb-170">Response</span></span>

<span data-ttu-id="7cccb-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7cccb-171">Here is an example of the response.</span></span>

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

<span data-ttu-id="7cccb-172">Такой отклик означает, что между отправками первоначального запроса и данного запроса (на обновление локального состояния) был удален элемент `folder2`, а элемент `file.txt` был добавлен или изменен.</span><span class="sxs-lookup"><span data-stu-id="7cccb-172">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="7cccb-173">На последней странице элементов указано свойство **@odata.deltaLink**, содержащее URL-адрес, с помощью которого можно будет получить изменения относительно текущего набора элементов.</span><span class="sxs-lookup"><span data-stu-id="7cccb-173">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="7cccb-p108">В некоторых случаях службе не удается предоставить список изменений для определенного маркера (например, если клиент пытается повторно использовать старый маркер после долгого отключения, а также если из-за измененного состояния сервера требуется новый маркер). В таких случаях служба возвращает ошибку `HTTP 410 Gone` с откликом, содержащим один из представленных ниже кодов ошибок, и заголовком `Location`, содержащим новый аргумент nextLink, который начинает новое перечисление delta. По завершении полного перечисления сравните возвращенные элементы с локальным состоянием и выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="7cccb-p108">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="7cccb-177">Тип ошибки</span><span class="sxs-lookup"><span data-stu-id="7cccb-177">Error Type</span></span>                       | <span data-ttu-id="7cccb-178">Инструкции</span><span class="sxs-lookup"><span data-stu-id="7cccb-178">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="7cccb-p109">Замените все локальные элементы (в том числе удаленные) соответствующими элементами с сервера, если вы уверены, что при последней синхронизации в службу были внесены все локальные изменения. Отправьте все локальные изменения, не загруженные на сервер.</span><span class="sxs-lookup"><span data-stu-id="7cccb-p109">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="7cccb-181">Отправьте все локальные элементы, не возвращенные службой, и все файлы, отличающиеся от соответствующих файлов на сервере (сохраняйте обе копии, если вы не знаете, какая из них более актуальна).</span><span class="sxs-lookup"><span data-stu-id="7cccb-181">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="7cccb-182">Получение текущего значения deltaLink</span><span class="sxs-lookup"><span data-stu-id="7cccb-182">Retrieving the current deltaLink</span></span>

<span data-ttu-id="7cccb-183">В некоторых случаях может быть удобно запросить текущее значение deltaLink, не перечисляя перед этим все элементы, уже хранящиеся в объекте drive.</span><span class="sxs-lookup"><span data-stu-id="7cccb-183">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="7cccb-184">Это может быть полезно, если приложению достаточно узнать об изменениях и ему не нужны сведения о существующих элементах.</span><span class="sxs-lookup"><span data-stu-id="7cccb-184">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items.</span></span>
<span data-ttu-id="7cccb-185">Чтобы получить последнее значение deltaLink, вызовите функцию `delta` с параметром `?token=latest` в строке запроса.</span><span class="sxs-lookup"><span data-stu-id="7cccb-185">To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="7cccb-186">**Примечание. Если вы пытаетесь поддерживать полное локальное представление элементов в папке или на диске, необходимо использовать `delta` для исходного перечисления. Другие подходы, например постраничный просмотр коллекции `children` для папки, не гарантируют возврата всех элементов, если во время перечисления выполняются операции записи. Только с помощью функции `delta` можно гарантировать, что считываются все необходимые данные.**</span><span class="sxs-lookup"><span data-stu-id="7cccb-186">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="7cccb-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cccb-187">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7cccb-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cccb-188">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "files.read", "target": "action" } -->

```http
GET /me/drive/root/delta?token=latest
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7cccb-189">C#</span><span class="sxs-lookup"><span data-stu-id="7cccb-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-latest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7cccb-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cccb-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-latest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7cccb-191">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7cccb-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-latest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7cccb-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cccb-192">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="7cccb-193">Примечания</span><span class="sxs-lookup"><span data-stu-id="7cccb-193">Remarks</span></span>

* <span data-ttu-id="7cccb-p111">В разностном канале показано последнее состояние каждого элемента, а не каждое изменение. Если элемент был переименован дважды, он будет указан только один раз, но с последним именем.</span><span class="sxs-lookup"><span data-stu-id="7cccb-p111">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="7cccb-p112">По ряду причин один и тот же элемент может отображаться в разностном канале несколько раз. Следует использовать последний представленный вариант.</span><span class="sxs-lookup"><span data-stu-id="7cccb-p112">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="7cccb-p113">Свойство `parentReference` элементов не включает значение **path**. Это вызвано тем, что при переименовании папки ее потомки не возвращаются с помощью **delta**. **При использовании delta следует всегда отслеживать элементы по идентификатору**.</span><span class="sxs-lookup"><span data-stu-id="7cccb-p113">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="7cccb-201">В OneDrive для бизнеса и SharePoint функция `delta` поддерживается только для папки `root`.</span><span class="sxs-lookup"><span data-stu-id="7cccb-201">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders within a drive.</span></span>

* <span data-ttu-id="7cccb-202">Запрос изменений не возвращает некоторые свойства DriveItem, в зависимости от типа операции и службы, как показано в таблицах ниже.</span><span class="sxs-lookup"><span data-stu-id="7cccb-202">Delta query will not return some DriveItem properties, depending on the operation and service type, as shown in the following tables.</span></span>

    <span data-ttu-id="7cccb-203">**OneDrive для бизнеса**</span><span class="sxs-lookup"><span data-stu-id="7cccb-203">**OneDrive for Business**</span></span>
    
    | <span data-ttu-id="7cccb-204">Тип операции</span><span class="sxs-lookup"><span data-stu-id="7cccb-204">Operation type</span></span> | <span data-ttu-id="7cccb-205">Свойства, опущенные запросом изменений</span><span class="sxs-lookup"><span data-stu-id="7cccb-205">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="7cccb-206">Создание или изменение</span><span class="sxs-lookup"><span data-stu-id="7cccb-206">Create/Modify</span></span> | <span data-ttu-id="7cccb-207">`ctag`, `lastModifiedBy`</span><span class="sxs-lookup"><span data-stu-id="7cccb-207"></span></span> |
    | <span data-ttu-id="7cccb-208">Удаление</span><span class="sxs-lookup"><span data-stu-id="7cccb-208">Delete</span></span> | <span data-ttu-id="7cccb-209">`ctag`, `lastModifiedBy`, `name`</span><span class="sxs-lookup"><span data-stu-id="7cccb-209"></span></span> |


    <span data-ttu-id="7cccb-210">**OneDrive (для потребителей)**</span><span class="sxs-lookup"><span data-stu-id="7cccb-210">**OneDrive (consumer)**</span></span>
    
    | <span data-ttu-id="7cccb-211">Тип операции</span><span class="sxs-lookup"><span data-stu-id="7cccb-211">Operation type</span></span> | <span data-ttu-id="7cccb-212">Свойства, опущенные запросом изменений</span><span class="sxs-lookup"><span data-stu-id="7cccb-212">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="7cccb-213">Создание или изменение</span><span class="sxs-lookup"><span data-stu-id="7cccb-213">Create/Modify</span></span> | <span data-ttu-id="7cccb-214">н/д</span><span class="sxs-lookup"><span data-stu-id="7cccb-214">n/a</span></span> |
    | <span data-ttu-id="7cccb-215">Удаление</span><span class="sxs-lookup"><span data-stu-id="7cccb-215">Delete</span></span> | <span data-ttu-id="7cccb-216">`ctag`, `size`</span><span class="sxs-lookup"><span data-stu-id="7cccb-216"></span></span> |

## <a name="error-responses"></a><span data-ttu-id="7cccb-217">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="7cccb-217">Error responses</span></span>

<span data-ttu-id="7cccb-218">Помимо вышеописанных ошибок повторной синхронизации, в статье [Ошибки][error-response] представлены сведения о том, как возвращаются ошибки.</span><span class="sxs-lookup"><span data-stu-id="7cccb-218">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": [
  ]
}
-->
