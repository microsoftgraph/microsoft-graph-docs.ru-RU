---
author: JeremyKelley
description: С помощью этого API вы можете получить содержимое элемента в определенном формате.
ms.date: 09/10/2017
title: Преобразование в другие форматы
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: eaa5dc018d74de4cea4a07ba9ae05f5d26adda0c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019899"
---
# <a name="download-a-file-in-another-format"></a>Скачивание файла в другом формате

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [tls-1.2-required](../../includes/tls-1.2-required.md)]

С помощью этого API вы можете получить содержимое элемента в определенном формате. Не все файлы можно преобразовать в любые форматы.

Сведения о том, как скачать элемент в его исходном формате, см. в статье о [скачивании содержимого элемента](driveitem-get-content.md).

## <a name="prerequisites"></a>Необходимые компоненты

Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a>Параметры запроса

| Параметр      | Тип  | Описание                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| _format_  | строка | Укажите формат, в котором следует скачать содержимое элемента. |


Для параметра **format** допустимы указанные ниже значения.

| Значение | Описание                        | Поддерживаемые расширения источника
|:------|:-----------------------------------|---------------------------------
| glb   | Преобразует элемент в формат GLB  | COOL, FBX, OBJ, PLY, STL, 3MF
| html  | Преобразует элемент в формат HTML | EML, MD, MSG
| jpg   | Преобразует элемент в формат JPG  | 3G2, 3GP, 3GP2, 3GPP, 3MF, AI, ARW, ASF, AVI, BAS, BASH, BAT, BMP, C, CBL, CMD, COOL, CPP, CR2, CRW, CS, CSS, CSV, CUR, DCM, DCM30, DIC, DICM, DICOM, DNG, DOC, DOCX, DWG, EML, EPI, EPS, EPSF, EPSI, EPUB, ERF, FBX, FPPX, GIF, GLB, H, HCP, HEIC, HEIF, HTM, HTML, ICO, ICON, JAVA, JFIF, JPEG, JPG, JS, JSON, KEY, LOG, M2TS, M4A, M4V, MARKDOWN, MD, MEF, MOV, MOVIE, MP3, MP4, MP4V, MRW, MSG, MTS, NEF, NRW, NUMBERS, OBJ, ODP, ODT, OGG, ORF, PAGES, PANO, PDF, PEF, PHP, PICT, PL, PLY, PNG, POT, POTM, POTX, PPS, PPSX, PPSXM, PPT, PPTM, PPTX, PS, PS1, PSB, PSD, PY, RAW, RB, RTF, RW1, RW2, SH, SKETCH, SQL, SR2, STL, TIF, TIFF, TS, TXT, VB, WEBM, WMA, WMV, XAML, XBM, XCF, XD, XML, XPM, YAML, YML
| pdf   | Преобразует элемент в формат PDF  | DOC, DOCX, EPUB, EML, HTM, HTML, MD, MSG, ODP, ODS, ODT, PPS, PPSX, PPT, PPTX, RTF, TIF, TIFF, XLS, XLSM, XLSX

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя            | Значение   | Описание                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | String  | Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`. |

## <a name="example"></a>Пример


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /drive/items/{item-id}/content?format={format}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/convert-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/convert-item-content-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>Отклик

Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.

Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.

URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a>Ответы с ошибками

Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].

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


