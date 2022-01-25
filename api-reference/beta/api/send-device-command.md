---
title: Отправка команды устройства (неподготовленная)
description: 'Этот API позволяет Project Риму командовать устройством, связанным с учетной записью Майкрософт. После вызова GET передай в ID устройства команду на `me/devices` устройство. Поддерживаются два типа команд: LaunchURI и AppServices. Если вы используете LaunchURI, укажите *параметры типа* и *полезной нагрузки.* Для вызова AppService укажите '
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: ''
author: ailae
ms.openlocfilehash: 76b6edf47492d5a04e554e3f70834b3aed24d6a2
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201610"
---
# <a name="send-device-command-deprecated"></a>Отправка команды устройства (неподготовленная)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!CAUTION]
> Этот API обесценилось и перестал возвращать данные 30 сентября 2020 г.

Этот API позволяет Project Риму командовать устройством, связанным с учетной записью Майкрософт. После вызова GET передай в ID устройства команду на `me/devices` устройство. Поддерживаются два типа команд: LaunchURI и AppServices. Если вы используете LaunchURI, укажите *параметры типа* и *полезной нагрузки.* Для вызова AppService укажите *тип,* полезной *нагрузки,* *packageFamilyName* и *параметры appServiceName.*

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

## <a name="request-body"></a>Тело запроса

В теле запроса поставляем представление JSON свойств команд.

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
### <a name="command-properties"></a>Свойства команд

|**Имя**|**Тип**|**Описание**|
|:----|:------|:------|
|payload | microsoft.graph.json| Полезной нагрузки для отправки в службу приложений или запуска URI на устройстве. |
|responsePayload | microsoft.graph.json| Полезной нагрузки, возвращаемой с целевого устройства. |
|postBackURI | String | Отправьте URI для отправки последующих уведомлений об обновлениях. |
|packageFamilyName | String | Windows имя семейства пакета приложения. |
|appServiceName | String | Имя службы приложения, определенной целевым приложением. Требуется при запуске службы приложений. |
|type| String | LaunchURI или AppService. |
|id| String | ID команды, отправленной на устройство. |
|actionStatus | String | Состояние [](get-device-command-status.md) команды. |
|error| String| Любые ошибки, связанные с запросом из целевого приложения. |

## <a name="examples"></a>Примеры

### <a name="example-1-launch-uri"></a>Пример 1. Запуск URI

Ниже приводится пример запроса LaunchURI; он запустит URI или приложение на целевом устройстве. Чтобы запустить URI или приложение, выпустим POST с помощью ID устройства (полученного при вызове `me/devices` GET). Установите *параметры Type* *для LaunchURI* и предоведите значение URI, например https://bing.com .

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

В следующем примере показано, как запрашивать службу приложений на устройстве. Чтобы использовать службу приложений, необходимо сделать вызов POST с помощью ID устройства (полученный при вызове `me/devices` GET). Чтобы использовать следующий пример, необходимо установить приложение [Rome на](https://aka.ms/romanapp) целевом устройстве.

В вызове необходимо установить несколько дополнительных свойств.  Введите значение *AppService,* *AppServiceName* должно быть задавлено имя службы приложений, определенной в приложении, *PackageFamilyName* должно быть задавлено семейство пакетов, определенное в манифесте приложения, и *Payload* содержит ключи и значения службы, вызываемой в целевом приложении.

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


