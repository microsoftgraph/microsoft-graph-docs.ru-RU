---
title: Удаление вызова
description: Удаление или подвешить активный вызов.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6f409c1fe0478bc92c2b4055d2d526f1bff539aa
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64629367"
---
# <a name="delete-call"></a>Удаление вызова

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление или подвешить активный вызов. Для групповых вызовов это удаляет только ногу вызова, а в основном групповой вызов будет по-прежнему продолжаться.

## <a name="permissions"></a>Разрешения

| Тип разрешения | Разрешения (в порядке повышения привилегий)                  |
| :-------------- | :----------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается.                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                         |
| Для приложений                            | Calls.Initiate.All, Calls.AccessMedia.All |

> **Примечание:** Разрешения проверяются при вызове; При вызове этого API не проводится дополнительная проверка разрешений. Calls.AccessMedia.All необходим только для вызовов, которые используют носители с использованием приложений.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /communications/calls/{id}
```
> **Примечание.** Путь `/app` является устаревшим. В дальнейшем используйте путь `/communications`.

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже показан пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call-1"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-call-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-call-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="notification---terminating"></a>Уведомление — прекращение

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminating"
      }
    }
  ]
}
  
```

### <a name="notification---terminated"></a>Уведомление — прекращено

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": "200",
          "subcode": "5001",
          "message": "The conversation has ended."
        }
      }
    }
  ]
}
```

#### <a name="call-end-reason-codes"></a>Коды конечных причин вызова

Это некоторые из распространенных кодов ошибок, полученных с помощью уведомления при прекращении вызова.

| Код | Sub-code | Причина прекращения                                                                                 |
| :--- | :------  | :------------------------------------------------------------------------------------------------  |
| 200  | 4097     | Вызов завершился другим участником вызова.                                                   |
| 200  | 4521     | Вызов, завершившийся другим участником одноранговых вызовов.                                          |
| 200  | 5000     | Удалено из беседы другим участником.                                              |
| 200  | 5001     | Беседа завершилась.                                                                        |
| 200  | 5002     | Беседа завершилась, так как все остальные участники покинули вызов.                           |
| 200  | 5003     | Беседа завершилась.                                                                        |
| 200  | 5007     | Беседа завершилась по мере того, как инициатор группового звонка покинул беседу.               |
| 200  | 5010     | Беседа завершилась, так как в беседе остался только один участник.                   |
| 200  | 5012     | Беседа завершилась, так как в входящих реестрах нет участников.                    |
| 200  | 5013     | Беседа завершилась, так как никто другой не присоединился к групповому вызову.                               |
| 200  | 5014     | Беседа завершилась, так как нам не удалось определить потенциального хоста для группового вызова. |
| 200  | 5020     | Беседа завершилась, так как в входящих реестрах нет скрытых участников.         |
| 200  | 5030     | Беседа завершилась по мере того, как продолжительность комнаты прорыва завершилась.                              |
| 200  | 5300     | Участник был удален из беседы другим участником.                              |
| 200  | 5855     | Участник ожидания в вестибюле был удален из беседы после ожидания неактивности лобби.     |
| 200  | 7000     | Беседа завершилась ботом.                                                                 |
| 200  | 7015     | Вызов завершился по мере успешного завершения переноса.                                                 |
| 200  | 10550    | Беседа завершилась ботом.                                                                 |
| 200  | 18503    | Другой участник одноранговых зовов покинул беседу.                              |
| 200  | 540000/560000   | Вызов завершился пользователем PSTN.                                                                |
| 408  | 8537     | Keep Alive timeout, cleaned up inactive call.                                                      |
| 408  | 1106     | Подтверждение не было получено для принятия вызова в отведенное время.                  |
| 408  | 10057    | Вызов, отогнав время из-за неявки с конечных точек вызова.                                          |
| 410  | 301005   | Сбой подключения к мультимедиа.                                                                        |
| 480  | 10037    | Конечные точки вызова не найдены.                                                                    |
| 480  | 10076    | Не удалось получить вызов.                                                                       |
| 480  | 10134    | Вызов отклонен из-за невозможности маршрутить вызов.                                                  |
| 480  | 10199    | Вызов отклоняется, так как частный вызов отключен для пользователя.                                         |
| 500  | 1005     | Сервер столкнулся с ошибкой подключения к средствам массовой информации Бота. Проверьте подключение мультимедиа между Bot и Microsoft. |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


