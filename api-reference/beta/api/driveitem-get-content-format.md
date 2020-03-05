---
author: JeremyKelley
description: С помощью этого API вы можете получить содержимое элемента в определенном формате.
ms.date: 09/10/2017
title: Преобразование в другие форматы
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 03bb884e8dde82c99d0aadfa2a6e925b0d6552a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432658"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="6765a-103">Скачивание файла в другом формате</span><span class="sxs-lookup"><span data-stu-id="6765a-103">Download a file in another format</span></span>

<span data-ttu-id="6765a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6765a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6765a-105">С помощью этого API вы можете получить содержимое элемента в определенном формате.</span><span class="sxs-lookup"><span data-stu-id="6765a-105">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="6765a-106">Не все файлы можно преобразовать в любые форматы.</span><span class="sxs-lookup"><span data-stu-id="6765a-106">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="6765a-107">Сведения о том, как скачать элемент в его исходном формате, см. в статье о [скачивании содержимого элемента](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="6765a-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6765a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6765a-108">Prerequisites</span></span>

<span data-ttu-id="6765a-109">Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.</span><span class="sxs-lookup"><span data-stu-id="6765a-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="6765a-110">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6765a-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="6765a-111">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="6765a-111">Query parameters</span></span>

| <span data-ttu-id="6765a-112">Параметр</span><span class="sxs-lookup"><span data-stu-id="6765a-112">Parameter</span></span>      | <span data-ttu-id="6765a-113">Тип</span><span class="sxs-lookup"><span data-stu-id="6765a-113">Type</span></span>  | <span data-ttu-id="6765a-114">Описание</span><span class="sxs-lookup"><span data-stu-id="6765a-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="6765a-115">_format_</span><span class="sxs-lookup"><span data-stu-id="6765a-115">_format_</span></span>  | <span data-ttu-id="6765a-116">строка</span><span class="sxs-lookup"><span data-stu-id="6765a-116">string</span></span> | <span data-ttu-id="6765a-117">Укажите формат, в котором следует скачать содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="6765a-117">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="6765a-118">Для параметра **format** допустимы указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="6765a-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="6765a-119">Значение</span><span class="sxs-lookup"><span data-stu-id="6765a-119">Value</span></span> | <span data-ttu-id="6765a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6765a-120">Description</span></span>                        | <span data-ttu-id="6765a-121">Поддерживаемые расширения источника</span><span class="sxs-lookup"><span data-stu-id="6765a-121">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="6765a-122">glb</span><span class="sxs-lookup"><span data-stu-id="6765a-122">glb</span></span>   | <span data-ttu-id="6765a-123">Преобразует элемент в формат GLB</span><span class="sxs-lookup"><span data-stu-id="6765a-123">Converts the item into GLB format</span></span>  | <span data-ttu-id="6765a-124">COOL, FBX, OBJ, PLY, STL, 3MF</span><span class="sxs-lookup"><span data-stu-id="6765a-124">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="6765a-125">html</span><span class="sxs-lookup"><span data-stu-id="6765a-125">html</span></span>  | <span data-ttu-id="6765a-126">Преобразует элемент в формат HTML</span><span class="sxs-lookup"><span data-stu-id="6765a-126">Converts the item into HTML format</span></span> | <span data-ttu-id="6765a-127">EML, MD, MSG</span><span class="sxs-lookup"><span data-stu-id="6765a-127">eml, md, msg</span></span>
| <span data-ttu-id="6765a-128">jpg</span><span class="sxs-lookup"><span data-stu-id="6765a-128">jpg</span></span>   | <span data-ttu-id="6765a-129">Преобразует элемент в формат JPG</span><span class="sxs-lookup"><span data-stu-id="6765a-129">Converts the item into JPG format</span></span>  | <span data-ttu-id="6765a-130">3G2, 3GP, 3GP2, 3GPP, 3MF, AI, ARW, ASF, AVI, BAS, BASH, BAT, BMP, C, CBL, CMD, COOL, CPP, CR2, CRW, CS, CSS, CSV, CUR, DCM, DCM30, DIC, DICM, DICOM, DNG, DOC, DOCX, DWG, EML, EPI, EPS, EPSF, EPSI, EPUB, ERF, FBX, FPPX, GIF, GLB, H, HCP, HEIC, HEIF, HTM, HTML, ICO, ICON, JAVA, JFIF, JPEG, JPG, JS, JSON, KEY, LOG, M2TS, M4A, M4V, MARKDOWN, MD, MEF, MOV, MOVIE, MP3, MP4, MP4V, MRW, MSG, MTS, NEF, NRW, NUMBERS, OBJ, ODP, ODT, OGG, ORF, PAGES, PANO, PDF, PEF, PHP, PICT, PL, PLY, PNG, POT, POTM, POTX, PPS, PPSX, PPSXM, PPT, PPTM, PPTX, PS, PS1, PSB, PSD, PY, RAW, RB, RTF, RW1, RW2, SH, SKETCH, SQL, SR2, STL, TIF, TIFF, TS, TXT, VB, WEBM, WMA, WMV, XAML, XBM, XCF, XD, XML, XPM, YAML, YML</span><span class="sxs-lookup"><span data-stu-id="6765a-130">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="6765a-131">pdf</span><span class="sxs-lookup"><span data-stu-id="6765a-131">pdf</span></span>   | <span data-ttu-id="6765a-132">Преобразует элемент в формат PDF</span><span class="sxs-lookup"><span data-stu-id="6765a-132">Converts the item into PDF format</span></span>  | <span data-ttu-id="6765a-133">DOC, DOCX, EPUB, EML, HTM, HTML, MD, MSG, ODP, ODS, ODT, PPS, PPSX, PPT, PPTX, RTF, TIF, TIFF, XLS, XLSM, XLSX</span><span class="sxs-lookup"><span data-stu-id="6765a-133">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="6765a-134">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6765a-134">Optional request headers</span></span>

| <span data-ttu-id="6765a-135">Имя</span><span class="sxs-lookup"><span data-stu-id="6765a-135">Name</span></span>            | <span data-ttu-id="6765a-136">Значение</span><span class="sxs-lookup"><span data-stu-id="6765a-136">Value</span></span>   | <span data-ttu-id="6765a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="6765a-137">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6765a-138">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="6765a-138">_if-none-match_</span></span> | <span data-ttu-id="6765a-139">String</span><span class="sxs-lookup"><span data-stu-id="6765a-139">String</span></span>  | <span data-ttu-id="6765a-140">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="6765a-140">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="6765a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="6765a-141">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="6765a-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6765a-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /drive/items/{item-id}/content?format={format}
```
# <a name="c"></a>[<span data-ttu-id="6765a-143">C#</span><span class="sxs-lookup"><span data-stu-id="6765a-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6765a-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6765a-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6765a-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6765a-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="6765a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="6765a-146">Response</span></span>

<span data-ttu-id="6765a-147">Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.</span><span class="sxs-lookup"><span data-stu-id="6765a-147">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="6765a-148">Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="6765a-148">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="6765a-149">URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.</span><span class="sxs-lookup"><span data-stu-id="6765a-149">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="6765a-150">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="6765a-150">Error responses</span></span>

<span data-ttu-id="6765a-151">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="6765a-151">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!--
{
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
  ]
}
-->
