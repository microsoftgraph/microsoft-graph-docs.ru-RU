---
author: JeremyKelley
ms.date: 09/10/2017
title: Преобразование в другие форматы
localization_priority: Priority
ms.prod: sharepoint
description: С помощью этого API вы можете получить содержимое элемента в определенном формате.
doc_type: apiPageType
ms.openlocfilehash: 38b87b43f137fe291be31d98d97ea9a9448e6c9a
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787809"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="c2b7d-103">Скачивание файла в другом формате</span><span class="sxs-lookup"><span data-stu-id="c2b7d-103">Download a file in another format</span></span>

<span data-ttu-id="c2b7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2b7d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2b7d-p101">С помощью этого API вы можете получить содержимое элемента в определенном формате. Не все файлы можно преобразовать в любые форматы.</span><span class="sxs-lookup"><span data-stu-id="c2b7d-p101">Use this API to retrieve the contents of an item in a specific format. Not all files can be converted into all formats.</span></span>

<span data-ttu-id="c2b7d-107">Сведения о том, как скачать элемент в его исходном формате, см. в статье о [скачивании содержимого элемента](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="c2b7d-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2b7d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2b7d-108">Prerequisites</span></span>

<span data-ttu-id="c2b7d-109">Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.</span><span class="sxs-lookup"><span data-stu-id="c2b7d-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="c2b7d-110">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2b7d-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="c2b7d-111">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="c2b7d-111">Query parameters</span></span>

| <span data-ttu-id="c2b7d-112">Параметр</span><span class="sxs-lookup"><span data-stu-id="c2b7d-112">Parameter</span></span>      | <span data-ttu-id="c2b7d-113">Тип</span><span class="sxs-lookup"><span data-stu-id="c2b7d-113">Type</span></span>  | <span data-ttu-id="c2b7d-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c2b7d-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="c2b7d-115">_format_</span><span class="sxs-lookup"><span data-stu-id="c2b7d-115">_format_</span></span>  | <span data-ttu-id="c2b7d-116">строка</span><span class="sxs-lookup"><span data-stu-id="c2b7d-116">string</span></span> | <span data-ttu-id="c2b7d-117">Укажите формат, в котором следует скачать содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="c2b7d-117">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="c2b7d-118">Параметры форматирования</span><span class="sxs-lookup"><span data-stu-id="c2b7d-118">Format options</span></span>

<span data-ttu-id="c2b7d-119">Для параметра **format** допустимы указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="c2b7d-119">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="c2b7d-120">Значение формата</span><span class="sxs-lookup"><span data-stu-id="c2b7d-120">Format value</span></span> | <span data-ttu-id="c2b7d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c2b7d-121">Description</span></span>                        | <span data-ttu-id="c2b7d-122">Поддерживаемые расширения источника</span><span class="sxs-lookup"><span data-stu-id="c2b7d-122">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="c2b7d-123">pdf</span><span class="sxs-lookup"><span data-stu-id="c2b7d-123">pdf</span></span>          | <span data-ttu-id="c2b7d-124">Преобразует элемент в формат PDF.</span><span class="sxs-lookup"><span data-stu-id="c2b7d-124">Converts the item into PDF format.</span></span> | <span data-ttu-id="c2b7d-125">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span><span class="sxs-lookup"><span data-stu-id="c2b7d-125">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="c2b7d-126">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2b7d-126">Optional request headers</span></span>

| <span data-ttu-id="c2b7d-127">Имя</span><span class="sxs-lookup"><span data-stu-id="c2b7d-127">Name</span></span>            | <span data-ttu-id="c2b7d-128">Значение</span><span class="sxs-lookup"><span data-stu-id="c2b7d-128">Value</span></span>   | <span data-ttu-id="c2b7d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c2b7d-129">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c2b7d-130">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="c2b7d-130">_if-none-match_</span></span> | <span data-ttu-id="c2b7d-131">String</span><span class="sxs-lookup"><span data-stu-id="c2b7d-131">String</span></span>  | <span data-ttu-id="c2b7d-132">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="c2b7d-132">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="c2b7d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c2b7d-133">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="c2b7d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2b7d-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/content?format={format}
```
# <a name="c"></a>[<span data-ttu-id="c2b7d-135">C#</span><span class="sxs-lookup"><span data-stu-id="c2b7d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2b7d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2b7d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2b7d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2b7d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2b7d-138">Java</span><span class="sxs-lookup"><span data-stu-id="c2b7d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="c2b7d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2b7d-139">Response</span></span>

<span data-ttu-id="c2b7d-140">Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.</span><span class="sxs-lookup"><span data-stu-id="c2b7d-140">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="c2b7d-141">Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="c2b7d-141">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="c2b7d-142">URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.</span><span class="sxs-lookup"><span data-stu-id="c2b7d-142">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="c2b7d-143">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="c2b7d-143">Error responses</span></span>

<span data-ttu-id="c2b7d-144">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="c2b7d-144">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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

