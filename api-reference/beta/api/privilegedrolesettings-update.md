---
title: Обновление Привилежедролесеттингс
description: Обновление параметров роли для данного параметра роли. Будет возвращен объект Привилежедролесеттингс.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: eb74999e48c3b2d524bf35d2d51390a526043a35
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455265"
---
# <a name="update-privilegedrolesettings"></a>Обновление Привилежедролесеттингс

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление параметров роли для данного параметра роли. Будет возвращен объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) .
## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Для обновления параметров роли запрашивающая сторона должна иметь роль администратора привилегированной роли. 

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [привилежедролесеттингс](../resources/privilegedrolesettings.md) в формате JSON.

В следующей таблице перечислены свойства, которые можно предоставить при обновлении параметров роли.

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|елеватиондуратион|duration|Продолжительность активации роли. Обязательный.|
|id|строка|Уникальный идентификатор для параметров роли. Только для чтения. Обязательный атрибут.|
|исмфаонелеватионконфигурабле|boolean|**значение true** , если мфаонелеватион является настраиваемым. **false** , если мфаонелеватион не является настраиваемым. Обязательное.|
|ластглобаладмин|Логический|Только для внутреннего использования.|
|макселаватиондуратион|duration|Максимальная длительность активированной роли. Обязательное.|
|мфаонелеватион|Логический|**значение true** , если для активации роли требуется mfa. **false** , если MFA не требуется для активации роли. Обязательное.|
|минелеватиондуратион|duration|Минимальная длительность активированной роли. Обязательное.|
|нотификатионтаусеронелеватион|Логический|**имеет значение true** , если вы отправляете уведомление конечному пользователю при активации роли. **значение false** , если уведомление не отправляется при активации роли. Обязательное.|
|тиккетингинфунелеватион|Логический|**имеет значение true** , если при активации роли требуются сведения о билетах. **false** , если при активации роли не требуются сведения о билетах. Обязательное.|
|аппровалонелеватион|Логический|**имеет значение true** , если при активации роли необходимо выполнить утверждение. **false** , если при активации роли не нужно утверждать. Обязательное.|
|аппроверидс|Коллекция строк|Список идентификаторов утверждения, если для активации необходимо утверждение.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Обратите внимание, что клиент должен быть зарегистрирован в PIM. В противном случае будет возвращен код состояния HTTP 403 запрещено.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
