---
author: JeremyKelley
ms.date: 09/10/2017
title: Скачивание файла
localization_priority: Priority
ms.prod: sharepoint
description: Скачивание содержимого основного потока (файла) ресурса DriveItem. Можно скачать только те ресурсы driveItem, у которых есть свойство file.
doc_type: apiPageType
ms.openlocfilehash: 524f9b44f0281be0b5731762b0d7654ae73984c3
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786039"
---
# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="50c07-104">Скачивание содержимого элемента DriveItem</span><span class="sxs-lookup"><span data-stu-id="50c07-104">Download the contents of a DriveItem</span></span>

<span data-ttu-id="50c07-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50c07-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50c07-106">В этой статье рассказывается, как скачать содержимое основного потока (файла) элемента DriveItem.</span><span class="sxs-lookup"><span data-stu-id="50c07-106">Download the contents of the primary stream (file) of a DriveItem.</span></span> <span data-ttu-id="50c07-107">Вы можете скачать только те элементы driveItem, у которых имеется свойство **file**.</span><span class="sxs-lookup"><span data-stu-id="50c07-107">Only driveItems with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="50c07-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50c07-108">Permissions</span></span>

<span data-ttu-id="50c07-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50c07-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50c07-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50c07-111">Permission type</span></span>      | <span data-ttu-id="50c07-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50c07-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50c07-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50c07-113">Delegated (work or school account)</span></span> | <span data-ttu-id="50c07-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50c07-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="50c07-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50c07-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50c07-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50c07-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="50c07-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50c07-117">Application</span></span> | <span data-ttu-id="50c07-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50c07-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50c07-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50c07-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a><span data-ttu-id="50c07-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50c07-120">Optional request headers</span></span>

| <span data-ttu-id="50c07-121">Имя</span><span class="sxs-lookup"><span data-stu-id="50c07-121">Name</span></span>          | <span data-ttu-id="50c07-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50c07-122">Value</span></span>  | <span data-ttu-id="50c07-123">Описание</span><span class="sxs-lookup"><span data-stu-id="50c07-123">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="50c07-124">if-none-match</span><span class="sxs-lookup"><span data-stu-id="50c07-124">if-none-match</span></span> | <span data-ttu-id="50c07-125">String</span><span class="sxs-lookup"><span data-stu-id="50c07-125">String</span></span> | <span data-ttu-id="50c07-126">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="50c07-126">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="50c07-127">Пример</span><span class="sxs-lookup"><span data-stu-id="50c07-127">Example</span></span>

<span data-ttu-id="50c07-128">В примере ниже показано, как скачать весь файл.</span><span class="sxs-lookup"><span data-stu-id="50c07-128">Here is an example to download a complete file.</span></span>



# <a name="http"></a>[<span data-ttu-id="50c07-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="50c07-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/content
```
# <a name="c"></a>[<span data-ttu-id="50c07-130">C#</span><span class="sxs-lookup"><span data-stu-id="50c07-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/download-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50c07-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50c07-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/download-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50c07-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50c07-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/download-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50c07-133">Java</span><span class="sxs-lookup"><span data-stu-id="50c07-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/download-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50c07-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="50c07-134">Response</span></span>

<span data-ttu-id="50c07-p104">Возвращает отклик `302 Found`, перенаправляя к URL-адресу загрузки файла, прошедшему предварительную проверку подлинности. Это такой же URL-адрес, доступный с помощью свойства `@microsoft.graph.downloadUrl` в ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="50c07-p104">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="50c07-137">Чтобы скачать содержимое файла, приложению необходимо следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="50c07-137">To download the contents of the file your application will need to follow the `Location` header in the response.</span></span>
<span data-ttu-id="50c07-138">Многие библиотеки клиентов HTTP будут автоматически следовать перенаправлению 302 и немедленно начинать загрузку файла.</span><span class="sxs-lookup"><span data-stu-id="50c07-138">Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immediately.</span></span>

<span data-ttu-id="50c07-139">URL-адреса загрузки, прошедшие предварительную проверку подлинности, действительны только на протяжении короткого периода времени (несколько минут) и не требуют заголовка `Authorization` для загрузки.</span><span class="sxs-lookup"><span data-stu-id="50c07-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="50c07-140">Загрузка части заданного диапазона байтов</span><span class="sxs-lookup"><span data-stu-id="50c07-140">Partial range downloads</span></span>

<span data-ttu-id="50c07-p106">Чтобы загрузить из файла часть заданного диапазона байтов, приложение может использовать заголовок `Range`, как указано в документе [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Обратите внимание, что заголовок `Range` необходимо добавлять в фактический URL-адрес `@microsoft.graph.downloadUrl`, а не в запрос для `/content`.</span><span class="sxs-lookup"><span data-stu-id="50c07-p106">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="50c07-p107">Это позволит вернуть отклик `HTTP 206 Partial Content` с запрашиваемым диапазоном байтов из файла. Если не удается создать диапазон, можно проигнорировать заголовок диапазона, после чего отклик `HTTP 200` возвращается с полным содержимым файла.</span><span class="sxs-lookup"><span data-stu-id="50c07-p107">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048
Content-Type: application/octet-stream

<first 1024 bytes of file>
```

### <a name="error-responses"></a><span data-ttu-id="50c07-145">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="50c07-145">Error responses</span></span>

<span data-ttu-id="50c07-146">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="50c07-146">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download",
  "suppressions": [
  ]
} -->

