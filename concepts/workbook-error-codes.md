---
title: Коды ошибок для книг и API диаграмм в Microsoft Graph
description: Списки и описания кодов ошибок и сообщений для книг и API диаграмм в Microsoft Graph.
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 981be39ad78af98d131e4b38a9de49e688e27551
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672408"
---
# <a name="error-codes-for-workbooks-and-charts-apis-in-microsoft-graph"></a>Коды ошибок для книг и API диаграмм в Microsoft Graph

В этой статье описываются коды ошибок, возвращаемые книгами и API диаграмм в Microsoft Graph при сбойе запроса, отправленного через API. Дополнительные сведения об ответах на ошибки и типах ресурсов в Microsoft Graph см. в [материале Errors](/concepts/errors.md). Сведения об обработке ответов на ошибки из Excel API в Microsoft Graph см. в материале [Обработка ошибок](workbook-error-handling.md).

## <a name="error-code"></a>Код ошибки

В следующей таблице перечислены текущие коды ошибок и сообщения. Служба может добавлять новые коды ошибок в любое время. 

| Код состояния               | Код ошибки                       | Сообщение об ошибке
|:--------------------------|:--------------------------|:--------------
|400    | **badRequest**          | Запрос имеет неправильный формат или содержит ошибку.
|401    | **несанкционированные**  | Вызывающая сторона не прошла проверку подлинности.
|403    | **запрещено**      | У вызывающей стороны нет разрешения на выполнение действия.
|404    | **notFound**          | Не удалось найти ресурс.
|405    | **methodNotAllowed**        | Метод HTTP в запросе недопустим для ресурса.
|409    | **конфликт**          | Текущее состояние противоречит ожидаемым результатам запроса.
|413    | **payloadTooLarge**       | Размер запроса превышает максимальное значение.
|429    | **tooManyRequests**     | Действия приложения или пользователя превысили ограничения.
|500    | **internalServerError**            | При обработке запроса произошла внутренняя ошибка сервера.
|501    | **notImplemented**          | Запрашиваемая функция не реализована.
|502    | **badGateway**          | Сервер столкнулся с временной ошибкой и не смог выполнить запрос.
|503    | **serviceUnavailable**      | Служба недоступна. Пожалуйста, попробуйте свой запрос еще раз.
|504    | **gatewayTimeout**        | Сервер, выступая в качестве прокси-сервера, не получил вовремя ответ от сервера, находящегося выше по течению, для выполнения запроса.

## <a name="detailed-error-code"></a>Подробный код ошибки
Ниже приводится ряд дополнительных кодов ошибок, с которыми ваше приложение может столкнуться на первом уровне вложенных объектов `innerError` . Служба может добавлять новые коды ошибок в любое время.

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

>**Примечание:** Объект **innerError может** повторно содержать более глубокие **объекты innerError** с дополнительными, более конкретными кодами ошибок. Эти более глубокие **коды innerError** являются для разработчика для чтения.
<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->
