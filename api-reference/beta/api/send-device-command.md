---
title: Команда отправки устройства (не рекомендуется)
description: 'Этот API позволяет project Rome командой устройства, связанного с учетной записью Майкрософт. После вызова GET передайте `me/devices`идентификатор устройства, чтобы выполнить команду на устройстве. Поддерживаются два типа команд: LaunchURI и AppServices. Если вы используете LaunchURI, укажите *тип* и *параметры полезных* данных. Для вызова Службы приложений укажите '
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: project-rome
author: ailae
ms.openlocfilehash: db99f797b234b96d83487765218d49c78d434c5f
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944172"
---
# <a name="send-device-command-deprecated"></a>Команда отправки устройства (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!CAUTION]
> Этот API устарел и перестал возвращать данные 30 сентября 2020 г.

Этот API позволяет project Rome командой устройства, связанного с учетной записью Майкрософт. После вызова GET передайте `me/devices`идентификатор устройства, чтобы выполнить команду на устройстве. Поддерживаются два типа команд: LaunchURI и AppServices. Если вы используете LaunchURI, укажите *тип* и *параметры полезных* данных. Для вызова Службы приложений укажите *тип,* *полезные* данные, *packageFamilyName* и *параметры appServiceName* .

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
|Авторизация| Bearer {token}. Обязательный. |
|Accept | application/json |

## <a name="request-body"></a>Текст запроса

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
### <a name="command-properties"></a>Свойства команды

|**Имя**|**Тип**|**Описание**|
|:----|:------|:------|
|payload | microsoft.graph.json| Полезные данные для отправки в службу приложений или запуска URI на устройстве. |
|responsePayload | microsoft.graph.json| Полезные данные, возвращаемые с целевого устройства. |
|postBackURI | Строка | Отправьте URI для отправки последующих уведомлений об обновлениях. |
|packageFamilyName | Строка | Имя семейства пакетов Windows для приложения. |
|appServiceName | Строка | Имя службы приложений, определенной целевым приложением. Требуется при запуске службы приложений. |
|type| Строка | LaunchURI или AppService. |
|id| Строка | Идентификатор команды, отправленной на устройство. |
|actionStatus | Строка | [Состояние команды](get-device-command-status.md). |
|error| String| Все ошибки, связанные с запросом из целевого приложения. |

## <a name="examples"></a>Примеры

### <a name="example-1-launch-uri"></a>Пример 1. Запуск URI

Ниже приведен пример запроса LaunchURI. он запустит универсальный код ресурса (URI) или приложение на целевом устройстве. Чтобы запустить универсальный код ресурса (URI) или приложение, выдайте запрос POST, используя идентификатор устройства (полученный при вызове GET `me/devices`). *Задайте для параметров Type* значение *LaunchURI* и укажите значение URI, например https://bing.com.

#### <a name="request"></a>Запрос

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


### <a name="example-2-app-service"></a>Пример 2. Служба приложений

В следующем примере показано, как запросить службу приложений на устройстве. Чтобы использовать службу приложений, необходимо выполнить вызов POST с использованием идентификатора устройства (полученного при вызове GET `me/devices`). Чтобы использовать следующий пример, необходимо установить приложение [Rome](https://aka.ms/romanapp) на целевом устройстве.

В вызове необходимо задать несколько дополнительных свойств.  Тип должен иметь значение *AppService*, *AppServiceName* — имя службы приложений, определенной в приложении, *PackageFamilyName* — имя семейства пакетов, определенное в манифесте приложения, а *Payload* содержит ключи и значения службы, вызываемой в целевом приложении.

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

#### <a name="response"></a>Отклик

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


