---
title: 'taskFileAttachment: createUploadSession'
description: Создайте сеанс отправки для последовательной отправки диапазонов файла в виде вложения в задачу Microsoft To Do.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a6a8aec00fcca1bbc50b25791c06db73cdd747f8
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645780"
---
# <a name="taskfileattachment-createuploadsession"></a>taskFileAttachment: createUploadSession
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте сеанс отправки для итеративной отправки диапазонов файла в виде вложения в [todoTask](../resources/todotask.md).

В рамках ответа это действие возвращает URL-адрес отправки, который можно использовать в последующих последовательных запросах `PUT` . Заголовки запросов для каждой операции `PUT` позволяют указать точный диапазон байтов для отправки. Это позволяет возобновить передачу на случай, если сетевое подключение будет удалено во время отправки.

Ниже приведены инструкции по присоединению файла к задаче Microsoft To Do с помощью сеанса отправки.

1. Создайте сеанс отправки.
2. В рамках этого сеанса отправки последовательно загружайте диапазоны байтов (до 4 МБ каждый раз), пока не будут отправлены все байты файла, а файл будет присоединен к **todoTask**.
3. Необязательно. Удалите сеанс отправки.

>**Примечание:** Используйте этот подход, чтобы вложить файл любого поддерживаемого размера от 0 МБ до 25 МБ.

Пример, описывающий сквозной процесс вложения, см. в разделе "Присоединение файлов [к задаче "Задачи"](/graph/todo-attachments).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Tasks.ReadWrite|
|Делегированные (личная учетная запись Майкрософт)|Tasks.ReadWrite|
|Для приложений|Не поддерживается.|


## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{id}/tasks/{id}/attachments/createUploadSession
POST /users/{id}/todo/lists/{id}/tasks/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление параметров в формате JSON.

В следующей таблице показан параметр, который можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|attachmentInfo|[attachmentInfo](../resources/attachmentinfo.md)|Представляет атрибуты элемента, который необходимо отправить и вложить. Укажите как минимум тип вложения (`file`), имя и размер файла.|


## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код `200 OK` отклика и новый [uploadSession](../resources/uploadsession.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса на создание сеанса отправки.
<!-- {
  "blockType": "request",
  "name": "attachmentbasethis.createuploadsession"
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

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
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