---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Преобразование в другие форматы
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8d65b7604c2ec17d4225c9cb887cbbfad2223009
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526307"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="483df-102">Скачивание файла в другом формате</span><span class="sxs-lookup"><span data-stu-id="483df-102">Download a file in another format</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="483df-103">С помощью этого API вы можете получить содержимое элемента в определенном формате.</span><span class="sxs-lookup"><span data-stu-id="483df-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="483df-104">Не все файлы можно преобразовать в любые форматы.</span><span class="sxs-lookup"><span data-stu-id="483df-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="483df-105">Чтобы загрузить элемента в исходном формате, обратитесь к разделу [загрузить содержимое элемента](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="483df-105">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="483df-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="483df-106">Prerequisites</span></span>

<span data-ttu-id="483df-107">Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.</span><span class="sxs-lookup"><span data-stu-id="483df-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="483df-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="483df-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="483df-109">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="483df-109">Query parameters</span></span>

| <span data-ttu-id="483df-110">Параметр</span><span class="sxs-lookup"><span data-stu-id="483df-110">Parameter</span></span>      | <span data-ttu-id="483df-111">Тип</span><span class="sxs-lookup"><span data-stu-id="483df-111">Type</span></span>  | <span data-ttu-id="483df-112">Описание</span><span class="sxs-lookup"><span data-stu-id="483df-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="483df-113">_format_</span><span class="sxs-lookup"><span data-stu-id="483df-113">_format_</span></span>  | <span data-ttu-id="483df-114">строка</span><span class="sxs-lookup"><span data-stu-id="483df-114">string</span></span> | <span data-ttu-id="483df-115">Укажите формат, в котором следует скачать содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="483df-115">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="483df-116">Для параметра **Формат** допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="483df-116">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="483df-117">Значение</span><span class="sxs-lookup"><span data-stu-id="483df-117">Value</span></span> | <span data-ttu-id="483df-118">Описание</span><span class="sxs-lookup"><span data-stu-id="483df-118">Description</span></span>                        | <span data-ttu-id="483df-119">Поддерживаемые расширения источника</span><span class="sxs-lookup"><span data-stu-id="483df-119">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="483df-120">командной</span><span class="sxs-lookup"><span data-stu-id="483df-120">glb</span></span>   | <span data-ttu-id="483df-121">Преобразует элемент в формате Командной</span><span class="sxs-lookup"><span data-stu-id="483df-121">Converts the item into GLB format</span></span>  | <span data-ttu-id="483df-122">здорово, fbx, obj, лист, stl, 3mf</span><span class="sxs-lookup"><span data-stu-id="483df-122">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="483df-123">html</span><span class="sxs-lookup"><span data-stu-id="483df-123">html</span></span>  | <span data-ttu-id="483df-124">Преобразует элемент в формате HTML</span><span class="sxs-lookup"><span data-stu-id="483df-124">Converts the item into HTML format</span></span> | <span data-ttu-id="483df-125">EML, md, сообщение</span><span class="sxs-lookup"><span data-stu-id="483df-125">eml, md, msg</span></span>
| <span data-ttu-id="483df-126">JPG</span><span class="sxs-lookup"><span data-stu-id="483df-126">jpg</span></span>   | <span data-ttu-id="483df-127">Преобразует элемент в формат JPG</span><span class="sxs-lookup"><span data-stu-id="483df-127">Converts the item into JPG format</span></span>  | <span data-ttu-id="483df-128">3g 2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, правда, cpp, cr2, crw, cs, css, csv, по, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, документа, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, командной, h, hcp , heic, heif, htm, html, ico, значок, java, jfif, jpeg, jpg, js, json, ключ, журнала, m2ts, m4a, m4v, наценки, md, mef, mov, фильмов, mp3, MP4 (en), mp4v, mrw, msg, mts, nef, nrw, номера, obj, odp, odt, ogg, orf, страницы, pano, pdf, pef, php, pict, pl, лист, png, pot , potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, низкое, psd, корректировка необработанные, rb, rtf, rw1, rw2, показывать, эскиз, sql, sr2, stl, временных файлов Интернета, tiff, служб терминалов, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span><span class="sxs-lookup"><span data-stu-id="483df-128">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="483df-129">PDF</span><span class="sxs-lookup"><span data-stu-id="483df-129">pdf</span></span>   | <span data-ttu-id="483df-130">Преобразует элемент в формат PDF.</span><span class="sxs-lookup"><span data-stu-id="483df-130">Converts the item into PDF format</span></span>  | <span data-ttu-id="483df-131">doc, docx, epub, eml, htm, html, md, сообщение, odp, программ ods odt, pps, ppsx, ppt, pptx, rtf, временных файлов Интернета, tiff, xls, xlsm, xlsx</span><span class="sxs-lookup"><span data-stu-id="483df-131">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="483df-132">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="483df-132">Optional request headers</span></span>

| <span data-ttu-id="483df-133">Имя</span><span class="sxs-lookup"><span data-stu-id="483df-133">Name</span></span>            | <span data-ttu-id="483df-134">Значение</span><span class="sxs-lookup"><span data-stu-id="483df-134">Value</span></span>   | <span data-ttu-id="483df-135">Описание</span><span class="sxs-lookup"><span data-stu-id="483df-135">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="483df-136">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="483df-136">_if-none-match_</span></span> | <span data-ttu-id="483df-137">String</span><span class="sxs-lookup"><span data-stu-id="483df-137">String</span></span>  | <span data-ttu-id="483df-138">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="483df-138">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="483df-139">Пример</span><span class="sxs-lookup"><span data-stu-id="483df-139">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="483df-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="483df-140">Response</span></span>

<span data-ttu-id="483df-141">Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.</span><span class="sxs-lookup"><span data-stu-id="483df-141">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="483df-142">Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="483df-142">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="483df-143">URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.</span><span class="sxs-lookup"><span data-stu-id="483df-143">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="483df-144">Ошибки</span><span class="sxs-lookup"><span data-stu-id="483df-144">Error responses</span></span>

<span data-ttu-id="483df-145">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="483df-145">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
    "Error: /api-reference/beta/api/driveitem-get-content-format.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
