---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Преобразование в другие форматы"
ms.openlocfilehash: 3031500beaec2d765075abfd925a6333f50368f9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="654bd-102">Скачивание файла в другом формате</span><span class="sxs-lookup"><span data-stu-id="654bd-102">Download a file in another format</span></span>

<span data-ttu-id="654bd-103">С помощью этого API вы можете получить содержимое элемента в определенном формате.</span><span class="sxs-lookup"><span data-stu-id="654bd-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="654bd-104">Не все файлы можно преобразовать в любые форматы.</span><span class="sxs-lookup"><span data-stu-id="654bd-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="654bd-105">Сведения о том, как скачать элемент в его исходном формате, см. в статье о [скачивании содержимого элемента](driveitem_get_content.md).</span><span class="sxs-lookup"><span data-stu-id="654bd-105">To download the item in it's original format, see [download an item's contents](driveitem_get_content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="654bd-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="654bd-106">Prerequisites</span></span>

<span data-ttu-id="654bd-107">Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.</span><span class="sxs-lookup"><span data-stu-id="654bd-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="654bd-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="654bd-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

### <a name="optional-request-headers"></a><span data-ttu-id="654bd-109">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="654bd-109">Optional request headers</span></span>

| <span data-ttu-id="654bd-110">Имя</span><span class="sxs-lookup"><span data-stu-id="654bd-110">Name</span></span>            | <span data-ttu-id="654bd-111">Значение</span><span class="sxs-lookup"><span data-stu-id="654bd-111">Value</span></span>   | <span data-ttu-id="654bd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="654bd-112">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="654bd-113">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="654bd-113">_if-none-match_</span></span> | <span data-ttu-id="654bd-114">String</span><span class="sxs-lookup"><span data-stu-id="654bd-114">String</span></span>  | <span data-ttu-id="654bd-115">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="654bd-115">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


### <a name="query-string-parameters"></a><span data-ttu-id="654bd-116">Параметры строки запроса</span><span class="sxs-lookup"><span data-stu-id="654bd-116">Query string parameters</span></span>

| <span data-ttu-id="654bd-117">Имя</span><span class="sxs-lookup"><span data-stu-id="654bd-117">Name</span></span>      | <span data-ttu-id="654bd-118">Значение</span><span class="sxs-lookup"><span data-stu-id="654bd-118">Value</span></span>  | <span data-ttu-id="654bd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="654bd-119">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="654bd-120">_format_</span><span class="sxs-lookup"><span data-stu-id="654bd-120">_format_</span></span>  | <span data-ttu-id="654bd-121">строка</span><span class="sxs-lookup"><span data-stu-id="654bd-121">string</span></span> | <span data-ttu-id="654bd-122">Укажите формат, в котором следует скачать содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="654bd-122">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="654bd-123">Для параметра **convert** допустимы указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="654bd-123">The following values are valid for the **convert** parameter:</span></span>

| <span data-ttu-id="654bd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="654bd-124">Value</span></span>   | <span data-ttu-id="654bd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="654bd-125">Description</span></span>                        | <span data-ttu-id="654bd-126">Поддерживаемые расширения источника</span><span class="sxs-lookup"><span data-stu-id="654bd-126">Supported source extensions</span></span> |
|:--------|:-----------------------------------|-----------------------------|
| <span data-ttu-id="654bd-127">**pdf**</span><span class="sxs-lookup"><span data-stu-id="654bd-127">**pdf**</span></span> | <span data-ttu-id="654bd-128">Преобразует элемент в формат PDF.</span><span class="sxs-lookup"><span data-stu-id="654bd-128">Converts the item into PDF format.</span></span> | <span data-ttu-id="654bd-129">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span><span class="sxs-lookup"><span data-stu-id="654bd-129">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span> | 

### <a name="example"></a><span data-ttu-id="654bd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="654bd-130">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="654bd-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="654bd-131">Response</span></span>

<span data-ttu-id="654bd-132">Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.</span><span class="sxs-lookup"><span data-stu-id="654bd-132">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="654bd-133">Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="654bd-133">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="654bd-134">URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.</span><span class="sxs-lookup"><span data-stu-id="654bd-134">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="654bd-135">Ошибки</span><span class="sxs-lookup"><span data-stu-id="654bd-135">Error responses</span></span>

<span data-ttu-id="654bd-136">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="654bd-136">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
