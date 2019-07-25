---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Преобразование в другие форматы
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e66d302c7397690f6975363f9c3785f8b620756d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890975"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="61bb0-102">Скачивание файла в другом формате</span><span class="sxs-lookup"><span data-stu-id="61bb0-102">Download a file in another format</span></span>

<span data-ttu-id="61bb0-103">С помощью этого API вы можете получить содержимое элемента в определенном формате.</span><span class="sxs-lookup"><span data-stu-id="61bb0-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="61bb0-104">Не все файлы можно преобразовать в любые форматы.</span><span class="sxs-lookup"><span data-stu-id="61bb0-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="61bb0-105">Сведения о том, как скачать элемент в его исходном формате, см. в статье о [скачивании содержимого элемента](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="61bb0-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61bb0-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="61bb0-106">Prerequisites</span></span>

<span data-ttu-id="61bb0-107">Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.</span><span class="sxs-lookup"><span data-stu-id="61bb0-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="61bb0-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61bb0-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="61bb0-109">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="61bb0-109">Query parameters</span></span>

| <span data-ttu-id="61bb0-110">Параметр</span><span class="sxs-lookup"><span data-stu-id="61bb0-110">Parameter</span></span>      | <span data-ttu-id="61bb0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="61bb0-111">Type</span></span>  | <span data-ttu-id="61bb0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="61bb0-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="61bb0-113">_format_</span><span class="sxs-lookup"><span data-stu-id="61bb0-113">_format_</span></span>  | <span data-ttu-id="61bb0-114">строка</span><span class="sxs-lookup"><span data-stu-id="61bb0-114">string</span></span> | <span data-ttu-id="61bb0-115">Укажите формат, в котором следует скачать содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="61bb0-115">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="61bb0-116">Параметры форматирования</span><span class="sxs-lookup"><span data-stu-id="61bb0-116">Format options</span></span>

<span data-ttu-id="61bb0-117">Для параметра **format** допустимы указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="61bb0-117">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="61bb0-118">Значение формата</span><span class="sxs-lookup"><span data-stu-id="61bb0-118">Format value</span></span> | <span data-ttu-id="61bb0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="61bb0-119">Description</span></span>                        | <span data-ttu-id="61bb0-120">Поддерживаемые расширения источника</span><span class="sxs-lookup"><span data-stu-id="61bb0-120">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="61bb0-121">pdf</span><span class="sxs-lookup"><span data-stu-id="61bb0-121">pdf</span></span>          | <span data-ttu-id="61bb0-122">Преобразует элемент в формат PDF.</span><span class="sxs-lookup"><span data-stu-id="61bb0-122">Converts the item into PDF format.</span></span> | <span data-ttu-id="61bb0-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span><span class="sxs-lookup"><span data-stu-id="61bb0-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="61bb0-124">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61bb0-124">Optional request headers</span></span>

| <span data-ttu-id="61bb0-125">Имя</span><span class="sxs-lookup"><span data-stu-id="61bb0-125">Name</span></span>            | <span data-ttu-id="61bb0-126">Значение</span><span class="sxs-lookup"><span data-stu-id="61bb0-126">Value</span></span>   | <span data-ttu-id="61bb0-127">Описание</span><span class="sxs-lookup"><span data-stu-id="61bb0-127">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="61bb0-128">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="61bb0-128">_if-none-match_</span></span> | <span data-ttu-id="61bb0-129">String</span><span class="sxs-lookup"><span data-stu-id="61bb0-129">String</span></span>  | <span data-ttu-id="61bb0-130">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="61bb0-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="61bb0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="61bb0-131">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="61bb0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="61bb0-132">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="61bb0-133">C#</span><span class="sxs-lookup"><span data-stu-id="61bb0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="61bb0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61bb0-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="61bb0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61bb0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="61bb0-136">Java</span><span class="sxs-lookup"><span data-stu-id="61bb0-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="61bb0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="61bb0-137">Response</span></span>

<span data-ttu-id="61bb0-138">Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.</span><span class="sxs-lookup"><span data-stu-id="61bb0-138">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="61bb0-139">Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="61bb0-139">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="61bb0-140">URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.</span><span class="sxs-lookup"><span data-stu-id="61bb0-140">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="61bb0-141">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="61bb0-141">Error responses</span></span>

<span data-ttu-id="61bb0-142">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="61bb0-142">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
