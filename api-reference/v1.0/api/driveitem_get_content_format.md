---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Преобразование в другие форматы"
ms.openlocfilehash: 3031500beaec2d765075abfd925a6333f50368f9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="download-a-file-in-another-format"></a>Скачивание файла в другом формате

С помощью этого API вы можете получить содержимое элемента в определенном формате.
Не все файлы можно преобразовать в любые форматы.

Сведения о том, как скачать элемент в его исходном формате, см. в статье о [скачивании содержимого элемента](driveitem_get_content.md).

## <a name="prerequisites"></a>Необходимые компоненты

Чтобы можно было вызвать этот API, пользователю необходимо предоставить приложению доступ на чтение к файлу, который это приложение собирается преобразовать.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

### <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя            | Значение   | Описание                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | String  | Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`. |


### <a name="query-string-parameters"></a>Параметры строки запроса

| Имя      | Значение  | Описание                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| _format_  | строка | Укажите формат, в котором следует скачать содержимое элемента. |


Для параметра **convert** допустимы указанные ниже значения.

| Значение   | Описание                        | Поддерживаемые расширения источника |
|:--------|:-----------------------------------|-----------------------------|
| **pdf** | Преобразует элемент в формат PDF. | csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx | 

### <a name="example"></a>Пример

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

[error-response]: ../../../concepts/errors.md
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
