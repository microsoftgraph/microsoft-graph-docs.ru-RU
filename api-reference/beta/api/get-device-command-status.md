---
title: Получение состояния команд для устройства
description: Получение состояния команды на устройстве. Полный список кодов состояния представлен в разделе List of Актионстатус.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 74104859b0621e51c0af9eced15912632fe5b9fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954307"
---
# <a name="get-device-command-status"></a>Получение состояния команд для устройства

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение состояния команды на устройстве. Полный список кодов состояния представлен в разделе [List of актионстатус](#list-of-actionstatus).

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

## <a name="response"></a>Отклик
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

## <a name="list-of-actionstatus"></a>Список Актионстатус

- была создана команда запроса//, ожидающая обработки
- Сенттотаржет,///команда отправлена на целевое устройство
- выполнение,//целевое устройство подтвердилое получение команды и выполняет ее.
- завершено,//выполнение команды завершено
- Фаиледтосенд,//служба не смогла отправить команду целевому устройству
- Сбой при выполнении команды Ексекутионфаилед или//.
- Команда Комманддроппед и//отброшена клиентом, если устройство находится в состоянии Коннектедстандби
- Отмена,//отмена команды
- Отмена и Отмена команды
- отменено,//команда отменена
- Retry,//служба повторяет попытку отправить целевую команду
- просрочено,//превышена Дата истечения срока действия обработки команд
- ошибка,//внутренняя ошибка при обработке команды
- настраиваемый//настраиваемый статус

## <a name="example"></a>Пример

В этом примере вам потребуется идентификатор устройства и идентификатор команды, выданной устройству. ИДЕНТИФИКАТОР устройства возвращается при выдаче вызова GET `/me/devices`, а идентификатор команды возвращается при выполнении вызова POST. `/me/devices/{id}/command`

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

#### <a name="response"></a>Отклик

Ниже приводится пример отклика.
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
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

Получение полезных данных ответа для определенного действия на устройстве. Полезные данные ответа используются при запросе службы приложений для обратного переноса данных.


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

### <a name="response"></a>Отклик
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

В этом примере вам потребуется идентификатор устройства и идентификатор команды, выданной устройству. ИДЕНТИФИКАТОР устройства возвращается при выдаче вызова GET `/me/devices`, а идентификатор команды возвращается при выполнении вызова POST. `/me/devices/{id}/command`

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

#### <a name="response"></a>Отклик

Ниже приводится пример отклика.

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
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
