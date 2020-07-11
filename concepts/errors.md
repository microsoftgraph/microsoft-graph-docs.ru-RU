---
title: Сообщения об ошибках и типы ресурсов Microsoft Graph
description: "  "
localization_priority: Priority
ms.openlocfilehash: cc3a0a0acacd7477c1cf686089c0235850059443
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091426"
---
# <a name="microsoft-graph-error-responses-and-resource-types"></a>Сообщения об ошибках и типы ресурсов Microsoft Graph

<!--In this article:
  
-   [Status code](#msg-status-code)
-   [Error resource type](#msg-error-resource-type)
-   [Code property](#msg-code-property)

<a name="msg_error_response"> </a> -->

Сообщения об ошибках в Microsoft Graph возвращаются с использованием стандартных кодов состояния HTTP, а также JSON-объекта сообщения об ошибке.

## <a name="http-status-codes"></a>Коды состояния HTTP

В приведенной ниже таблице представлен список возможных кодов состояния HTTP и их описаний.

| Код состояния | Сообщение о состоянии                  | Описание                                                                                                                            |
|:------------|:--------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------|
| 400         | Неправильный запрос (Bad Request)                     | Не удается обработать запрос, так как он имеет неправильный формат или содержит ошибку.                                                                       |
| 401         | Не авторизован (Unauthorized)                    | Требуемые сведения о проверке подлинности отсутствуют или недопустимы для ресурса.                                                   |
| 403         | Запрещено                       | Access is denied to the requested resource. The user might not have enough permission. <br /><br /> **Важно!** Если к ресурсу применены политики условного доступа, то, возможно, будет возвращена ошибка HTTP 403; Forbidden error=insufficent_claims. Дополнительные сведения о Microsoft Graph и условном доступе см. в статье [Руководство для разработчиков по условному доступу в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)  |
| 404         | Не найдено (Not Found)                       | Запрашиваемый ресурс не существует.                                                                                                  |
| 405         | Недопустимый метод (Method Not Allowed)              | Метод HTTP в запросе недопустим для ресурса.                                                                         |
| 406         | Неприемлемо (Not Acceptable)                  | Эта служба не поддерживает формат, запрошенный в заголовке Accept.                                                                |
| 409         | Конфликт (Conflict)                        | The current state conflicts with what the request expects. For example, the specified parent folder might not exist.                   |
| 410         | Отсутствует (Gone)                            | Запрошенный ресурс недоступен на сервере.                                               |
| 411         | Требуется длина (Length Required)                 | В запросе нужно указать заголовок Content-Length.                                                                                    |
| 412         | Необходимое условие не выполнено (Precondition Failed)             | Необходимое условие, указанное в запросе (например, заголовок If-Match), не соответствует текущему состоянию ресурса.                       |
| 413         | Слишком большой объект запроса (Request Entity Too Large)        | Размер запроса превышает максимальное значение.                                                                                            |
| 415         | Неподдерживаемый тип носителя (Unsupported Media Type)          | Тип содержимого запроса имеет формат, который не поддерживает служба.                                                      |
| 416         | Запрошенный диапазон невыполним (Requested Range Not Satisfiable) | Указан недопустимый или недоступный диапазон байтов.                                                                                    |
| 422         | Необрабатываемый объект (Unprocessable Entity)            | Не удается обработать запрос из-за неправильной семантики.                                                                        |
| 423         | Заблокирован                          | Ресурс заблокирован.                                                                                          |
| 429         | Слишком много запросов (Too Many Requests)               | Количество запросов клиентского приложения отрегулировано, оно сможет повторить запрос по истечении некоторого времени.                |
| 500         | Внутренняя ошибка сервера (Internal Server Error)           | При обработке запроса возникла внутренняя ошибка сервера.                                                                       |
| 501         | Не реализовано (Not Implemented)                 | Запрашиваемая функция не реализована.                                                                                               |
| 503         | Служба недоступна (Service Unavailable)             | The service is temporarily unavailable for maintenance or is overloaded. You may repeat the request after a delay, the length of which may be specified in a Retry-After header.|
| 504         | Истекло время ожидания шлюза (Gateway Timeout)                 | The server, while acting as a proxy, did not receive a timely response from the upstream server it needed to access in attempting to complete the request. May occur together with 503. |
| 507         | Недостаточно места (Insufficient Storage)            | Достигнута максимальная квота хранилища.                                                                                            |
| 509         | Превышено ограничение пропускной способности (Bandwidth Limit Exceeded)        | Your app has been throttled for exceeding the maximum bandwidth cap. Your app can retry the request again after more time has elapsed. |

The error response is a single JSON object that contains a single property named **error**. This object includes all the details of the error. You can use the information returned here instead of or in addition to the HTTP status code. The following is an example of a full JSON error body.

<!-- { "blockType": "ignored", "@odata.type": "odata.error", "expectError": true, "name": "example-error-response" } -->
```json
{
  "error": {
    "code": "invalidRange",
    "message": "Uploaded fragment overlaps with existing data.",
    "innerError": {
      "requestId": "request-id",
      "date": "date-time"
    }
  }
}
```

<!--<a name="msg_error_resource_type"> </a> -->

## <a name="error-resource-type"></a>Тип ресурса ошибки

Ресурс ошибки возвращается, если при обработке запроса происходит ошибка.

Сообщения об ошибках соответствуют определению в спецификации [OData версии 4](https://docs.oasis-open.org/odata/odata-json-format/v4.0/os/odata-json-format-v4.0-os.html#_Toc372793091).

### <a name="json-representation"></a>Представление JSON

Ресурс ошибки состоит из указанных ниже ресурсов.

<!-- { "blockType": "resource", "@odata.type": "odata.error" } -->
```json
{
  "error": { "@odata.type": "odata.error" }  
}
```

#### <a name="odataerror-resource-type"></a>Тип ресурса odata.error

Сообщение об ошибке содержит ресурс ошибки, состоящий из следующих свойств:

<!-- { "blockType": "resource", "@odata.type": "odata.error", "optionalProperties": [ "target", "details", "innererror"] } -->
```json
{
  "code": "string",
  "message": "string",
  "innererror": { "@odata.type": "odata.error" }
}
```

| Имя свойства  | Значение                  | Описание                                                                                               |
|:---------------|:-----------------------|:-----------------------------------------------------------------------------------------------------------|
| **code**       | string                 | Строка с кодом возникшей ошибки                                                            |
| **message**    | string                 | A developer ready message about the error that occurred. This should not be displayed to the user directly. |
| **innererror** | error object           | Optional. Additional error objects that may be more specific than the top level error.                     |

<!--<a name="msg_code_property"> </a> -->

#### <a name="code-property"></a>Свойство code

The `code` property contains one of the following possible values. Your apps should be prepared to handle any one of these errors.

| Код                      | Описание
|:--------------------------|:--------------
| **accessDenied**          | У вызывающей стороны нет разрешения на выполнение действия. 
| **activityLimitReached**  | Действия приложения или пользователя превысили ограничения.
| **generalException**      | Произошла неуказанная ошибка.
| **invalidRange**          | Указан недопустимый или недоступный диапазон байтов.
| **invalidRequest**        | Запрос имеет неправильный формат или содержит ошибку.
| **itemNotFound**          | Не удалось найти ресурс.
| **malwareDetected**       | В запрошенном ресурсе обнаружена вредоносная программа.
| **nameAlreadyExists**     | Элемент с указанным именем уже существует.
| **notAllowed**            | Действие запрещено системой.
| **notSupported**          | Запрос не поддерживается в системе.
| **resourceModified**      | Обновляемый ресурс изменился с момента последнего чтения вызывающей стороной. Как правило, не совпадают теги eTag.
| **resyncRequired**        | Разностный токен больше не действителен, а приложение должно сбросить состояние синхронизации.
| **serviceNotAvailable**   | The service is not available. Try the request again after a delay. There may be a Retry-After header. 
| **syncStateNotFound**     | Создание состояния синхронизации не найдено. Срок действия разностного маркера истек, и данные требуется синхронизировать повторно. 
| **quotaLimitReached**     | Пользователь превысил квоту.
| **unauthenticated**       | Вызывающая сторона не прошла проверку подлинности.

The `innererror` object might recursively contain more `innererror` objects with additional, more specific error codes. When handling an error, apps should loop through all the error codes available and use the most detailed one that they understand. Some of the more detailed codes are listed at the bottom of this page.

To verify that an error object is an error you are expecting, you must loop over the `innererror` objects, looking for the error codes you expect. For example:

```csharp
public bool IsError(string expectedErrorCode)
{
    OneDriveInnerError errorCode = this.Error;
    while (null != errorCode)
    {
        if (errorCode.Code == expectedErrorCode)
            return true;
        errorCode = errorCode.InnerError;
    }
    return false;
}
```

В примере [Обработка кодов ошибок](https://gist.github.com/rgregg/a1866be15e685983b441) показано, как правильно обрабатывать ошибки.

The `message` property at the root contains an error message intended for the developer to read. Error messages are not localized and shouldn't be displayed directly to the user. When handling errors, your code should not key off of `message` values because they can change at any time, and they often contain dynamic information specific to the failed request. You should only code against error codes returned in `code` properties.

#### <a name="detailed-error-codes"></a>Подробные коды ошибок
The following are some additional errors that your app might encounter within the nested `innererror` objects. Apps are not required to handle these, but can if they choose. The service might add new error codes or stop returning old ones at any time, so it is important that all apps be able to handle the [basic error codes](#code-property).

| Код                               | Описание
|:-----------------------------------|:----------------------------------------------------------
| **accessRestricted**               | Доступ разрешен только владельцу элемента.
| **cannotSnapshotTree**             | Failed to get a consistent delta snapshot. Try again later.
| **childItemCountExceeded**         | Достигнуто максимальное количество дочерних элементов.
| **entityTagDoesNotMatch**          | Тег ETag не соответствует текущему значению элемента.
| **fragmentLengthMismatch**         | Объявленный общий размер этого фрагмента отличается от размера сеанса отправки.
| **fragmentOutOfOrder**             | Фрагмент передан не по порядку.
| **fragmentOverlap**                | Переданный фрагмент перекрывает существующие данные.
| **invalidAcceptType**              | Недопустимый тип входных данных.
| **invalidParameterFormat**         | Недопустимый формат параметра.
| **invalidPath**                    | Имя содержит недопустимые символы.
| **invalidQueryOption**             | Недопустимый параметр запроса.
| **invalidStartIndex**              | Недопустимый начальный индекс.
| **lockMismatch**                   | Маркер блокировки не соответствует существующей блокировке.
| **lockNotFoundOrAlreadyExpired**   | В данный момент для элемента не задана действительная блокировка.
| **lockOwnerMismatch**              | Идентификатор владельца блокировки не соответствует указанному идентификатору.
| **malformedEntityTag**             | ETag header is malformed. ETags must be quoted strings.
| **maxDocumentCountExceeded**       | Достигнуто максимальное количество документов.
| **maxFileSizeExceeded**            | Превышен максимальный размер файла.
| **maxFolderCountExceeded**         | Достигнуто максимальное количество папок.
| **maxFragmentLengthExceeded**      | Превышен максимальный размер файла.
| **maxItemCountExceeded**           | Достигнуто максимальное количество элементов.
| **maxQueryLengthExceeded**         | Превышена максимальная длина запроса.
| **maxStreamSizeExceeded**          | Превышен максимальный размер потока.
| **parameterIsTooLong**             | Превышена максимальная длина параметра.
| **parameterIsTooSmall**            | Размер параметра меньше минимального значения.
| **pathIsTooLong**                  | Превышена максимальная длина пути.
| **pathTooDeep**                    | Достигнуто максимальное число уровней в иерархии папок.
| **propertyNotUpdateable**          | Свойство не поддерживает обновление.
| **resyncApplyDifferences**         | Resync required. Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.
| **resyncRequired**                 | Требуется повторная синхронизация.
| **resyncUploadDifferences**        | Resync required. Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).
| **serviceNotAvailable**            | Сервер не может обработать текущий запрос.
| **serviceReadOnly**                | Ресурс временно доступен только для чтения.
| **throttledRequest**               | Слишком много запросов.
| **tooManyResultsRequested**        | Запрошено слишком много результатов.
| **tooManyTermsInQuery**            | Запрос содержит слишком много условий.
| **totalAffectedItemCountExceeded** | Операция запрещена, так как количество задействованных элементов превышает пороговое значение.
| **truncationNotAllowed**           | Усечение данных запрещено.
| **uploadSessionFailed**            | Ошибка сеанса отправки.
| **uploadSessionIncomplete**        | Сеанс отправки не завершен.
| **uploadSessionNotFound**          | Сеанс отправки не найден.
| **virusSuspicious**                | Этот документ подозрительный и может содержать вирус.
| **zeroOrFewerResultsRequested**    | Запрошено ноль или меньше результатов.


<!-- {
  "type": "#page.annotation",
  "description": "Understand the error format for the API and error codes.",
  "keywords": "error response, error, error codes, innererror, message, code",
  "section": "documentation",
  "suppressions": [
    " Warning: /concepts/errors.md:
      Multiple resources found in file, but we only support one per file. 'odata.error,odata.error'. Skipping."
  ],
  "tocPath": "Misc/Error Responses"
} -->
