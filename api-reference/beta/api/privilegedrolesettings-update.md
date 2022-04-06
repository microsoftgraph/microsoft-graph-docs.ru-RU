---
title: Обновление privilegedRoleSettings
description: Обновление параметров ролей для данного параметра ролей. Объект privilegedRoleSettings будет возвращен.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: japere
ms.openlocfilehash: d4a21eb18d8cfa6e6b3616840b66cd2e2ec01c2f
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509947"
---
# <a name="update-privilegedrolesettings"></a>Обновление privilegedRoleSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление параметров ролей для данного параметра ролей. Объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) будет возвращен.
## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Запрашиватель должен иметь роль администратора привилегированных ролей для обновления параметров ролей. 

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD    |
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
| Авторизация  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [privilegedRoleSettings](../resources/privilegedrolesettings.md) .

В следующей таблице перечислены свойства, которые можно предоставить при обновлении параметра роли.

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|elevationDuration|duration|Продолжительность активации роли. Обязательный.|
|id|string|Уникальный идентификатор параметров ролей. Только для чтения. Обязательный атрибут.|
|isMfaOnElevationConfigurable|boolean|**верно** , если mfaOnElevation настраивается. **false** , если mfaOnElevation не настраивается. Обязательный аргумент.|
|lastGlobalAdmin|Boolean|Только для внутреннего использования.|
|maxElavationDuration|duration|Максимальная продолжительность для активированной роли. Обязательный аргумент.|
|mfaOnElevation|Boolean|**значение true** , если для активации роли требуется MFA. **false** , если MFA не требуется для активации роли. Обязательный аргумент.|
|minElevationDuration|duration|Минимальная продолжительность для активированной роли. Обязательный аргумент.|
|notificationToUserOnElevation|Boolean|**значение true** , если отправить уведомление конечному пользователю при активации роли. **false** , если не отправлять уведомления при активации роли. Обязательный аргумент.|
|ticketingInfoOnElevation|Boolean|**значение true** , если при активации роли требуется информация о билетах. **false** , если сведения о билетах не требуются при активации роли. Обязательный аргумент.|
|approvalOnElevation|Boolean|**значение true** , если требуется утверждение при активации роли. **false** , если утверждение не требуется при активации роли. Обязательный аргумент.|
|approverIds|string collection|Список ID утверждения, если требуется утверждение для активации.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`.

Обратите внимание, что клиент должен быть зарегистрирован в PIM. В противном случае код запретного статуса HTTP 403 будет возвращен.
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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/put-privilegedrolesettings-go-snippets.md)]
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


