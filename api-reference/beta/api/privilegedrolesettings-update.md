---
title: Обновление privilegedRoleSettings
description: Обновите параметры роли для заданного параметра роли. Будет возвращен объект privilegedRoleSettings.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 210d70c4ddb7b55003f2e78d9bfcc4e3f64491f6
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399392"
---
# <a name="update-privilegedrolesettings"></a>Обновление privilegedRoleSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите параметры роли для заданного параметра роли. Будет [возвращен объект privilegedRoleSettings](../resources/privilegedrolesettings.md) .
## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Запрашиватель должен иметь роль администратора привилегированных ролей для обновления параметров роли. 

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD    |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
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
В тексте запроса добавьте представление объекта [privilegedRoleSettings](../resources/privilegedrolesettings.md) в формате JSON.

В следующей таблице перечислены свойства, которые можно указать при обновлении параметра роли.

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|elevationDuration|duration|Длительность активации роли. Обязательный.|
|id|string|Уникальный идентификатор параметров роли. Только для чтения. Обязательный.|
|isMfaOnElevationConfigurable|логический|**Значение true** , если mfaOnElevation настраивается. **Значение false** , если mfaOnElevation не настраивается. Обязательно.|
|lastGlobalAdmin|Логический|Только для внутреннего использования.|
|maxElavationDuration|duration|Максимальная длительность активированной роли. Обязательно.|
|mfaOnElevation|Логический|**Значение true** , если для активации роли требуется многофакторная проверка подлинности. **false** if MFA is not required to activate the role. Обязательно.|
|minElevationDuration|duration|Минимальная длительность активированной роли. Обязательно.|
|notificationToUserOnElevation|Логическое|**Значение true** , если при активации роли пользователю отправляется уведомление. **false** if do not send notification when the role is activated. Обязательно.|
|ticketingInfoOnElevation|Логическое|**Значение true** , если сведения о запросе требуются при активации роли. **false** if the ticketing information is not required when activate the role. Обязательно.|
|approvalOnElevation|Логическое|**true** if the approval is required when activate the role. **false** if the approval is not required when activate the role. Обязательно.|
|approverIds|string collection|Список идентификаторов утверждения, если для активации требуется утверждение.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`.

Обратите внимание, что клиент должен быть зарегистрирован в PIM. В противном случае возвращается код состояния HTTP 403 Forbidden.
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


