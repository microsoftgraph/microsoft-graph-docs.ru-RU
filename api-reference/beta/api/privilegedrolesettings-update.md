---
title: Обновление privilegedRoleSettings
description: Обновление параметров ролей для параметров указанного ролей. Объект privilegedRoleSettings будут возвращены.
localization_priority: Normal
ms.openlocfilehash: 09464c878c76ed557f30d0eac21e0572fae05062
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527656"
---
# <a name="update-privilegedrolesettings"></a>Обновление privilegedRoleSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление параметров ролей для параметров указанного ролей. Объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) будут возвращены.
## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Источник запроса, должны использовать одну из следующих ролей: привилегированной роль администратора, глобального администратора, администратора безопасности или безопасности чтения. 

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All    |
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
В тексте запроса укажите представление JSON объекта [privilegedRoleSettings](../resources/privilegedrolesettings.md) .

В следующей таблице приведены свойства, которые можно указать при обновлении параметров ролей.

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|ElevationDuration|duration|Длительность, при активации роли. Обязательный.|
|id|string|Уникальный идентификатор для параметров роли. Только для чтения. Обязательный.|
|isMfaOnElevationConfigurable|boolean|**значение true,** Если mfaOnElevation может быть настроен. **значение false,** Если mfaOnElevation не настраивается. Обязательный.|
|lastGlobalAdmin|Логическое|Только для внутреннего использования.|
|maxElavationDuration|duration|Максимальная длительность для активации роли. Обязательный.|
|mfaOnElevation|Логическое|**значение true,** Если необходимо активировать роль многофакторной проверкой Подлинности. **значение false,** Если многофакторной проверкой Подлинности не требуется для включения роли. Обязательный.|
|minElevationDuration|duration|Минимальная продолжительность активированные роли. Обязательный.|
|notificationToUserOnElevation|Логическое|**значение true,** Если отправить уведомление конечному пользователю при активации роли. **значение false,** Если не отправлять уведомления при активации роли. Обязательный.|
|ticketingInfoOnElevation|Логическое|**значение true,** Если отдела сведения требуется при активации роли. **значение false,** Если отдела сведения не является обязательным, когда активировать роль. Обязательный.|
|approvalOnElevation|Логическое|**значение true,** Если требуется утверждение при активации роли. **значение false,** Если утверждение не является обязательным, когда активировать роль. Обязательный.|
|approverIds|array|Список идентификаторов утверждения, если требуется для активации утверждение.|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Обратите внимание, что необходимо зарегистрировать для PIM клиента. В противном случае будут возвращены код состояния HTTP 403 запрещено.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
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
##### <a name="response"></a>Ответ
Ниже приведен пример отклика.

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
    "Error: /api-reference/beta/api/privilegedrolesettings-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
