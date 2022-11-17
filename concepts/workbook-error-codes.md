---
title: Коды ошибок для API книг и диаграмм
description: Перечисляет и описывает коды ошибок, возвращаемые API книг и диаграмм в Microsoft Graph при сбое запроса, отправленного через API.
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 88921271f38f9ae8ad440ea40a2733b890e14d83
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444182"
---
# <a name="error-codes-for-workbooks-and-charts-apis"></a>Коды ошибок для API книг и диаграмм

В этой статье описываются коды ошибок, возвращаемые API книг и диаграмм в Microsoft Graph при сбое запроса, отправленного через API. Дополнительные сведения об ошибках и типах ресурсов в Microsoft Graph см. в [разделе "Ошибки"](/concepts/errors.md). Дополнительные сведения об обработке ответов на ошибки из API Excel в Microsoft Graph см. в [разделе "Обработка ошибок"](workbook-error-handling.md).

## <a name="error-codes-and-messages"></a>Коды ошибок и сообщения

В следующей таблице перечислены текущие коды ошибок и сообщения. Служба может в любое время добавить новые коды ошибок.

| Код состояния | Код ошибки                | Сообщение об ошибке
|:------------|:--------------------------|:--------------
|400          | **badRequest**            | Запрос имеет неправильный формат или содержит ошибку.
|401          | **Несанкционированного**          | Вызывающая сторона не прошла проверку подлинности.
|403          | **Запрещено**             | У вызывающей стороны нет разрешения на выполнение действия.
|404          | **notFound**              | Не удалось найти ресурс.
|405          | **methodNotAllowed**      | Метод HTTP в запросе недопустим для ресурса.
|409          | **Конфликта**              | Текущее состояние противоречит ожидаемым результатам запроса.
|413          | **payloadTooLarge**       | Размер запроса превышает максимальное значение.
|429          | **tooManyRequests**       | Действия приложения или пользователя превысили ограничения.
|500          | **internalServerError**   | При обработке запроса произошла внутренняя ошибка сервера.
|501          | **notImplemented**        | Запрашиваемая функция не реализована.
|502          | **badGateway**            | Сервер обнаружил временную ошибку и не удалось выполнить запрос.
|503          | **serviceUnavailable**    | Служба недоступна. Повторите запрос.
|504          | **gatewayTimeout**        | Сервер, выступающий в качестве прокси-сервера, не получает от вышестоящего сервера во времени ответ для выполнения запроса.

## <a name="detailed-error-codes"></a>Подробные коды ошибок

Ниже приведены некоторые дополнительные коды ошибок, с которыми приложение может столкнуться на первом уровне вложенных `innerError` объектов. Служба может в любое время добавить новые коды ошибок.

- accessConflict
- accessDenied
- badRequestUncategorized
- conflictUncategorized
- filteredRangeConflict
- forbiddenUncategorized
- gatewayTimeoutUncategorized
- generalException
- insertDeleteConflict
- internalServerErrorUncategorized
- invalidArgument
- invalidReference
- invalidSessionAccessConflict
- invalidSessionAuthentication
- invalidSessionNotFound
- invalidSessionReCreatable
- invalidSessionRestricted
- invalidSessionUnexpected
- invalidSessionUnsupportedWorkbook
- itemAlreadyExists
- itemNotFound
- methodNotAllowed
- methodNotAllowedUncategorized
- nonBlankCellOffSheet
- notFoundUncategorized
- notImplementedUncategorized
- payloadTooLargeUncategorized
- rangeExceedsLimit
- requestAborted
- serviceUnavailableUncategorized
- tooManyRequestsUncategorized
- transientFailure
- unauthorizedUncategorized
- unsupportedOperation
- unsupportedWorkbook

> [!NOTE]
> Объект **innerError** может рекурсивно содержать более глубокие объекты **innerError** с дополнительными более конкретными кодами ошибок. Эти более **глубокие коды innerError** предназначены для чтения разработчиком.

<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->

## <a name="see-also"></a>См. также

- [Использование REST API для Excel](/graph/api/resources/excel)