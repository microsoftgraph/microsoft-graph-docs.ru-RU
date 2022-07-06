---
title: Перечисление объектов taskFileAttachment
description: Получение списка объектов taskFileAttachment и их свойств.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 66caaea5cf604ab85cd7e64c4a4ca088c2db2b6f
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645768"
---
# <a name="list-taskfileattachments"></a>Перечисление объектов taskFileAttachment
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [taskFileAttachment](../resources/taskfileattachment.md) и их свойств. Свойство **contentBytes** не будет возвращено в ответе. Используйте API [получения вложений](../api/attachment-get.md) для просмотра **contentBytes**.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Tasks.Read, Tasks.ReadWrite|
|Делегированные (личная учетная запись Майкрософт)|Tasks.Read, Tasks.ReadWrite|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/attachments
GET /users/{id}/todo/lists/{id}/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [taskFileAttachment](../resources/taskfileattachment.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "list_taskfileattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMehdkfuhgAAA=/tasks/AAMkAGUzY5QKjAAA=/attachments
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.taskFileAttachment",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.taskFileAttachment",
            "id": "AAMkADliMm=",
            "name": "flower.md",
            "size": 2814,
            "lastModifiedDateTime": "2022-06-09T10:40:52Z",
            "contentType": "application/octet-stream"
        },
        {
            "@odata.type": "#microsoft.graph.taskFileAttachment",
            "id": "AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwBGAAAAAADdOMUbUmCfTKa7OC-fqjkdBwBnu3olF7NfToRyJ2f__TNcAAAAAAESAABnu3olF7NfToRyJ2f__TNcAAHmG2K0AAABEgAQAFWmGvX71MhOrjRDhWM95yY=",
            "name": "tree.jpg",
            "size": 8591,
            "lastModifiedDateTime": "2022-06-09T10:40:59Z",
            "contentType": "image/jpeg"
        }
    ]
}
```
