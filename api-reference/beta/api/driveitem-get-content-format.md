---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Преобразование в другие форматы
localization_priority: Normal
ms.openlocfilehash: d27420153a295eac9d3f880910d63bd701525427
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887439"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="3a2f5-102">Скачивание файла в другом формате</span><span class="sxs-lookup"><span data-stu-id="3a2f5-102">Download a file in another format</span></span>

> <span data-ttu-id="3a2f5-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a2f5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a2f5-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a2f5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a2f5-105">С помощью этого API вы можете получить содержимое элемента в определенном формате.</span><span class="sxs-lookup"><span data-stu-id="3a2f5-105">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="3a2f5-106">Не все файлы можно преобразовать в любые форматы.</span><span class="sxs-lookup"><span data-stu-id="3a2f5-106">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="3a2f5-107">Чтобы загрузить элемента в исходном формате, обратитесь к разделу [загрузить содержимое элемента](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="3a2f5-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a2f5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a2f5-108">Prerequisites</span></span>

<span data-ttu-id="3a2f5-109">Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.</span><span class="sxs-lookup"><span data-stu-id="3a2f5-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="3a2f5-110">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a2f5-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="3a2f5-111">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="3a2f5-111">Query parameters</span></span>

| <span data-ttu-id="3a2f5-112">Параметр</span><span class="sxs-lookup"><span data-stu-id="3a2f5-112">Parameter</span></span>      | <span data-ttu-id="3a2f5-113">Тип</span><span class="sxs-lookup"><span data-stu-id="3a2f5-113">Type</span></span>  | <span data-ttu-id="3a2f5-114">Описание</span><span class="sxs-lookup"><span data-stu-id="3a2f5-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="3a2f5-115">_format_</span><span class="sxs-lookup"><span data-stu-id="3a2f5-115">_format_</span></span>  | <span data-ttu-id="3a2f5-116">строка</span><span class="sxs-lookup"><span data-stu-id="3a2f5-116">string</span></span> | <span data-ttu-id="3a2f5-117">Укажите формат, в котором следует скачать содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="3a2f5-117">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="3a2f5-118">Для параметра **Формат** допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="3a2f5-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="3a2f5-119">Значение</span><span class="sxs-lookup"><span data-stu-id="3a2f5-119">Value</span></span> | <span data-ttu-id="3a2f5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3a2f5-120">Description</span></span>                        | <span data-ttu-id="3a2f5-121">Поддерживаемые расширения источника</span><span class="sxs-lookup"><span data-stu-id="3a2f5-121">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="3a2f5-122">командной</span><span class="sxs-lookup"><span data-stu-id="3a2f5-122">glb</span></span>   | <span data-ttu-id="3a2f5-123">Преобразует элемент в формате Командной</span><span class="sxs-lookup"><span data-stu-id="3a2f5-123">Converts the item into GLB format</span></span>  | <span data-ttu-id="3a2f5-124">здорово, fbx, obj, лист, stl, 3mf</span><span class="sxs-lookup"><span data-stu-id="3a2f5-124">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="3a2f5-125">html</span><span class="sxs-lookup"><span data-stu-id="3a2f5-125">html</span></span>  | <span data-ttu-id="3a2f5-126">Преобразует элемент в формате HTML</span><span class="sxs-lookup"><span data-stu-id="3a2f5-126">Converts the item into HTML format</span></span> | <span data-ttu-id="3a2f5-127">EML, md, сообщение</span><span class="sxs-lookup"><span data-stu-id="3a2f5-127">eml, md, msg</span></span>
| <span data-ttu-id="3a2f5-128">JPG</span><span class="sxs-lookup"><span data-stu-id="3a2f5-128">jpg</span></span>   | <span data-ttu-id="3a2f5-129">Преобразует элемент в формат JPG</span><span class="sxs-lookup"><span data-stu-id="3a2f5-129">Converts the item into JPG format</span></span>  | <span data-ttu-id="3a2f5-130">3g 2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, правда, cpp, cr2, crw, cs, css, csv, по, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, документа, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, командной, h, hcp , heic, heif, htm, html, ico, значок, java, jfif, jpeg, jpg, js, json, ключ, журнала, m2ts, m4a, m4v, наценки, md, mef, mov, фильмов, mp3, MP4 (en), mp4v, mrw, msg, mts, nef, nrw, номера, obj, odp, odt, ogg, orf, страницы, pano, pdf, pef, php, pict, pl, лист, png, pot , potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, низкое, psd, корректировка необработанные, rb, rtf, rw1, rw2, показывать, эскиз, sql, sr2, stl, временных файлов Интернета, tiff, служб терминалов, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span><span class="sxs-lookup"><span data-stu-id="3a2f5-130">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="3a2f5-131">PDF</span><span class="sxs-lookup"><span data-stu-id="3a2f5-131">pdf</span></span>   | <span data-ttu-id="3a2f5-132">Преобразует элемент в формате PDF</span><span class="sxs-lookup"><span data-stu-id="3a2f5-132">Converts the item into PDF format</span></span>  | <span data-ttu-id="3a2f5-133">doc, docx, epub, eml, htm, html, md, сообщение, odp, программ ods odt, pps, ppsx, ppt, pptx, rtf, временных файлов Интернета, tiff, xls, xlsm, xlsx</span><span class="sxs-lookup"><span data-stu-id="3a2f5-133">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="3a2f5-134">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a2f5-134">Optional request headers</span></span>

| <span data-ttu-id="3a2f5-135">Имя</span><span class="sxs-lookup"><span data-stu-id="3a2f5-135">Name</span></span>            | <span data-ttu-id="3a2f5-136">Значение</span><span class="sxs-lookup"><span data-stu-id="3a2f5-136">Value</span></span>   | <span data-ttu-id="3a2f5-137">Описание</span><span class="sxs-lookup"><span data-stu-id="3a2f5-137">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3a2f5-138">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="3a2f5-138">_if-none-match_</span></span> | <span data-ttu-id="3a2f5-139">String</span><span class="sxs-lookup"><span data-stu-id="3a2f5-139">String</span></span>  | <span data-ttu-id="3a2f5-140">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="3a2f5-140">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="3a2f5-141">Пример</span><span class="sxs-lookup"><span data-stu-id="3a2f5-141">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="3a2f5-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a2f5-142">Response</span></span>

<span data-ttu-id="3a2f5-143">Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.</span><span class="sxs-lookup"><span data-stu-id="3a2f5-143">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="3a2f5-144">Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.</span><span class="sxs-lookup"><span data-stu-id="3a2f5-144">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="3a2f5-145">URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.</span><span class="sxs-lookup"><span data-stu-id="3a2f5-145">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="3a2f5-146">Ошибки</span><span class="sxs-lookup"><span data-stu-id="3a2f5-146">Error responses</span></span>

<span data-ttu-id="3a2f5-147">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="3a2f5-147">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
