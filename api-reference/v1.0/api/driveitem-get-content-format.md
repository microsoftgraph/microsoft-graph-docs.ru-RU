---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Преобразование в другие форматы
localization_priority: Priority
ms.prod: sharepoint
description: С помощью этого API вы можете получить содержимое элемента в определенном формате.
doc_type: apiPageType
ms.openlocfilehash: 811c0ae25666d23fd597b5d584e5b00e50a00e93
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726335"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="d1a6a-103">Скачивание файла в другом формате</span><span class="sxs-lookup"><span data-stu-id="d1a6a-103">Download a file in another format</span></span>

<span data-ttu-id="d1a6a-104">С помощью этого API вы можете получить содержимое элемента в определенном формате.</span><span class="sxs-lookup"><span data-stu-id="d1a6a-104">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="d1a6a-105">Не все файлы можно преобразовать в любые форматы.</span><span class="sxs-lookup"><span data-stu-id="d1a6a-105">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="d1a6a-106">Сведения о том, как скачать элемент в его исходном формате, см. в статье о [скачивании содержимого элемента](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="d1a6a-106">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1a6a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d1a6a-107">Prerequisites</span></span>

<span data-ttu-id="d1a6a-108">Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.</span><span class="sxs-lookup"><span data-stu-id="d1a6a-108">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="d1a6a-109">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1a6a-109">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="d1a6a-110">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="d1a6a-110">Query parameters</span></span>

| <span data-ttu-id="d1a6a-111">Параметр</span><span class="sxs-lookup"><span data-stu-id="d1a6a-111">Parameter</span></span>      | <span data-ttu-id="d1a6a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="d1a6a-112">Type</span></span>  | <span data-ttu-id="d1a6a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d1a6a-113">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="d1a6a-114">_format_</span><span class="sxs-lookup"><span data-stu-id="d1a6a-114">_format_</span></span>  | <span data-ttu-id="d1a6a-115">строка</span><span class="sxs-lookup"><span data-stu-id="d1a6a-115">string</span></span> | <span data-ttu-id="d1a6a-116">Укажите формат, в котором следует скачать содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="d1a6a-116">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="d1a6a-117">Параметры форматирования</span><span class="sxs-lookup"><span data-stu-id="d1a6a-117">Format options</span></span>

<span data-ttu-id="d1a6a-118">Для параметра **format** допустимы указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="d1a6a-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="d1a6a-119">Значение формата</span><span class="sxs-lookup"><span data-stu-id="d1a6a-119">Format value</span></span> | <span data-ttu-id="d1a6a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d1a6a-120">Description</span></span>                        | <span data-ttu-id="d1a6a-121">Поддерживаемые расширения источника</span><span class="sxs-lookup"><span data-stu-id="d1a6a-121">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="d1a6a-122">pdf</span><span class="sxs-lookup"><span data-stu-id="d1a6a-122">pdf</span></span>          | <span data-ttu-id="d1a6a-123">Преобразует элемент в формат PDF.</span><span class="sxs-lookup"><span data-stu-id="d1a6a-123">Converts the item into PDF format.</span></span> | <span data-ttu-id="d1a6a-124">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span><span class="sxs-lookup"><span data-stu-id="d1a6a-124">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="d1a6a-125">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1a6a-125">Optional request headers</span></span>

| <span data-ttu-id="d1a6a-126">Имя</span><span class="sxs-lookup"><span data-stu-id="d1a6a-126">Name</span></span>            | <span data-ttu-id="d1a6a-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d1a6a-127">Value</span></span>   | <span data-ttu-id="d1a6a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d1a6a-128">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d1a6a-129">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="d1a6a-129">_if-none-match_</span></span> | <span data-ttu-id="d1a6a-130">String</span><span class="sxs-lookup"><span data-stu-id="d1a6a-130">String</span></span>  | <span data-ttu-id="d1a6a-131">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="d1a6a-131">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="d1a6a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d1a6a-132">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d1a6a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1a6a-133">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/content?format={format}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d1a6a-134">C#</span><span class="sxs-lookup"><span data-stu-id="d1a6a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1a6a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1a6a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d1a6a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1a6a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d1a6a-137">Java</span><span class="sxs-lookup"><span data-stu-id="d1a6a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="d1a6a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1a6a-138">Response</span></span>

<span data-ttu-id="d1a6a-139">Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.</span><span class="sxs-lookup"><span data-stu-id="d1a6a-139">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="d1a6a-140">Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="d1a6a-140">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="d1a6a-141">URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.</span><span class="sxs-lookup"><span data-stu-id="d1a6a-141">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="d1a6a-142">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="d1a6a-142">Error responses</span></span>

<span data-ttu-id="d1a6a-143">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="d1a6a-143">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
  ]
} -->
