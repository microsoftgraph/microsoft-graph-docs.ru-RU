---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Преобразование в другие форматы
ms.openlocfilehash: 7798905363217d366caabbdd9c82559f578c01aa
ms.sourcegitcommit: 809748ea18943f5fd1d99c4c65a9b964f39a5f25
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/08/2018
ms.locfileid: "23893300"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="4a037-102">Скачивание файла в другом формате</span><span class="sxs-lookup"><span data-stu-id="4a037-102">Download a file in another format</span></span>

<span data-ttu-id="4a037-103">С помощью этого API вы можете получить содержимое элемента в определенном формате.</span><span class="sxs-lookup"><span data-stu-id="4a037-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="4a037-104">Не все файлы можно преобразовать в любые форматы.</span><span class="sxs-lookup"><span data-stu-id="4a037-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="4a037-105">Сведения о том, как скачать элемент в его исходном формате, см. в статье о [скачивании содержимого элемента](driveitem_get_content.md).</span><span class="sxs-lookup"><span data-stu-id="4a037-105">To download the item in it's original format, see [download an item's contents](driveitem_get_content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a037-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4a037-106">Prerequisites</span></span>

<span data-ttu-id="4a037-107">Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.</span><span class="sxs-lookup"><span data-stu-id="4a037-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="4a037-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a037-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="4a037-109">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="4a037-109">Query parameters</span></span>

| <span data-ttu-id="4a037-110">Параметр</span><span class="sxs-lookup"><span data-stu-id="4a037-110">Parameter</span></span>      | <span data-ttu-id="4a037-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4a037-111">Type</span></span>  | <span data-ttu-id="4a037-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4a037-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="4a037-113">_формат_</span><span class="sxs-lookup"><span data-stu-id="4a037-113">_format_</span></span>  | <span data-ttu-id="4a037-114">строка</span><span class="sxs-lookup"><span data-stu-id="4a037-114">string</span></span> | <span data-ttu-id="4a037-115">Укажите формат, в котором следует скачать содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="4a037-115">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="4a037-116">Опции форматирования</span><span class="sxs-lookup"><span data-stu-id="4a037-116">Format options</span></span>

<span data-ttu-id="4a037-117">Для параметра **формат** допустимы указанные ниже значения:</span><span class="sxs-lookup"><span data-stu-id="4a037-117">The following values are valid for the **convert** parameter:</span></span>

| <span data-ttu-id="4a037-118">Значение формата</span><span class="sxs-lookup"><span data-stu-id="4a037-118">Format value</span></span> | <span data-ttu-id="4a037-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4a037-119">Description</span></span>                        | <span data-ttu-id="4a037-120">Поддерживаемые расширения источника</span><span class="sxs-lookup"><span data-stu-id="4a037-120">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="4a037-121">PDF</span><span class="sxs-lookup"><span data-stu-id="4a037-121">pdf</span></span>          | <span data-ttu-id="4a037-122">Преобразует элемент в формат PDF.</span><span class="sxs-lookup"><span data-stu-id="4a037-122">Converts the item into PDF format.</span></span> | <span data-ttu-id="4a037-123">CSV, DOC, DOCX, ODP, ODS, ODT, POT, POTM, POTX, PPS, PPSX, PPSXM, PPT, PPTM, PPTX, RTF, XLS, XLSX</span><span class="sxs-lookup"><span data-stu-id="4a037-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="4a037-124">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a037-124">Optional request headers</span></span>

| <span data-ttu-id="4a037-125">Имя</span><span class="sxs-lookup"><span data-stu-id="4a037-125">Name</span></span>            | <span data-ttu-id="4a037-126">Значение</span><span class="sxs-lookup"><span data-stu-id="4a037-126">Value</span></span>   | <span data-ttu-id="4a037-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4a037-127">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4a037-128">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="4a037-128">_if-none-match_</span></span> | <span data-ttu-id="4a037-129">Строка</span><span class="sxs-lookup"><span data-stu-id="4a037-129">String</span></span>  | <span data-ttu-id="4a037-130">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="4a037-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="4a037-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4a037-131">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="4a037-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a037-132">Response</span></span>

<span data-ttu-id="4a037-133">Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.</span><span class="sxs-lookup"><span data-stu-id="4a037-133">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="4a037-134">Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="4a037-134">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="4a037-135">URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.</span><span class="sxs-lookup"><span data-stu-id="4a037-135">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="4a037-136">Ошибки</span><span class="sxs-lookup"><span data-stu-id="4a037-136">Error responses</span></span>

<span data-ttu-id="4a037-137">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="4a037-137">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
