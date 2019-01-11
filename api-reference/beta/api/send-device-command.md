---
title: Отправка команды устройства
description: 'Этот интерфейс API обеспечивает возможности рим проекта для передачи команд устройство, связанное с учетной записью Майкрософт. После выполнения на вызов GET `me/devices`, передайте идентификатор устройства, чтобы выполнить команду на устройство. Поддерживаются два типа из команд: LaunchURI и AppServices. Если вы используете LaunchURI, указания параметров *типа* и *полезных данных* . Для вызова AppService, укажите '
localization_priority: Normal
ms.openlocfilehash: 54349e2f43a776523614b0cd2abbc209e89305fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891989"
---
# <a name="send-device-command"></a>Отправка команды устройства

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Этот интерфейс API обеспечивает возможности рим проекта для передачи команд устройство, связанное с учетной записью Майкрософт. После выполнения на вызов GET `me/devices`, передайте идентификатор устройства, чтобы выполнить команду на устройство. Поддерживаются два типа из команд: LaunchURI и AppServices. Если вы используете LaunchURI, указания параметров *типа* и *полезных данных* . Для вызова AppService укажите *Тип*, *полезных данных*, *packageFamilyName*и *appServiceName* параметры.

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
POST me/devices/{id}/commands
```

## <a name="request-headers"></a>Заголовки запросов


| Заголовок |Значение
|:----|:------|
|Авторизация| Bearer {токен}. Обязательный. |
|Accept | application/json |

## <a name="request-body"></a>Тело запроса

В тексте запроса укажите представление JSON свойства команды.

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a>Ответ

```http
HTTP/1.1 201 OK
```

```json
{
  "id": "0",
  "status": "requesting",
  "type": "appService",
  "appServiceName": "appServiceName",
  "packageFamilyName": "packageFamilyName",
  "error": "null",
  "responsePayload": "null",
  "payload": "payload-JSON",
  "permissionTicket": "null",
  "postBackUri": "postbackURI"
}
```
## <a name="command-properties"></a>Свойства команды 

|**Name**|**Тип**|**Описание**|
|:----|:------|:------|
|payload | Microsoft.Graph.JSON| Полезные данные для отправки приложения-службы или для запуска URI на устройстве. |
|responsePayload | Microsoft.Graph.JSON| Полезные данные, возвращаемые целевого устройства. |
|postBackURI | Строка | Публикация резервного URI для отправки последующих уведомлений об обновлениях. |
|packageFamilyName | Строка | Имя семейства Windows пакет приложения. |
|appServiceName | Строка | Имя приложения-службы, определенные в конечное приложение. Требуется при запуске приложения-службы. |
|type| Строка | LaunchURI или AppService. |
|id| Строка | Идентификатор команды, полученного на устройство. |
|actionStatus | Строка | [Состояние](get-device-command-status.md) команды. |
|error| Строка| Все ошибки, связанные с запросом от целевого приложения. |

## <a name="launch-uri-example"></a>Запуск примера URI

Ниже приведен пример запроса LaunchURI; он запустится URI или на устройстве конечного приложения. Для запуска приложения или URI, заключать POST, используя идентификатор устройства (полученных при выполнении вызова GET для `me/devices`). Параметры *типа* для *LaunchURI* , поэтому указывать значение URI, таких как https://bing.com.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "post_command"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{ "type" : "LaunchUri", "payload" : {"uri":"https://bing.com"}}

```

#### <a name="response"></a>Ответ 

Ниже приведен пример ответа.

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7337D1B...",
  "status": "requesting",
  "type": null,
  "appServiceName": null,
  "packageFamilyName": null,
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "uri": "https://bing.com"
  }
}

```


## <a name="app-service-example"></a>Пример приложения-службы

Ниже приведен пример запросов службу приложения на устройстве. Использование приложения-службы необходимо выполнить вызов POST, с помощью идентификатор устройства (полученных при выполнении вызова GET для `me/devices`). Для использования в следующем примере, необходимо установить [приложение рим](https://aka.ms/romanapp) целевое устройство.

Несколько дополнительных свойств необходимо установить в вызове. *Тип* должен иметь значение *AppService*, *AppServiceName* должно быть присвоено имя службы приложения, определенные в приложении, *PackageFamilyName* должно быть присвоено имя пакета семейства, определенные в манифесте приложения и *полезных данных* содержит ключи и значения для службы вызова в конечном приложении.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "post_command_2"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{
  "type" : "AppService",
  "appServiceName" : "com.microsoft.test.cdppingpongservice",
  "packageFamilyName" : "5085ShawnHenry.RomanTestApp_jsjw7knzsgcce",
  "payload" : {
    "Type":"Toast","Title":"Hello","Subtitle":"World!"}
  }
```

#### <a name="response"></a>Ответ

Ниже приведен пример ответа.

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7EADA8307E96FF1C8D19B..",
  "status": "requesting",
  "type": null,
  "appServiceName": "com.microsoft.randomnumbergenerator",
  "packageFamilyName": "Microsoft.SDKSamples.AppServicesProvider.CS_8wekyb3d8bbwe",
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "Type": "Toast",
    "Title": "Hello",
    "Subtitle": "World!"
  }
}
```
