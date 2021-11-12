---
title: Перечисление пользовательских устройств
description: Получите список пользовательских устройств, поддерживаю Project возможностей Рима. Это включает возможность запуска приложения, сообщения или отправки данных в приложение. После вызова GET для меня или устройств передайте в ID устройства команду на устройство.
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: dd47f2f9cd3edfb1b45db833857e0a3f2cc0820b
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60940905"
---
# <a name="list-user-devices"></a>Перечисление пользовательских устройств

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список пользовательских устройств, поддерживаю Project возможностей Рима. Это включает возможность запуска приложения, сообщения или отправки данных в приложение. После вызова GET для меня или устройств передайте в ID устройства команду [на](send-device-command.md) устройство.

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

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа в 200 и свойства устройства пользователя в тексте ответа.

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
В этом примере будет возвращен список устройств для пользователя. Чтобы командовать устройством с помощью, необходимо получить `me/devices/{id}/command` ID возвращенного устройства.

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

Ниже представлен пример ответа. Примечание: показанный здесь объект ответа может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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


