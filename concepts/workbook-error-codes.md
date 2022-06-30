---
title: Коды ошибок для API книг и диаграмм
description: Перечисляет и описывает коды ошибок, возвращаемые API книг и диаграмм в Microsoft Graph при сбое запроса, отправленного через API.
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: d51b2da336e5d27177f654dfff25c86adcd0dd79
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555858"
---
# <a name="error-codes-for-workbooks-and-charts-apis"></a>Коды ошибок для API книг и диаграмм

В этой статье описываются коды ошибок, возвращаемые книгами и API диаграмм в Microsoft Graph при сбое запроса, отправленного через эти API. Дополнительные сведения об обработке ответов на ошибки из книг и API диаграмм в Microsoft Graph см. в разделе "Обработка ошибок для [API Excel" в Microsoft Graph](workbook-error-handling.md). Дополнительные сведения об ответах на ошибки и типах ресурсов в Microsoft Graph см. в ответах на ошибки [и типах ресурсов Microsoft Graph](errors.md).

## <a name="error-codes-and-messages"></a>Коды ошибок и сообщения

В следующей таблице перечислены текущие коды ошибок и сообщения. Служба может в любое время добавить новые коды ошибок.

| Код состояния | Код ошибки            | Сообщение об ошибке                                                                                                                     |
|:------------|:----------------------|:----------------------------------------------------------------------------------------------------------------------------------|
| 400         | `badRequest`          | Запрос имеет неправильный формат или содержит ошибку.                                                                                            |
| 401         | `unauthorized`        | Вызывающая сторона не прошла проверку подлинности.                                                                                                  |
| 403         | `forbidden`           | У вызывающей стороны нет разрешения на выполнение действия.                                                                         |
| 404         | `notFound`            | Не удалось найти ресурс.                                                                                                  |
| 405         | `methodNotAllowed`    | Метод HTTP в запросе недопустим для ресурса.                                                                    |
| 409         | `conflict`            | Текущее состояние противоречит ожидаемым результатам запроса.                                                                        |
| 413         | `payloadTooLarge`     | Размер запроса превышает максимальное значение.                                                                                       |
| 429         | `tooManyRequests`     | Действия приложения или пользователя превысили ограничения.                                                                                               |
| 500         | `internalServerError` | При обработке запроса произошла внутренняя ошибка сервера.                                                                   |
| 501         | `notImplemented`      | Запрашиваемая функция не реализована.                                                                                          |
| 502         | `badGateway`          | Сервер обнаружил временную ошибку и не удалось выполнить запрос.                                                     |
| 503         | `serviceUnavailable`  | Служба недоступна. Повторите запрос.                                                                      |
| 504         | `gatewayTimeout`      | Сервер, выступающий в качестве прокси-сервера, не получает от вышестоящего сервера во времени ответ для выполнения запроса. |

## <a name="detailed-error-codes"></a>Подробные коды ошибок

Ниже приведены обязательные коды ошибок, с которыми приложение может столкнуться на первом уровне вложенных **объектов innerError** . Служба может в любое время добавить новые коды ошибок.

- `accessConflict`
- `badRequestUncategorized`
- `conflictUncategorized`
- `forbiddenUncategorized`
- `gatewayTimeoutUncategorized`
- `internalServerErrorUncategorized`
- `invalidSessionAccessConflict`
- `invalidSessionAuthentication`
- `invalidSessionNotFound`
- `invalidSessionReCreatable`
- `invalidSessionRestricted`
- `invalidSessionUnexpected`
- `invalidSessionUnsupportedWorkbook`
- `methodNotAllowedUncategorized`
- `notFoundUncategorized`
- `notImplementedUncategorized`
- `payloadTooLargeUncategorized`
- `serviceUnavailableUncategorized`
- `tooManyRequestsUncategorized`
- `transientFailure`
- `unauthorizedUncategorized`
- `unsupportedWorkbook`

Примеры необязательных кодов ошибок на первом уровне вложенных объектов **innerError** см. в дополнительных примерах кода ошибок [второго уровня](workbook-error-handling.md#optional-second-level-error-code-examples).

> [!NOTE]
> Объект **innerError** может рекурсивно содержать более глубокие объекты **innerError** с дополнительными более конкретными кодами ошибок. Эти более **глубокие коды innerError** предназначены только для диагностики.

<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->

## <a name="see-also"></a>См. также

- [Использование REST API для Excel](/graph/api/resources/excel)