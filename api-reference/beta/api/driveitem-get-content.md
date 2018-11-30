---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Скачивание файла
ms.openlocfilehash: 8b86954bd2a07d7b476762c4baef36f4f7fb7cbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079806"
---
# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="818b3-102">Скачивание содержимого элемента DriveItem</span><span class="sxs-lookup"><span data-stu-id="818b3-102">Download the contents of a DriveItem</span></span>

> <span data-ttu-id="818b3-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="818b3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="818b3-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="818b3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="818b3-105">В этой статье рассказывается, как скачать содержимое основного потока (файла) элемента DriveItem.</span><span class="sxs-lookup"><span data-stu-id="818b3-105">Download the contents of the primary stream (file) of a DriveItem.</span></span> <span data-ttu-id="818b3-106">Вы можете скачать только те элементы driveItem, у которых имеется свойство **file**.</span><span class="sxs-lookup"><span data-stu-id="818b3-106">Only driveItems with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="818b3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="818b3-107">Permissions</span></span>

<span data-ttu-id="818b3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="818b3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="818b3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="818b3-110">Permission type</span></span>      | <span data-ttu-id="818b3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="818b3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="818b3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="818b3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="818b3-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="818b3-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="818b3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="818b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="818b3-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="818b3-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="818b3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="818b3-116">Application</span></span> | <span data-ttu-id="818b3-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="818b3-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="818b3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="818b3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a><span data-ttu-id="818b3-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="818b3-119">Optional request headers</span></span>

| <span data-ttu-id="818b3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="818b3-120">Name</span></span>          | <span data-ttu-id="818b3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="818b3-121">Value</span></span>  | <span data-ttu-id="818b3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="818b3-122">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="818b3-123">if-none-match</span><span class="sxs-lookup"><span data-stu-id="818b3-123">if-none-match</span></span> | <span data-ttu-id="818b3-124">String</span><span class="sxs-lookup"><span data-stu-id="818b3-124">String</span></span> | <span data-ttu-id="818b3-125">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="818b3-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="818b3-126">Пример</span><span class="sxs-lookup"><span data-stu-id="818b3-126">Example</span></span>

<span data-ttu-id="818b3-127">В примере ниже показано, как скачать весь файл.</span><span class="sxs-lookup"><span data-stu-id="818b3-127">Here is an example to download a complete file.</span></span>


<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content
```

### <a name="response"></a><span data-ttu-id="818b3-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="818b3-128">Response</span></span>

<span data-ttu-id="818b3-p104">Возвращает отклик `302 Found`, перенаправляя к URL-адресу загрузки файла, прошедшему предварительную проверку подлинности. Это такой же URL-адрес, доступный с помощью свойства `@microsoft.graph.downloadUrl` в ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="818b3-p104">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="818b3-p105">Чтобы загрузить содержимое файла, приложению необходимо будет следовать заголовку `Location` в отклике. Многие библиотеки клиентов HTTP будут автоматически следовать перенаправлению 302 и немедленно начинать загрузку файла.</span><span class="sxs-lookup"><span data-stu-id="818b3-p105">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="818b3-133">URL-адреса загрузки, прошедшие предварительную проверку подлинности, действительны только на протяжении короткого периода времени (несколько минут) и не требуют заголовка `Authorization` для загрузки.</span><span class="sxs-lookup"><span data-stu-id="818b3-133">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="818b3-134">Загрузка части заданного диапазона байтов</span><span class="sxs-lookup"><span data-stu-id="818b3-134">Partial range downloads</span></span>

<span data-ttu-id="818b3-p106">Чтобы загрузить из файла часть заданного диапазона байтов, приложение может использовать заголовок `Range`, как указано в документе [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Обратите внимание, что заголовок `Range` необходимо добавлять в фактический URL-адрес `@microsoft.graph.downloadUrl`, а не в запрос для `/content`.</span><span class="sxs-lookup"><span data-stu-id="818b3-p106">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="818b3-p107">Это позволит вернуть отклик `HTTP 206 Partial Content` с запрашиваемым диапазоном байтов из файла. Если не удается создать диапазон, можно проигнорировать заголовок диапазона, после чего отклик `HTTP 200` возвращается с полным содержимым файла.</span><span class="sxs-lookup"><span data-stu-id="818b3-p107">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048

<first 1024 bytes of file>
```

### <a name="error-responses"></a><span data-ttu-id="818b3-139">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="818b3-139">Error responses</span></span>

<span data-ttu-id="818b3-140">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="818b3-140">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download"
} -->
