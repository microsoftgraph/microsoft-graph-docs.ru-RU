---
title: Удаление Алловедграуп
description: Отозвать доступ указанной группы, чтобы отправить задания печати на соответствующий общий ресурс принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e6c3fb214126d4414ed35d6ba58a52acc6b65bab
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216622"
---
# <a name="delete-allowedgroup"></a>Удаление Алловедграуп

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отозвать доступ указанной группы, чтобы послать задания печати в связанный [принтершаре](../resources/printershare.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| Users. Read. ALL |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Сервер приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{id}/allowedGroups/{id}/$ref
```
## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "delete_allowedgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/shares/{id}/allowedGroup/{id}/$ref
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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
  "description": "Delete allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->