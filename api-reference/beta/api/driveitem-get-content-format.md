---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Преобразование в другие форматы
ms.openlocfilehash: 70558e7c0497c71f620481ff67b7d07cc255cd95
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209721"
---
# <a name="download-a-file-in-another-format"></a>Скачивание файла в другом формате

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

С помощью этого API вы можете получить содержимое элемента в определенном формате.
Не все файлы можно преобразовать в любые форматы.

Чтобы загрузить элемента в исходном формате, обратитесь к разделу [загрузить содержимое элемента](driveitem-get-content.md).

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


Для параметра **Формат** допустимы следующие значения:

| Значение | Описание                        | Поддерживаемые расширения источника
|:------|:-----------------------------------|---------------------------------
| командной   | Преобразует элемент в формате Командной  | здорово, fbx, obj, лист, stl, 3mf
| html  | Преобразует элемент в формате HTML | EML, md, сообщение
| JPG   | Преобразует элемент в формат JPG  | 3g 2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, правда, cpp, cr2, crw, cs, css, csv, по, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, документа, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, командной, h, hcp , heic, heif, htm, html, ico, значок, java, jfif, jpeg, jpg, js, json, ключ, журнала, m2ts, m4a, m4v, наценки, md, mef, mov, фильмов, mp3, MP4 (en), mp4v, mrw, msg, mts, nef, nrw, номера, obj, odp, odt, ogg, orf, страницы, pano, pdf, pef, php, pict, pl, лист, png, pot , potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, низкое, psd, корректировка необработанные, rb, rtf, rw1, rw2, показывать, эскиз, sql, sr2, stl, временных файлов Интернета, tiff, служб терминалов, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml
| PDF   | Преобразует элемент в формате PDF  | doc, docx, epub, eml, htm, html, md, сообщение, odp, программ ods odt, pps, ppsx, ppt, pptx, rtf, временных файлов Интернета, tiff, xls, xlsm, xlsx

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя            | Значение   | Описание                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | String  | Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`. |

## <a name="example"></a>Пример

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a>Ответ

Возвращает ответ `302 Found`, выполняющий перенаправление на URL-адрес скачивания, прошедший предварительную аутентификацию, для преобразованного файла.

Чтобы скачать преобразованный файл, ваше приложение должно следовать заголовку `Location` в ответе.

URL-адреса, прошедшие предварительную аутентификацию, действуют только в течение небольшого периода времени (несколько минут) и не требуют заголовка `Authorization` для доступа.

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a>Ошибки

Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
