---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Синхронизация содержимого ресурса drive
ms.openlocfilehash: b16787a3939d514e3c84ea0f06b562cd3c689e76
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748432"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="e1391-102">Отслеживание изменений для Drive</span><span class="sxs-lookup"><span data-stu-id="e1391-102">Track changes for a Drive</span></span>

> <span data-ttu-id="e1391-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e1391-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1391-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1391-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1391-105">С помощью этого метода приложение может отслеживать изменения drive и соответствующих дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="e1391-105">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="e1391-p102">Для начала приложение вызывает `delta` без параметров. Служба начинает перечислять иерархию диска, возвращая страницы элементов и `@odata.nextLink` или `@odata.deltaLink`, как показано ниже. Приложению следует выполнять вызовы с использованием `@odata.nextLink`, пока не будет возвращен отклик без `@odata.nextLink` или с пустым набором изменений.</span><span class="sxs-lookup"><span data-stu-id="e1391-p102">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="e1391-p103">Завершив получать изменения, вы можете применить их к локальному состоянию. Для проверки наличия изменений в будущем снова вызовите `delta` с использованием `@odata.deltaLink` из предыдущего отклика.</span><span class="sxs-lookup"><span data-stu-id="e1391-p103">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="e1391-p104">Удаленные элементы возвращаются с [аспектом `deleted`](../resources/deleted.md). Элементы с этим набором свойств следует удалить из локального состояния.</span><span class="sxs-lookup"><span data-stu-id="e1391-p104">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="e1391-113">**Примечание.** Локально удалять папку следует, только если после синхронизации всех изменений она пуста.</span><span class="sxs-lookup"><span data-stu-id="e1391-113">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1391-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1391-114">Permissions</span></span>

<span data-ttu-id="e1391-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1391-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1391-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1391-117">Permission type</span></span>      | <span data-ttu-id="e1391-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1391-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1391-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1391-119">Delegated (work or school account)</span></span> | <span data-ttu-id="e1391-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1391-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1391-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1391-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1391-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1391-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1391-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1391-123">Application</span></span> | <span data-ttu-id="e1391-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1391-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1391-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1391-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="e1391-126">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="e1391-126">Function parameters</span></span>

| <span data-ttu-id="e1391-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="e1391-127">Parameter</span></span>   | <span data-ttu-id="e1391-128">Тип</span><span class="sxs-lookup"><span data-stu-id="e1391-128">Type</span></span>  | <span data-ttu-id="e1391-129">Описание</span><span class="sxs-lookup"><span data-stu-id="e1391-129">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e1391-130">токен</span><span class="sxs-lookup"><span data-stu-id="e1391-130">token</span></span>  | <span data-ttu-id="e1391-131">string</span><span class="sxs-lookup"><span data-stu-id="e1391-131">string</span></span> | <span data-ttu-id="e1391-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e1391-132">Optional.</span></span> <span data-ttu-id="e1391-133">Если не указано, перечисляет текущее состояние иерархии.</span><span class="sxs-lookup"><span data-stu-id="e1391-133">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="e1391-134">Если `latest`, возвращается пустая ответа с последнего разностного маркер.</span><span class="sxs-lookup"><span data-stu-id="e1391-134">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="e1391-135">Если маркер предыдущей дельты возвращает новое состояние с момента маркер.</span><span class="sxs-lookup"><span data-stu-id="e1391-135">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="e1391-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e1391-136">Optional query parameters</span></span>

<span data-ttu-id="e1391-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select`, `$expand` и `$top` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e1391-137">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="e1391-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1391-138">Response</span></span>

<span data-ttu-id="e1391-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию ресурсов [DriveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e1391-139">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="e1391-140">Помимо коллекции ресурсов DriveItem, отклик также включает одно из указанных ниже свойств.</span><span class="sxs-lookup"><span data-stu-id="e1391-140">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="e1391-141">Имя</span><span class="sxs-lookup"><span data-stu-id="e1391-141">Name</span></span>                 | <span data-ttu-id="e1391-142">Значение</span><span class="sxs-lookup"><span data-stu-id="e1391-142">Value</span></span>  | <span data-ttu-id="e1391-143">Описание</span><span class="sxs-lookup"><span data-stu-id="e1391-143">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e1391-144">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="e1391-144">**@odata.nextLink**</span></span>  | <span data-ttu-id="e1391-145">url</span><span class="sxs-lookup"><span data-stu-id="e1391-145">url</span></span>    | <span data-ttu-id="e1391-146">URL-адрес для получения следующей доступной страницы изменений, если в текущем наборе есть дополнительные изменения.</span><span class="sxs-lookup"><span data-stu-id="e1391-146">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="e1391-147">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="e1391-147">**@odata.deltaLink**</span></span> | <span data-ttu-id="e1391-148">url</span><span class="sxs-lookup"><span data-stu-id="e1391-148">url</span></span>    | <span data-ttu-id="e1391-p107">URL-адрес, возвращаемый вместо **@odata.nextLink** после возврата всех текущих изменений. Используется для считывания следующего набора изменений в будущем.</span><span class="sxs-lookup"><span data-stu-id="e1391-p107">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="e1391-151">Пример (первоначальный запрос)</span><span class="sxs-lookup"><span data-stu-id="e1391-151">Example (Initial Request)</span></span>

<span data-ttu-id="e1391-152">Ниже приведен пример вызова этого API для определения локального состояния.</span><span class="sxs-lookup"><span data-stu-id="e1391-152">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="e1391-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1391-153">Request</span></span>

<span data-ttu-id="e1391-154">Ниже приведен пример первоначального запроса.</span><span class="sxs-lookup"><span data-stu-id="e1391-154">Here is an example of the initial request.</span></span>

<!-- { "blockType": "request", "name": "get_item_delta_first" } -->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

### <a name="response"></a><span data-ttu-id="e1391-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1391-155">Response</span></span>

<span data-ttu-id="e1391-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1391-156">Here is an example of the response.</span></span>

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

<span data-ttu-id="e1391-p108">Этот отклик включает первую страницу изменений, а свойство **@odata.nextLink** указывает, что в текущем наборе доступны дополнительные элементы. Ваше приложение должно запрашивать значение URL-адреса, указанного в свойстве **@odata.nextLink**, пока не будут получены все страницы элементов.</span><span class="sxs-lookup"><span data-stu-id="e1391-p108">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="e1391-159">Пример (последняя страница в наборе)</span><span class="sxs-lookup"><span data-stu-id="e1391-159">Example (Last page in a set)</span></span>

<span data-ttu-id="e1391-160">Ниже приведен пример вызова этого API для обновления локального состояния.</span><span class="sxs-lookup"><span data-stu-id="e1391-160">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="e1391-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1391-161">Request</span></span>

<span data-ttu-id="e1391-162">Ниже приведен пример запроса, выполненного после первоначального.</span><span class="sxs-lookup"><span data-stu-id="e1391-162">Here is an example request after the initial request.</span></span>

<!-- { "blockType": "request", "name": "get_item_delta_last" }-->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

### <a name="response"></a><span data-ttu-id="e1391-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1391-163">Response</span></span>

<span data-ttu-id="e1391-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1391-164">Here is an example of the response.</span></span>

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

<span data-ttu-id="e1391-165">Такой отклик означает, что между отправками первоначального запроса и данного запроса (на обновление локального состояния) был удален элемент `folder2`, а элемент `file.txt` был добавлен или изменен.</span><span class="sxs-lookup"><span data-stu-id="e1391-165">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="e1391-166">На последней странице элементов указано свойство **@odata.deltaLink**, содержащее URL-адрес, с помощью которого можно будет получить изменения относительно текущего набора элементов.</span><span class="sxs-lookup"><span data-stu-id="e1391-166">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="e1391-p109">В некоторых случаях службе не удается предоставить список изменений для определенного маркера (например, если клиент пытается повторно использовать старый маркер после долгого отключения, а также если из-за измененного состояния сервера требуется новый маркер). В таких случаях служба возвращает ошибку `HTTP 410 Gone` с откликом, содержащим один из представленных ниже кодов ошибок, и заголовком `Location`, содержащим новый аргумент nextLink, который начинает новое перечисление delta. По завершении полного перечисления сравните возвращенные элементы с локальным состоянием и выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="e1391-p109">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="e1391-170">Тип ошибки</span><span class="sxs-lookup"><span data-stu-id="e1391-170">Error Type</span></span>                       | <span data-ttu-id="e1391-171">Инструкции</span><span class="sxs-lookup"><span data-stu-id="e1391-171">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="e1391-p110">Замените все локальные элементы (в том числе удаленные) соответствующими элементами с сервера, если вы уверены, что при последней синхронизации в службу были внесены все локальные изменения. Отправьте все локальные изменения, не загруженные на сервер.</span><span class="sxs-lookup"><span data-stu-id="e1391-p110">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="e1391-174">Отправьте все локальные элементы, не возвращенные службой, и все файлы, отличающиеся от соответствующих файлов на сервере (сохраняйте обе копии, если вы не знаете, какая из них более актуальна).</span><span class="sxs-lookup"><span data-stu-id="e1391-174">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="e1391-175">Получение текущего значения deltaLink</span><span class="sxs-lookup"><span data-stu-id="e1391-175">Retrieving the current deltaLink</span></span>

<span data-ttu-id="e1391-176">В некоторых случаях может быть удобно запросить текущее значение deltaLink, не перечисляя перед этим все элементы, уже хранящиеся в объекте drive.</span><span class="sxs-lookup"><span data-stu-id="e1391-176">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="e1391-177">Это может быть полезно, если приложению достаточно узнать об изменениях и ему не нужны сведения о существующих элементах.</span><span class="sxs-lookup"><span data-stu-id="e1391-177">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items.</span></span>
<span data-ttu-id="e1391-178">Чтобы получить последнее значение deltaLink, вызовите функцию `delta` с параметром `?token=latest` в строке запроса.</span><span class="sxs-lookup"><span data-stu-id="e1391-178">To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="e1391-179">**Примечание. Если вы пытаетесь поддерживать полное локальное представление элементов в папке или на диске, необходимо использовать `delta` для исходного перечисления. Другие подходы, например постраничный просмотр коллекции `children` для папки, не гарантируют возврата всех элементов, если во время перечисления выполняются операции записи. Только с помощью функции `delta` можно гарантировать, что считываются все необходимые данные.**</span><span class="sxs-lookup"><span data-stu-id="e1391-179">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="e1391-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1391-180">Request</span></span>

<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "files.read", "target": "action" } -->

```http
GET /me/drive/root/delta?token=latest
```

### <a name="response"></a><span data-ttu-id="e1391-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1391-181">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="e1391-182">Примечания</span><span class="sxs-lookup"><span data-stu-id="e1391-182">Remarks</span></span>

* <span data-ttu-id="e1391-p112">В разностном канале показано последнее состояние каждого элемента, а не каждое изменение. Если элемент был переименован дважды, он будет указан только один раз, но с последним именем.</span><span class="sxs-lookup"><span data-stu-id="e1391-p112">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="e1391-p113">По ряду причин один и тот же элемент может отображаться в разностном канале несколько раз. Следует использовать последний представленный вариант.</span><span class="sxs-lookup"><span data-stu-id="e1391-p113">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="e1391-p114">Свойство `parentReference` элементов не включает значение **path**. Это вызвано тем, что при переименовании папки ее потомки не возвращаются с помощью **delta**. **При использовании delta следует всегда отслеживать элементы по идентификатору**.</span><span class="sxs-lookup"><span data-stu-id="e1391-p114">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="e1391-190">В OneDrive для бизнеса и SharePoint функция `delta` поддерживается только для папки `root`.</span><span class="sxs-lookup"><span data-stu-id="e1391-190">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders within a drive.</span></span>

* <span data-ttu-id="e1391-191">Функция delta не возвращает следующие свойства ресурса DriveItem:</span><span class="sxs-lookup"><span data-stu-id="e1391-191">Delta will not return the following DriveItem properties:</span></span>

* <span data-ttu-id="e1391-192">**cTag**;</span><span class="sxs-lookup"><span data-stu-id="e1391-192">**cTag**</span></span>
* <span data-ttu-id="e1391-193">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="e1391-193">**lastModifiedBy**</span></span>
* <span data-ttu-id="e1391-194">**size**.</span><span class="sxs-lookup"><span data-stu-id="e1391-194">**size**</span></span>

## <a name="error-responses"></a><span data-ttu-id="e1391-195">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="e1391-195">Error responses</span></span>

<span data-ttu-id="e1391-196">Помимо вышеописанных ошибок повторной синхронизации, в статье [Ошибки][error-response] представлены сведения о том, как возвращаются ошибки.</span><span class="sxs-lookup"><span data-stu-id="e1391-196">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes"
} -->
