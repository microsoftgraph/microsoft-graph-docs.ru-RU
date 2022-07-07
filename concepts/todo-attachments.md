---
title: Вложение файлов в задачу Списка дел
description: Узнайте, как вложить большие файлы в задачу Списка дел Microsoft и как выбрать правильный подход для вложения файла в задачу.
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 2d4c66a6e6e2438f1d7b7aafc6555ab701d1883a
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671362"
---
# <a name="attach-files-to-a-to-do-task"></a>Вложение файлов в задачу Списка дел

С помощью Списка дел API в Microsoft Graph, вы можете вкладывать в [задачи Списка дел](/graph/api/resources/todotask) файлы размером до 25 МБ. В зависимости от размера файла выберите один из двух способов вложения файла:
- Чтобы объединить файлы любого размера, создайте сеанс загрузки и итеративно используйте `PUT` для загрузки диапазонов байтов файла, пока не загрузите весь файл. Заголовок в итоговом успешном отклике `PUT` включает URL-адрес с ИД вложения.
- Если размер файла меньше 3 МБ, выполните однократное `POST` в свойстве навигации по **вложениям** **задачи Списка дел**; посмотрите, как это сделать [для задачи](/graph/api/todotask-post-attachments). Успешный отклик `POST` включает ИД вложенного файла.

Эта статья иллюстрирует первый подход. Вы научитесь шаг за шагом создавать и использовать сеанс отправки для добавления вложенного файла к задаче.
## <a name="step-1-create-an-upload-session"></a>Шаг 1. Создание сеанса отправки

[Создайте сеанс отправки](/graph/api/taskfileattachment-createuploadsession), чтобы вложить файл в задачу **Списка дел**. Укажите файл во входном параметре [attachmentInfo](/graph/api/resources/attachmentinfo).

После успешной операции возвращается `HTTP 201 Created` и новый экземпляр объекта [uploadSession](/graph/api/resources/uploadsession), содержащий непрозрачный URL-адрес, который можно использовать в последующих операциях `PUT` для отправки частей этого файла. Этот экземпляр **uploadSession** предоставляет временное место хранения, где байты файла сохраняются до отправки всего файла.

Объект **uploadSession** в ответе также включает свойство **nextExpectedRanges**, указывающее, что исходное начальное расположение загрузки должно быть байтом `0`.

### <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Tasks.ReadWrite|
|Делегированные (личная учетная запись Майкрософт)|Tasks.ReadWrite|
|Для приложений|Не поддерживается.|

### <a name="example-create-an-upload-session-for-a-todotask"></a>Пример: создание сеанса отправки для задачи Списка дел

#### <a name="request"></a>Запрос

Ниже приведен пример запроса на создание сеанса отправки.
<!-- {
  "blockType": "request",
  "name": "todo_attachment_walkthrough_createuploadsession"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachments/createUploadSession
Content-Type: application/json

{
  "attachmentInfo": {
    "@odata.type": "microsoft.graph.attachmentInfo",
    "attachmentType": "file",
    "name": "flower",
    "size": 3483322
  }
}
```

#### <a name="response"></a>Отклик
В следующем примере показан ресурс **uploadSession**, возвращенный для задачи в тексте отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=",
    "expirationDateTime": "2022-06-09T10:45:27.4324526Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

## <a name="step-2-use-the-upload-session-to-upload-a-range-of-bytes-of-the-file"></a>Шаг 2. Отправка диапазона байтов файла с помощью сеанса отправки

Чтобы отправить файл или часть файла, выполните запрос `PUT` к URL-адресу, возвращенному на шаге 1 в свойстве **uploadUrl** ресурса **uploadSession**. Можно отправить файл целиком или разделить файл на несколько диапазонов байтов. Каждый диапазон байтов должен быть менее 4 МБ.

Укажите заголовки и текст запроса, как описано в следующих разделах.

### <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
|Авторизация | String | Bearer {token}. Обязательный. |
| Content-Length | Int32 | Количество байтов, отправляемых в этой операции. Верхний предел числа байтов для каждой операции `PUT` составляет 4 МБ. Запрос завершится сбоем для всего, что превышает 4 МБ. Обязательный элемент. |
| Content-Range | String | Диапазон байтов файла, отправляемого в этой операции, начиная с байта 0, выраженный в формате `bytes {start}-{end}/{total}`. Обязательно. |
| Content-Type | String  | Тип MIME. Укажите `application/octet-stream`. Обязательный элемент. |


### <a name="request-body"></a>Основной текст запроса

Укажите фактические байты вкладываемого файла, находящиеся в диапазоне расположения, указанном в заголовке запроса `Content-Range`.

### <a name="response"></a>Отклик
Успешная отправка возвращает код отклика `HTTP 200 OK` и объект **uploadSession**. Объект отклика имеет указанные ниже свойства.

- Значение свойства **expirationDateTime** остается тем же, что было возвращено исходным **uploadSession** на шаге 1.
- **nextExpectedRanges** указывает расположение следующего байта для начала загрузки, например, `"nextExpectedRanges":["2097152"]`. Байты файла необходимо отправлять по порядку.
<!-- The **nextExpectedRanges** specifies one or more byte ranges, each indicating the starting point of a subsequent `PUT` request:

  - On a successful upload, this property returns the next range to start from, for example, `"nextExpectedRanges":["2097152"]`.
  - If a portion of a byte range has not uploaded successfully, this property includes the byte range with the start and end locations, for example, `"nextExpectedRanges":["1998457-2097094"]`.
-->
- Свойство **uploadUrl** не возвращается явно, так как все операции сеанса загрузки `PUT` используют один и тот же URL-адрес, возвращаемый при создании сеанса (шаг 1).

### <a name="example-first-upload-to-the-todotask"></a>Пример: первая загрузка в задачу Списка дел

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=/content
Content-Type: application/octet-stream
Content-Length: 2097152
Content-Range: bytes 0-2097151/3483322

{
  <bytes 0-2097151 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>Отклик

Следующий пример ответа показывает в свойстве **nextExpectedRanges** начало следующего диапазона байтов, ожидаемого сервером.
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "ExpirationDateTime":"2022-06-09T10:45:27.4324526Z",
  "NextExpectedRanges":["2097152"]
}
```

## <a name="step-3-continue-uploading-byte-ranges-until-the-entire-file-has-been-uploaded"></a>Шаг 3. Продолжение отправки диапазонов байтов вплоть до отправки всего файла

После первоначальной отправки на шаге 2 продолжайте отправлять оставшиеся части файла, используя аналогичный запрос `PUT`, как описано на шаге 2, до достижения даты и времени окончания срока действия сеанса. Используйте коллекцию **nextExpectedRanges**, чтобы определить, с чего начать отправку следующего диапазона байтов. Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером. Это удобно, когда требуется возобновить прерванную передачу, а клиенту неизвестно состояние службы.

После успешной отправки последнего байта файла операция `PUT` возвращает `HTTP 201 Created` и заголовок `Location`, указывающий URL-адрес вложенного файла. Можно получить ИД вложения по этому URL-адресу и сохранить его для дальнейшего использования.

В следующих примерах покажите, как отправить последний диапазон в файл **задачи Списка дел** на предыдущих шагах.

### <a name="example-final-upload-to-the-todotask"></a>Пример: окончательная отправка в задачу Списка дел

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored"
}-->
```http
PUT https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=/content
Content-Type: application/octet-stream
Content-Length: 1386170
Content-Range: bytes 2097152-3483321/3483322

{
  <bytes 2097152-3483321 of the file to be attached, in binary format>
}
```

#### <a name="response"></a>Отклик
Ниже приведен пример отклика, в котором показан заголовок отклика `Location`, из которого можно сохранить идентификатор вложения (`AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=`) для последующего использования.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 201 Created

Location: https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/Attachments/AAMkADI5MAAIT3drCAAABEgAQANAqbAe7qaROhYdTnUQwXm0=
Content-Length: 0
```

## <a name="alternative-step-cancel-the-upload-session"></a>Альтернатива: отмена сеанса отправки
Если необходимо отменить отправку в любое время до окончания срока действия сеанса отправки, можно использовать тот же самый начальный URL-адрес для удаления сеанса отправки. Успешная операция возвращает код отклика HTTP `204 No Content`.

### <a name="example-cancel-the-upload-session"></a>Пример: отмена сеанса отправки

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/6f9a2a92-8527-4d64-837e-b5312852f36d/todo/lists/AAMDiFkfh=/tasks/AAMkADliMm=/attachmentSessions/AAMkADliMm=
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 204 No content
```

