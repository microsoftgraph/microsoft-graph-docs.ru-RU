---
title: 'Call: keepAlive'
description: Сделайте запрос к этому API каждые 15 – 45 минут, чтобы убедиться, что текущий вызов остается активным.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 50eec71f674f9f2dfaef1e405b7261c47199f5e6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871911"
---
# <a name="call-keepalive"></a>Call: keepAlive

Сделайте запрос к этому API каждые 15 – 45 минут, чтобы убедиться, что текущий вызов остается активным. Вызов, не получающий этот запрос в течение 45 минут, считается неактивным и позднее завершается.

По крайней мере один успешный запрос должен быть выполнен в течение 45 минут предыдущего запроса или с начала вызова.

Мы рекомендуем отправлять запрос через более короткие интервалы времени (каждые 15 минут). Убедитесь, что эти запросы выполнены успешно, чтобы предотвратить истечение времени и завершения вызова.

Попытка отправить запрос на уже завершенный вызов приведет к `404 Not-Found` ошибке. Ресурсы, связанные с вызовом, необходимо очистить на стороне приложения.

## <a name="permissions"></a>Permissions
Для вызова этого API может потребоваться одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| :-------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается        |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается        |
| Приложение     | Нет.                                        |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/keepAlive
```


## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
Этот метод возвращает код `200 OK` HTTP-ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "keep-alive"
}-->

```http
POST https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive
```

### <a name="response"></a>Отклик
Ниже приводится пример отклика.
<!-- {
  "blockType": "response",
  "name": "keep-alive",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 200 OK
```


<!--
{
  "type": "#page.annotation",
  "description": "call: keepAlive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
