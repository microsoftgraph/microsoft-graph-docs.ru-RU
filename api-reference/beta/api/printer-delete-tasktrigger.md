---
title: Удаление Тасктригжер
description: Удаление триггера задачи принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c96edf3379e1d20e35070e4e131ffb08cce98d5f
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091723"
---
# <a name="delete-tasktrigger"></a>Удаление Тасктригжер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление [триггера задачи](../resources/printtasktrigger.md) [принтера](../resources/printer.md)для предотвращения выполнения задач, связанных с печатью, на указанном принтере.

## <a name="permissions"></a>Разрешения
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| Printer. ReadWrite. ALL, Printer. FullControl. ALL |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/taskTriggers/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token}. Required. |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "delete_printer_tasktrigger"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/1a5f91a7-9bd1-4d5f-bb86-f43554cac51c/taskTriggers/25be207e-1154-491f-aa68-a9f7007d4bec
```

---

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete taskTrigger",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
