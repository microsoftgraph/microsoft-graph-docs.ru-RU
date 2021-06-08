---
author: JeremyKelley
description: С помощью этого API вы можете получить содержимое элемента в определенном формате.
ms.date: 09/10/2017
title: Преобразование в другие форматы
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f6343e3b0ce7ba9eb114e6eeadc6040341fb5c47
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786820"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="5a2e2-103">Скачивание файла в другом формате</span><span class="sxs-lookup"><span data-stu-id="5a2e2-103">Download a file in another format</span></span>

<span data-ttu-id="5a2e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a2e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a2e2-p101">С помощью этого API вы можете получить содержимое элемента в определенном формате. Не все файлы можно преобразовать в любые форматы.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-p101">Use this API to retrieve the contents of an item in a specific format. Not all files can be converted into all formats.</span></span>

<span data-ttu-id="5a2e2-107">Сведения о том, как скачать элемент в его исходном формате, см. в статье о [скачивании содержимого элемента](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="5a2e2-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a2e2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a2e2-108">Prerequisites</span></span>

<span data-ttu-id="5a2e2-109">Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="5a2e2-110">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a2e2-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="5a2e2-111">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="5a2e2-111">Query parameters</span></span>

| <span data-ttu-id="5a2e2-112">Параметр</span><span class="sxs-lookup"><span data-stu-id="5a2e2-112">Parameter</span></span>      | <span data-ttu-id="5a2e2-113">Тип</span><span class="sxs-lookup"><span data-stu-id="5a2e2-113">Type</span></span>  | <span data-ttu-id="5a2e2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="5a2e2-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="5a2e2-115">_format_</span><span class="sxs-lookup"><span data-stu-id="5a2e2-115">_format_</span></span>  | <span data-ttu-id="5a2e2-116">строка</span><span class="sxs-lookup"><span data-stu-id="5a2e2-116">string</span></span> | <span data-ttu-id="5a2e2-117">Укажите формат, в котором следует скачать содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-117">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="5a2e2-118">Для параметра **format** допустимы указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="5a2e2-119">Значение</span><span class="sxs-lookup"><span data-stu-id="5a2e2-119">Value</span></span> | <span data-ttu-id="5a2e2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5a2e2-120">Description</span></span>                        | <span data-ttu-id="5a2e2-121">Поддерживаемые расширения источника</span><span class="sxs-lookup"><span data-stu-id="5a2e2-121">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="5a2e2-122">glb</span><span class="sxs-lookup"><span data-stu-id="5a2e2-122">glb</span></span>   | <span data-ttu-id="5a2e2-123">Преобразует элемент в формат GLB</span><span class="sxs-lookup"><span data-stu-id="5a2e2-123">Converts the item into GLB format</span></span>  | <span data-ttu-id="5a2e2-124">COOL, FBX, OBJ, PLY, STL, 3MF</span><span class="sxs-lookup"><span data-stu-id="5a2e2-124">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="5a2e2-125">html</span><span class="sxs-lookup"><span data-stu-id="5a2e2-125">html</span></span>  | <span data-ttu-id="5a2e2-126">Преобразует элемент в формат HTML</span><span class="sxs-lookup"><span data-stu-id="5a2e2-126">Converts the item into HTML format</span></span> | <span data-ttu-id="5a2e2-127">EML, MD, MSG</span><span class="sxs-lookup"><span data-stu-id="5a2e2-127">eml, md, msg</span></span>
| <span data-ttu-id="5a2e2-128">jpg</span><span class="sxs-lookup"><span data-stu-id="5a2e2-128">jpg</span></span>   | <span data-ttu-id="5a2e2-129">Преобразует элемент в формат JPG</span><span class="sxs-lookup"><span data-stu-id="5a2e2-129">Converts the item into JPG format</span></span>  | <span data-ttu-id="5a2e2-130">3G2, 3GP, 3GP2, 3GPP, 3MF, AI, ARW, ASF, AVI, BAS, BASH, BAT, BMP, C, CBL, CMD, COOL, CPP, CR2, CRW, CS, CSS, CSV, CUR, DCM, DCM30, DIC, DICM, DICOM, DNG, DOC, DOCX, DWG, EML, EPI, EPS, EPSF, EPSI, EPUB, ERF, FBX, FPPX, GIF, GLB, H, HCP, HEIC, HEIF, HTM, HTML, ICO, ICON, JAVA, JFIF, JPEG, JPG, JS, JSON, KEY, LOG, M2TS, M4A, M4V, MARKDOWN, MD, MEF, MOV, MOVIE, MP3, MP4, MP4V, MRW, MSG, MTS, NEF, NRW, NUMBERS, OBJ, ODP, ODT, OGG, ORF, PAGES, PANO, PDF, PEF, PHP, PICT, PL, PLY, PNG, POT, POTM, POTX, PPS, PPSX, PPSXM, PPT, PPTM, PPTX, PS, PS1, PSB, PSD, PY, RAW, RB, RTF, RW1, RW2, SH, SKETCH, SQL, SR2, STL, TIF, TIFF, TS, TXT, VB, WEBM, WMA, WMV, XAML, XBM, XCF, XD, XML, XPM, YAML, YML</span><span class="sxs-lookup"><span data-stu-id="5a2e2-130">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="5a2e2-131">pdf</span><span class="sxs-lookup"><span data-stu-id="5a2e2-131">pdf</span></span>   | <span data-ttu-id="5a2e2-132">Преобразует элемент в формат PDF</span><span class="sxs-lookup"><span data-stu-id="5a2e2-132">Converts the item into PDF format</span></span>  | <span data-ttu-id="5a2e2-133">DOC, DOCX, EPUB, EML, HTM, HTML, MD, MSG, ODP, ODS, ODT, PPS, PPSX, PPT, PPTX, RTF, TIF, TIFF, XLS, XLSM, XLSX</span><span class="sxs-lookup"><span data-stu-id="5a2e2-133">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="5a2e2-134">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a2e2-134">Optional request headers</span></span>

| <span data-ttu-id="5a2e2-135">Имя</span><span class="sxs-lookup"><span data-stu-id="5a2e2-135">Name</span></span>            | <span data-ttu-id="5a2e2-136">Значение</span><span class="sxs-lookup"><span data-stu-id="5a2e2-136">Value</span></span>   | <span data-ttu-id="5a2e2-137">Описание</span><span class="sxs-lookup"><span data-stu-id="5a2e2-137">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5a2e2-138">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="5a2e2-138">_if-none-match_</span></span> | <span data-ttu-id="5a2e2-139">String</span><span class="sxs-lookup"><span data-stu-id="5a2e2-139">String</span></span>  | <span data-ttu-id="5a2e2-140">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-140">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="5a2e2-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5a2e2-141">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="5a2e2-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a2e2-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /drive/items/{item-id}/content?format={format}
```
# <a name="c"></a>[<span data-ttu-id="5a2e2-143">C#</span><span class="sxs-lookup"><span data-stu-id="5a2e2-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a2e2-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a2e2-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a2e2-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a2e2-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a2e2-146">Java</span><span class="sxs-lookup"><span data-stu-id="5a2e2-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="5a2e2-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a2e2-147">Response</span></span>

<span data-ttu-id="5a2e2-148">Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-148">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="5a2e2-149">Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-149">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="5a2e2-150">URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-150">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="5a2e2-151">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="5a2e2-151">Error responses</span></span>

<span data-ttu-id="5a2e2-152">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="5a2e2-152">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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


