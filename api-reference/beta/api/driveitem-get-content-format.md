---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Преобразование в другие форматы
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ea4061187ea9890a75a85cef2122a2ec7e280920
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325286"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="6b20d-102">Скачивание файла в другом формате</span><span class="sxs-lookup"><span data-stu-id="6b20d-102">Download a file in another format</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b20d-103">С помощью этого API вы можете получить содержимое элемента в определенном формате.</span><span class="sxs-lookup"><span data-stu-id="6b20d-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="6b20d-104">Не все файлы можно преобразовать в любые форматы.</span><span class="sxs-lookup"><span data-stu-id="6b20d-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="6b20d-105">Сведения о том, как скачать элемент в его исходном формате, см. в статье о [скачивании содержимого элемента](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="6b20d-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b20d-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6b20d-106">Prerequisites</span></span>

<span data-ttu-id="6b20d-107">Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.</span><span class="sxs-lookup"><span data-stu-id="6b20d-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="6b20d-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b20d-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="6b20d-109">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="6b20d-109">Query parameters</span></span>

| <span data-ttu-id="6b20d-110">Параметр</span><span class="sxs-lookup"><span data-stu-id="6b20d-110">Parameter</span></span>      | <span data-ttu-id="6b20d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6b20d-111">Type</span></span>  | <span data-ttu-id="6b20d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6b20d-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="6b20d-113">_format_</span><span class="sxs-lookup"><span data-stu-id="6b20d-113">_format_</span></span>  | <span data-ttu-id="6b20d-114">строка</span><span class="sxs-lookup"><span data-stu-id="6b20d-114">string</span></span> | <span data-ttu-id="6b20d-115">Укажите формат, в котором следует скачать содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="6b20d-115">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="6b20d-116">Для параметра **format** допустимы указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="6b20d-116">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="6b20d-117">Значение</span><span class="sxs-lookup"><span data-stu-id="6b20d-117">Value</span></span> | <span data-ttu-id="6b20d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="6b20d-118">Description</span></span>                        | <span data-ttu-id="6b20d-119">Поддерживаемые расширения источника</span><span class="sxs-lookup"><span data-stu-id="6b20d-119">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="6b20d-120">ГЛБ</span><span class="sxs-lookup"><span data-stu-id="6b20d-120">glb</span></span>   | <span data-ttu-id="6b20d-121">Преобразует элемент в формат ГЛБ</span><span class="sxs-lookup"><span data-stu-id="6b20d-121">Converts the item into GLB format</span></span>  | <span data-ttu-id="6b20d-122">крутой, фбкс, obj, лист, STL, 3mf</span><span class="sxs-lookup"><span data-stu-id="6b20d-122">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="6b20d-123">html</span><span class="sxs-lookup"><span data-stu-id="6b20d-123">html</span></span>  | <span data-ttu-id="6b20d-124">Преобразует элемент в формат HTML</span><span class="sxs-lookup"><span data-stu-id="6b20d-124">Converts the item into HTML format</span></span> | <span data-ttu-id="6b20d-125">EML, MD, MSG</span><span class="sxs-lookup"><span data-stu-id="6b20d-125">eml, md, msg</span></span>
| <span data-ttu-id="6b20d-126">JPEG</span><span class="sxs-lookup"><span data-stu-id="6b20d-126">jpg</span></span>   | <span data-ttu-id="6b20d-127">Преобразует элемент в формат JPG</span><span class="sxs-lookup"><span data-stu-id="6b20d-127">Converts the item into JPG format</span></span>  | <span data-ttu-id="6b20d-128">3G2, 3GP, 3GP2, 3GPP, 3mf, AI, АРВ, ASF, AVI, BAS, bash, bat, BMP, c, КБЛ, cmd, Cool, CPP, CR2, КРВ, CS, CSS, CSV, cur, DCM, dcm30, DIC, ДИКМ, DICOM, ДНГ, doc, DOCX, DWG, EML, EPI,, епсф, епси, GIF, епуб, h, HCP , хеик, хеиф, htm, HTML, ICO, Icon, Java, жфиф, JPEG, JPG, JS, JSON, Key, log, M2TS, M4A, M4V, Markdown, MD, MEF, MOV, Movie, MP3, MP4, MP4V, МРВ, MSG, MTS, неф, НРВ, Number,, ODP,, ОГГ, в формате PICT , POTM, POTX, PPS, ppsx, ппсксм, PPT, PPTM, PPTX, PS, PS1, PSB, PSD, копировать, RAW, RB, RTF, RW1, RW2, sh,, SR2, STL, TIF, TIFF,,, ВебМ, в формате WMA, WMV, XAML, ксбм,, WMV, XML, КСКФ, КСПМ,, ямл</span><span class="sxs-lookup"><span data-stu-id="6b20d-128">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="6b20d-129">pdf</span><span class="sxs-lookup"><span data-stu-id="6b20d-129">pdf</span></span>   | <span data-ttu-id="6b20d-130">Преобразует элемент в формат PDF</span><span class="sxs-lookup"><span data-stu-id="6b20d-130">Converts the item into PDF format</span></span>  | <span data-ttu-id="6b20d-131">doc, DOCX, епуб, EML, htm, HTML, MD, MSG, ODP, ODS, ODT, PPS, ppsx, PPT, PPTX, RTF, TIF, TIFF, XLS, xlsm, XLSX</span><span class="sxs-lookup"><span data-stu-id="6b20d-131">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="6b20d-132">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b20d-132">Optional request headers</span></span>

| <span data-ttu-id="6b20d-133">Имя</span><span class="sxs-lookup"><span data-stu-id="6b20d-133">Name</span></span>            | <span data-ttu-id="6b20d-134">Значение</span><span class="sxs-lookup"><span data-stu-id="6b20d-134">Value</span></span>   | <span data-ttu-id="6b20d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="6b20d-135">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6b20d-136">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="6b20d-136">_if-none-match_</span></span> | <span data-ttu-id="6b20d-137">String</span><span class="sxs-lookup"><span data-stu-id="6b20d-137">String</span></span>  | <span data-ttu-id="6b20d-138">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="6b20d-138">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="6b20d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="6b20d-139">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="6b20d-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b20d-140">Response</span></span>

<span data-ttu-id="6b20d-141">Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.</span><span class="sxs-lookup"><span data-stu-id="6b20d-141">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="6b20d-142">Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="6b20d-142">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="6b20d-143">URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.</span><span class="sxs-lookup"><span data-stu-id="6b20d-143">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="6b20d-144">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="6b20d-144">Error responses</span></span>

<span data-ttu-id="6b20d-145">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="6b20d-145">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!--
{
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": []
}
-->
