---
title: Получение taskFileAttachment
description: Чтение свойств и связей объекта taskFileAttachment.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0a269e67fd3305aa12e3492609d8d672f6c49f69
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645774"
---
# <a name="get-taskfileattachment"></a>Получение taskFileAttachment
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Чтение свойств и связей объекта [taskFileAttachment](../resources/taskfileattachment.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Tasks.Read, Tasks.ReadWrite|
|Делегированные (личная учетная запись Майкрософт)|Tasks.Read, Tasks.ReadWrite|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
Чтобы получить файл, вложенный в [todoTask](../resources/todotask.md):
 
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /me/todo/lists/{id}/tasks/{id}/attachments/{id}
GET /users/{id}/todo/lists/{id}/tasks/{id}/attachments/{id}
```

Для получения необработанного содержимого вложения файла (тип контента основан на исходном типе содержимого файла):
<!-- {
  "blockType": "ignored"
}
-->
``http
GET /me/todo/lists/{id}/tasks/{id}/attachments/{id}/$value
GET /users/{id}/todo/lists/{id}/tasks/{id}/attachments/{id}/$value
``

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект [taskFileAttachment](../resources/taskfileattachment.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_taskfileattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMehdkfuhgAAA=/tasks/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.taskFileAttachment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.taskFileAttachment",
    "id": "AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=",
    "lastModifiedDateTime": "2021-04-02T03:41:29Z",
    "name": "Q1 Planning.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 29068,
    "contentBytes": "UEsDBBQABgAIAAAAIQ4AAAAA"
  }
}
```

