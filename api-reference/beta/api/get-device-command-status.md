---
title: Получение состояния команды устройства
description: Получение состояния команды на устройстве. Полный список кодов состояния списка actionStatus см.
localization_priority: Normal
ms.openlocfilehash: 9dca743a50f248abee76fb4d54352df3d400ada1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883134"
---
# <a name="get-device-command-status"></a>Получение состояния команды устройства

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
