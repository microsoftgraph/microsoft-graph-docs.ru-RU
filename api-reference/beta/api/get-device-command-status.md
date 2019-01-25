---
title: Получение состояния команды устройства
description: Получение состояния команды на устройстве. Полный список кодов состояния списка actionStatus см.
localization_priority: Normal
ms.openlocfilehash: ae5fe1f2b6b48c0a739911bd20370562e8540f18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510115"
---
# <a name="get-device-command-status"></a>Получение состояния команды устройства

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение состояния команды на устройстве. Полный список кодов состояния [списка actionStatus](#list-of-actionstatus)см.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.    |
|Делегированные (личная учетная запись Майкрософт) | Device.Command    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок |Значение
|:----|:------|
|Авторизация| Bearer {токен}. Обязательный. |
|Accept | application/json |

## <a name="response"></a>Ответ
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
  {
    "id": "0",
    "status": "requesting",
    "type": "null",
    "appServiceName": "null",
    "packageFamilyName": "null",
    "error": "null",
    "responsepayload": "null",
    "payload": "null",
    "permissionTicket": "null",
    "postBackUri": "null"
  }
```

## <a name="list-of-actionstatus"></a>Список actionStatus

- разрешения на запрос, / / команда будет создан и ожидает обработки
- sentToTarget, / / отправить команду целевого устройства
- выполнение, / / устройство подтверждено поступления команды и он выполняется
- завершена, и аудио- и завершения выполнения команд
- failedToSend, / / службе не удалось передать команду устройство
- executionFailed, / / команда не выполнена.
- commandDropped, / / команда Удалить клиентом, если устройство находится в состоянии ConnectedStandby
- отменить, / / отмена команды
- Отмена, / / отмены команды
- отменено, / / команда была отменена
- повторить попытку, / / службы восстанавливается для отправки команд к целевому
- истек срок действия, / / команды обработки превышено время истечения срока действия
- Ошибка, / аудио- и внутренняя ошибка при обработке команды
- настраиваемые / аудио- и настраиваемые состояния

## <a name="example"></a>Пример

В этом примере необходимо будет идентификатор устройства и идентификатор команды, которая выполнялась для устройства. При выдаче GET возвращается идентификатор устройства звонок, чтобы `/me/devices`, и команды, при выполнении отправки возвращается идентификатор звонок на `/me/devices/{id}/command`.

#### <a name="request"></a>Запрос

Ниже показан пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>Ответ

Ниже приводится пример отклика.
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "value":
  {
    "id": "0158355AD4D680CC4E2994CC009EFFD7337D1335FCA6ED266…",
    "status": "completed",
    "type": null,
    "appServiceName": null,
    "packageFamilyName": null,
    "error": null,
    "permissionTicket": null,
    "postBackUri": null,
    "payload": null
  }
}
```


## <a name="get-command-payload"></a>Получение полезных данных команды

Получение ответа полезных для определенных действий на устройстве. Полезные данные ответа используется при запросе приложения-службы для выполнения данных обратно.


### <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.    |
|Делегированные (личная учетная запись Майкрософт) | Device.Command    |
|Для приложений | Не поддерживается. |

### <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a>Заголовки запросов

| Заголовок |Значение
|:----|:------|
|Авторизация| Bearer {токен}. Обязательный. |
|Accept | application/json |

### <a name="response"></a>Ответ
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"date-time",
  "Type":"Ok"
}
```

### <a name="example"></a>Пример

В этом примере необходимо будет идентификатор устройства и идентификатор команды, которая выполнялась для устройства. Устройство, возвращается идентификатор при выдаче получить вызов на `/me/devices`, и команды, при выполнении отправки возвращается идентификатор звонок на `/me/devices/{id}/command`.

#### <a name="request"></a>Запрос

Ниже показан пример запроса.

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>Ответ

Ниже приводится пример отклика.

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"04/27/2017",
  "Type":"Ok"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/get-device-command-status.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
