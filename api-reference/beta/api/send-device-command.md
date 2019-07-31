---
title: Отправка команд для устройства
description: 'Этот API позволяет функциям Project Рим выполнять командное устройство, связанное с учетной записью Майкрософт. После выполнения вызова GET `me/devices`, передайте идентификатор устройства, чтобы выдать команду на устройство. Поддерживаются два типа команд: Лаунчури и Аппсервицес. Если вы используете Лаунчури, укажите *тип* и параметры *полезных данных* . Для вызова включающее укажите '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: fd45047d673dc6def51d3f417861cf15a38a2f98
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991515"
---
# <a name="send-device-command"></a>Отправка команд для устройства

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Этот API позволяет функциям Project Рим выполнять командное устройство, связанное с учетной записью Майкрософт. После выполнения вызова GET `me/devices`, передайте идентификатор устройства, чтобы выдать команду на устройство. Поддерживаются два типа команд: Лаунчури и Аппсервицес. Если вы используете Лаунчури, укажите *тип* и параметры *полезных данных* . Для вызова включающее укажите параметры *Type*, *полезная нагрузка*, *паккажефамилинаме*и *аппсервиценаме* .

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

В тексте запроса добавьте представление свойств команды в формате JSON.

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a>Отклик

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

|**Имя**|**Тип**|**Описание**|
|:----|:------|:------|
|payload | Microsoft. Graph. JSON| Полезные данные для отправки в службу приложения или для запуска URI на устройстве. |
|Респонсепайлоад | Microsoft. Graph. JSON| Полезные данные, возвращенные с целевого устройства. |
|Постбаккури | String | Обратный адрес URI для отправки последующих уведомлений об обновлениях. |
|Паккажефамилинаме | String | Имя семейства пакетов Windows Application. |
|Аппсервиценаме | String | Имя службы приложений, определенной конечным приложением. Является обязательным при запуске службы приложений. |
|type| String | Лаунчури или включающее. |
|id| Строка | Идентификатор команды, отправленной на устройство. |
|Актионстатус | String | [Состояние](get-device-command-status.md) команды. |
|error| String| Все ошибки, связанные с запросом от конечного приложения. |

## <a name="launch-uri-example"></a>Пример кода URI запуска

Ниже приведен пример запроса Лаунчури. он запустит URI или приложение на целевом устройстве. Чтобы запустить URI или приложение, отправьте сообщение POST с использованием идентификатора устройства (получено при вызове GET `me/devices`). Задайте для параметров *Type* значение *лаунчури* и введите значение URI, например https://bing.com.

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

#### <a name="response"></a>Отклик 

Ниже приведен пример ответа.

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
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


## <a name="app-service-example"></a>Пример службы приложений

Ниже приведен пример запроса службы приложения на устройстве. Чтобы использовать службу приложений, необходимо выполнить запрос POST, используя идентификатор устройства (полученный при выполнении вызова GET `me/devices`). Чтобы использовать приведенный ниже пример, необходимо установить [приложение Рим](https://aka.ms/romanapp) на целевом устройстве.

В вызове необходимо задать несколько дополнительных свойств. Для *типа* должно быть задано значение *включающее*, для *аппсервиценаме* должно быть задано имя службы приложений, определенной в приложении, *паккажефамилинаме* должно быть задано имя семейства пакетов, заданное в манифесте приложения, а *полезные данные* . содержит ключи и значения для службы, вызываемой в целевом приложении.

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
  "@odata.type": "microsoft.graph.command",
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
