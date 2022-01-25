---
title: Получить состояние команды устройства (неподготовленное)
description: Получите состояние команды на устройстве. Полный список кодов состояния см. в списке actionStatus.
ms.localizationpriority: medium
doc_type: apiPageType
author: ailae
ms.prod: ''
ms.openlocfilehash: bbe26243c9779e7917e4014038b26473a7cd17f7
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201322"
---
# <a name="get-device-command-status-deprecated"></a>Получить состояние команды устройства (неподготовленное)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите состояние команды на устройстве. Полный список кодов состояния см. [в списке actionStatus.](#list-of-actionstatus)

> [!CAUTION]
> Этот API обесценилось и перестал возвращать данные 30 сентября 2020 г.

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
|Авторизация| Bearer {token}. Обязательный. |
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

## <a name="list-of-actionstatus"></a>Список действийStatus

- запрос, // Команда создана и ожидает обработки
- sentToTarget, // Команда отправлена на целевое устройство
- выполнение, // Целевое устройство признало получение команды и выполняет ее
- завершено,// Выполнено выполнение команды
- failedToSend, // Служба не отправила команду на целевое устройство
- executionFailed, // Выполнение команды не удалось
- commandDropped, // Команда отброшена клиентом, если устройство находится в состоянии ConnectedStandby
- отмена, // Отмена команды
- отмена, // Отмена команды
- отменено, // Команда отменена
- retry, // Служба повторно отправляет команду в целевой адрес
- истек, // Обработка команд превысила срок действия
- ошибка, // Внутренняя ошибка при обработке команды
- настраиваемый // Настраиваемый статус

## <a name="example"></a>Пример

В этом примере вам потребуется ID устройства и ID команды, которая была выдана устройству. ID устройства возвращается при выдаче вызова GET, а командный ID возвращается при вызове `/me/devices` `/me/devices/{id}/command` POST.

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


## <a name="get-command-payload"></a>Получить командную нагрузку

Получите полезное устройство для определенного действия на устройстве. Полезной нагрузки ответа используется при запросе службы приложения для переноса данных обратно.


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
GET me/devices/{id}/commands/{id}/responsePayload
```

### <a name="request-headers"></a>Заголовки запросов

| Заголовок |Значение
|:----|:------|
|Авторизация| Bearer {token}. Обязательный. |
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

В этом примере вам потребуется ID устройства и ID команды, которая была выдана устройству. При выдаче вызова GET возвращается ID устройства, а при вызове POST возвращается командный `/me/devices` `/me/devices/{id}/command` ID.

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


