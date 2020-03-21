---
title: Удаление Принтершаре
description: Удаление общего принтера (отменяйте общий доступ к связанному принтеру). Это действие невозможно отменить. Если к принтеру предоставлен общий доступ в будущем, все пользователи Windows, на которых ранее устанавливался принтер, должны обнаружить и повторно установить его.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 534dc61037efd99f92100c87bc911cdea6dfb6a5
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896212"
---
# <a name="delete-printershare"></a>Удаление Принтершаре

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление общего принтера (отменяйте общий доступ к связанному [принтеру](../resources/printer.md)). Это действие невозможно отменить. Если к [принтеру](../resources/printer.md) предоставлен общий доступ в будущем, все пользователи Windows, на которых ранее устанавливался [принтер](../resources/printer.md) , должны обнаружить и переустановить его.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| Users. Read. ALL |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложения|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShares/{id}
DELETE /print/printers/{id}/share
```
## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printerShares/{id}
```
##### <a name="response"></a>Отклик
Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->