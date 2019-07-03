---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Скачивание файла
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 8c7d364fde1fa6009a96c308330cd37d5a56df5f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445445"
---
# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="404af-102">Скачивание содержимого элемента DriveItem</span><span class="sxs-lookup"><span data-stu-id="404af-102">Download the contents of a DriveItem</span></span>

<span data-ttu-id="404af-103">В этой статье рассказывается, как скачать содержимое основного потока (файла) элемента DriveItem.</span><span class="sxs-lookup"><span data-stu-id="404af-103">Download the contents of the primary stream (file) of a DriveItem.</span></span> <span data-ttu-id="404af-104">Вы можете скачать только те элементы driveItem, у которых имеется свойство **file**.</span><span class="sxs-lookup"><span data-stu-id="404af-104">Only driveItems with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="404af-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="404af-105">Permissions</span></span>

<span data-ttu-id="404af-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="404af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="404af-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="404af-108">Permission type</span></span>      | <span data-ttu-id="404af-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="404af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="404af-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="404af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="404af-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="404af-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="404af-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="404af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="404af-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="404af-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="404af-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="404af-114">Application</span></span> | <span data-ttu-id="404af-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="404af-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="404af-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="404af-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a><span data-ttu-id="404af-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="404af-117">Optional request headers</span></span>

| <span data-ttu-id="404af-118">Имя</span><span class="sxs-lookup"><span data-stu-id="404af-118">Name</span></span>          | <span data-ttu-id="404af-119">Значение</span><span class="sxs-lookup"><span data-stu-id="404af-119">Value</span></span>  | <span data-ttu-id="404af-120">Описание</span><span class="sxs-lookup"><span data-stu-id="404af-120">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="404af-121">if-none-match</span><span class="sxs-lookup"><span data-stu-id="404af-121">if-none-match</span></span> | <span data-ttu-id="404af-122">String</span><span class="sxs-lookup"><span data-stu-id="404af-122">String</span></span> | <span data-ttu-id="404af-123">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="404af-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="404af-124">Пример</span><span class="sxs-lookup"><span data-stu-id="404af-124">Example</span></span>

<span data-ttu-id="404af-125">В примере ниже показано, как скачать весь файл.</span><span class="sxs-lookup"><span data-stu-id="404af-125">Here is an example to download a complete file.</span></span>



# <a name="httptabhttp"></a>[<span data-ttu-id="404af-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="404af-126">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="404af-127">C#</span><span class="sxs-lookup"><span data-stu-id="404af-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/download-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="404af-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="404af-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/download-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="404af-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="404af-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/download-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="404af-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="404af-130">Response</span></span>

<span data-ttu-id="404af-p103">Возвращает отклик `302 Found`, перенаправляя к URL-адресу загрузки файла, прошедшему предварительную проверку подлинности. Это такой же URL-адрес, доступный с помощью свойства `@microsoft.graph.downloadUrl` в ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="404af-p103">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="404af-133">Чтобы скачать содержимое файла, приложению необходимо следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="404af-133">To download the contents of the file your application will need to follow the `Location` header in the response.</span></span>
<span data-ttu-id="404af-134">Многие библиотеки клиентов HTTP будут автоматически следовать перенаправлению 302 и немедленно начинать загрузку файла.</span><span class="sxs-lookup"><span data-stu-id="404af-134">Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immediately.</span></span>

<span data-ttu-id="404af-135">URL-адреса загрузки, прошедшие предварительную проверку подлинности, действительны только на протяжении короткого периода времени (несколько минут) и не требуют заголовка `Authorization` для загрузки.</span><span class="sxs-lookup"><span data-stu-id="404af-135">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="404af-136">Загрузка части заданного диапазона байтов</span><span class="sxs-lookup"><span data-stu-id="404af-136">Partial range downloads</span></span>

<span data-ttu-id="404af-p105">Чтобы загрузить из файла часть заданного диапазона байтов, приложение может использовать заголовок `Range`, как указано в документе [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Обратите внимание, что заголовок `Range` необходимо добавлять в фактический URL-адрес `@microsoft.graph.downloadUrl`, а не в запрос для `/content`.</span><span class="sxs-lookup"><span data-stu-id="404af-p105">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="404af-p106">Это позволит вернуть отклик `HTTP 206 Partial Content` с запрашиваемым диапазоном байтов из файла. Если не удается создать диапазон, можно проигнорировать заголовок диапазона, после чего отклик `HTTP 200` возвращается с полным содержимым файла.</span><span class="sxs-lookup"><span data-stu-id="404af-p106">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048
Content-Type: application/octet-stream

<first 1024 bytes of file>
```

### <a name="error-responses"></a><span data-ttu-id="404af-141">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="404af-141">Error responses</span></span>

<span data-ttu-id="404af-142">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="404af-142">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
