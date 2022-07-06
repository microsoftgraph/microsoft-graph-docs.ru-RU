---
title: Создание taskFileAttachment
description: Добавьте новый объект taskFileAttachment в todoTask.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 590e8912178cdbc6eb0c2ed9f756ff2a77e84f9e
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645750"
---
# <a name="create-taskfileattachment"></a>Создание taskFileAttachment
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавьте новый [объект taskFileAttachment](../resources/taskfileattachment.md) в [todoTask](../resources/todotask.md).

Эта операция ограничивает размер вложения, которое можно добавить, до 3 МБ. Если размер вложений файлов превышает 3 [МБ,](../api/taskfileattachment-createuploadsession.md) создайте сеанс отправки для отправки вложений.


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
POST /me/todo/lists/{id}/tasks/{id}/attachments
POST /users/{id}/todo/lists/{id}/tasks/{id}/attachments
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [taskFileAttachment](../resources/taskfileattachment.md) в формате JSON.

При создании вложения в файл включите `"@odata.type": "#microsoft.graph.taskFileAttachment"` и требуемые свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|contentBytes|Двоичный|Содержимое файла в кодировке base64. Обязательный.|
|contentType|String|Тип контента этого вложения. |
|name|String|Имя текста, отображаемого под значком, представляющий внедренное вложение. Он может не быть фактическим именем файла. Обязательный. |
|size|Int32|Размер вложения в байтах. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [taskFileAttachment](../resources/taskfileattachment.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_taskFileAttachment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/AAMkpsDRVK=/tasks/AAKdfjhgsjhgJ=/attachments
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.taskFileAttachment",
  "name": "smile",
  "contentBytes": "a0b1c76de9f7=",
  "contentType": "image/gif"
}
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
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.taskFileAttachment",
  "id": "AAMkADNkN2R",
  "lastModifiedDateTime": "2017-01-26T08:48:28Z",
  "name": "smile",
  "contentType": "image/gif",
  "size": 1008
}
```

