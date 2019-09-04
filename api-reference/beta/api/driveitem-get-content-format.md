---
author: JeremyKelley
description: С помощью этого API вы можете получить содержимое элемента в определенном формате.
ms.date: 09/10/2017
title: Преобразование в другие форматы
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 914f6b5d847c6b8af5439c4b5e83f3d9f281aa65
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719383"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="8eba3-103">Скачивание файла в другом формате</span><span class="sxs-lookup"><span data-stu-id="8eba3-103">Download a file in another format</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8eba3-104">С помощью этого API вы можете получить содержимое элемента в определенном формате.</span><span class="sxs-lookup"><span data-stu-id="8eba3-104">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="8eba3-105">Не все файлы можно преобразовать в любые форматы.</span><span class="sxs-lookup"><span data-stu-id="8eba3-105">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="8eba3-106">Сведения о том, как скачать элемент в его исходном формате, см. в статье о [скачивании содержимого элемента](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="8eba3-106">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8eba3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8eba3-107">Prerequisites</span></span>

<span data-ttu-id="8eba3-108">Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.</span><span class="sxs-lookup"><span data-stu-id="8eba3-108">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="8eba3-109">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8eba3-109">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="8eba3-110">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="8eba3-110">Query parameters</span></span>

| <span data-ttu-id="8eba3-111">Параметр</span><span class="sxs-lookup"><span data-stu-id="8eba3-111">Parameter</span></span>      | <span data-ttu-id="8eba3-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8eba3-112">Type</span></span>  | <span data-ttu-id="8eba3-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8eba3-113">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="8eba3-114">_format_</span><span class="sxs-lookup"><span data-stu-id="8eba3-114">_format_</span></span>  | <span data-ttu-id="8eba3-115">строка</span><span class="sxs-lookup"><span data-stu-id="8eba3-115">string</span></span> | <span data-ttu-id="8eba3-116">Укажите формат, в котором следует скачать содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="8eba3-116">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="8eba3-117">Для параметра **format** допустимы указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="8eba3-117">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="8eba3-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8eba3-118">Value</span></span> | <span data-ttu-id="8eba3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8eba3-119">Description</span></span>                        | <span data-ttu-id="8eba3-120">Поддерживаемые расширения источника</span><span class="sxs-lookup"><span data-stu-id="8eba3-120">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="8eba3-121">глб</span><span class="sxs-lookup"><span data-stu-id="8eba3-121">glb</span></span>   | <span data-ttu-id="8eba3-122">Преобразует элемент в формат ГЛБ</span><span class="sxs-lookup"><span data-stu-id="8eba3-122">Converts the item into GLB format</span></span>  | <span data-ttu-id="8eba3-123">крутой, фбкс, obj, лист, STL, 3mf</span><span class="sxs-lookup"><span data-stu-id="8eba3-123">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="8eba3-124">html</span><span class="sxs-lookup"><span data-stu-id="8eba3-124">html</span></span>  | <span data-ttu-id="8eba3-125">Преобразует элемент в формат HTML</span><span class="sxs-lookup"><span data-stu-id="8eba3-125">Converts the item into HTML format</span></span> | <span data-ttu-id="8eba3-126">EML, MD, MSG</span><span class="sxs-lookup"><span data-stu-id="8eba3-126">eml, md, msg</span></span>
| <span data-ttu-id="8eba3-127">JPEG</span><span class="sxs-lookup"><span data-stu-id="8eba3-127">jpg</span></span>   | <span data-ttu-id="8eba3-128">Преобразует элемент в формат JPG</span><span class="sxs-lookup"><span data-stu-id="8eba3-128">Converts the item into JPG format</span></span>  | <span data-ttu-id="8eba3-129">3G2, 3GP, 3GP2, 3GPP, 3mf, AI, АРВ, ASF, AVI, BAS, bash, bat, BMP, c, КБЛ, cmd, Cool, CPP, CR2, КРВ, CS, CSS, CSV, cur, DCM, dcm30, DIC, ДИКМ, DICOM, ДНГ, doc, DOCX, DWG, EML, EPI,, епсф, епси, GIF, епуб, h, HCP , хеик, хеиф, htm, HTML, ICO, Icon, Java, жфиф, JPEG, JPG, JS, JSON, Key, log, M2TS, M4A, M4V, Markdown, MD, MEF, MOV, Movie, MP3, MP4, MP4V, МРВ, MSG, MTS, неф, НРВ, Number,, ODP,, ОГГ, в формате PICT , POTM, POTX, PPS, ppsx, ппсксм, PPT, PPTM, PPTX, PS, PS1, PSB, PSD, копировать, RAW, RB, RTF, RW1, RW2, sh,, SR2, STL, TIF, TIFF,,, ВебМ, в формате WMA, WMV, XAML, ксбм,, WMV, XML, КСКФ, КСПМ,, ямл</span><span class="sxs-lookup"><span data-stu-id="8eba3-129">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="8eba3-130">pdf</span><span class="sxs-lookup"><span data-stu-id="8eba3-130">pdf</span></span>   | <span data-ttu-id="8eba3-131">Преобразует элемент в формат PDF</span><span class="sxs-lookup"><span data-stu-id="8eba3-131">Converts the item into PDF format</span></span>  | <span data-ttu-id="8eba3-132">doc, DOCX, епуб, EML, htm, HTML, MD, MSG, ODP, ODS, ODT, PPS, ppsx, PPT, PPTX, RTF, TIF, TIFF, XLS, xlsm, XLSX</span><span class="sxs-lookup"><span data-stu-id="8eba3-132">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="8eba3-133">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8eba3-133">Optional request headers</span></span>

| <span data-ttu-id="8eba3-134">Имя</span><span class="sxs-lookup"><span data-stu-id="8eba3-134">Name</span></span>            | <span data-ttu-id="8eba3-135">Значение</span><span class="sxs-lookup"><span data-stu-id="8eba3-135">Value</span></span>   | <span data-ttu-id="8eba3-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8eba3-136">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8eba3-137">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="8eba3-137">_if-none-match_</span></span> | <span data-ttu-id="8eba3-138">String</span><span class="sxs-lookup"><span data-stu-id="8eba3-138">String</span></span>  | <span data-ttu-id="8eba3-139">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="8eba3-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="8eba3-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8eba3-140">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8eba3-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8eba3-141">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /drive/items/{item-id}/content?format={format}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8eba3-142">C#</span><span class="sxs-lookup"><span data-stu-id="8eba3-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8eba3-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8eba3-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8eba3-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8eba3-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="8eba3-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="8eba3-145">Response</span></span>

<span data-ttu-id="8eba3-146">Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.</span><span class="sxs-lookup"><span data-stu-id="8eba3-146">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="8eba3-147">Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="8eba3-147">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="8eba3-148">URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.</span><span class="sxs-lookup"><span data-stu-id="8eba3-148">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="8eba3-149">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="8eba3-149">Error responses</span></span>

<span data-ttu-id="8eba3-150">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="8eba3-150">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
