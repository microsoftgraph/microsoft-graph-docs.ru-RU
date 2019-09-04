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
# <a name="download-a-file-in-another-format"></a>Скачивание файла в другом формате

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

С помощью этого API вы можете получить содержимое элемента в определенном формате.
Не все файлы можно преобразовать в любые форматы.

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
| глб   | Преобразует элемент в формат ГЛБ  | крутой, фбкс, obj, лист, STL, 3mf
| html  | Преобразует элемент в формат HTML | EML, MD, MSG
| JPEG   | Преобразует элемент в формат JPG  | 3G2, 3GP, 3GP2, 3GPP, 3mf, AI, АРВ, ASF, AVI, BAS, bash, bat, BMP, c, КБЛ, cmd, Cool, CPP, CR2, КРВ, CS, CSS, CSV, cur, DCM, dcm30, DIC, ДИКМ, DICOM, ДНГ, doc, DOCX, DWG, EML, EPI,, епсф, епси, GIF, епуб, h, HCP , хеик, хеиф, htm, HTML, ICO, Icon, Java, жфиф, JPEG, JPG, JS, JSON, Key, log, M2TS, M4A, M4V, Markdown, MD, MEF, MOV, Movie, MP3, MP4, MP4V, МРВ, MSG, MTS, неф, НРВ, Number,, ODP,, ОГГ, в формате PICT , POTM, POTX, PPS, ppsx, ппсксм, PPT, PPTM, PPTX, PS, PS1, PSB, PSD, копировать, RAW, RB, RTF, RW1, RW2, sh,, SR2, STL, TIF, TIFF,,, ВебМ, в формате WMA, WMV, XAML, ксбм,, WMV, XML, КСКФ, КСПМ,, ямл
| pdf   | Преобразует элемент в формат PDF  | doc, DOCX, епуб, EML, htm, HTML, MD, MSG, ODP, ODS, ODT, PPS, ppsx, PPT, PPTX, RTF, TIF, TIFF, XLS, xlsm, XLSX

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя            | Значение   | Описание                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | String  | Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`. |

## <a name="example"></a>Пример


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /drive/items/{item-id}/content?format={format}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>Ответ

Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.

Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.

URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a>Ответы с ошибками

Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].

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
