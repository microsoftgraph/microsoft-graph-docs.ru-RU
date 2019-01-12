---
title: Список пользователей устройств
description: Ознакомьтесь со списком пользователей устройств, которые поддерживают возможности рим проекта. Этот компонент включает возможность запуска приложения, или сообщение или отправки данных в приложение. После того как вы выполнять на мне вызов GET- и устройств, передайте идентификатор устройства для отправки команды на устройство.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 04b67b770eec38d9e70a2263cd54212077335c85
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983543"
---
# <a name="list-user-devices"></a>Список пользователей устройств

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ознакомьтесь со списком пользователей устройств, которые поддерживают возможности рим проекта. Этот компонент включает возможность запуска приложения, или сообщение или отправки данных в приложение. После того как вы выполнять на мне вызов GET- и устройств, передайте идентификатор устройства для [отправки команды](send-device-command.md) на устройство.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.    |
|Делегированные (личная учетная запись Майкрософт) | Device.Read    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок |Значение
|:----|:------|
|Авторизация| Bearer {токен}. Обязательный. |
|Accept | application/json |

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код ответа 200 и свойств пользователя устройства в теле ответа.

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```

<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices",
  "value": [
    {
      "name": "name",
      "id": "id",
      "status": "status",
      "platform": "platform",
      "kind": "formFactor",
      "model": "model",
      "manufacturer": "manufacturer",
    }
  ]
}
```

## <a name="example"></a>Пример
В этом примере возвращается список устройств для пользователя. Для передачи команд устройство, с помощью `me/devices/{id}/command`, вам потребуется получить идентификатор устройства, который возвращается.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа. Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 140

{
  "value": [
    {
      "Name": "JimSurface",
      "id": "6841b3db-2b55-467b-ad84-79a41a4ef665",
      "Manufacturer": "Microsoft Corporation",
      "Model": "Surface Book",
      "Kind": "Tablet",
      "Status": "Unknown",
      "Platform": "Windows"
    }
  ]
}
```
