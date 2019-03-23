---
title: Обновление Привилежедролесеттингс
description: Обновление параметров роли для данного параметра роли. Будет возвращен объект Привилежедролесеттингс.
localization_priority: Normal
ms.openlocfilehash: f416656362c5be0ccdaa2b3aaa7812511e357875
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789608"
---
# <a name="update-privilegedrolesettings"></a>Обновление Привилежедролесеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление параметров роли для данного параметра роли. Будет возвращен объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) .
## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный администратор ролей, глобальный администратор, администратор безопасности или средство чтения безопасности. 

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
В тексте запроса добавьте представление объекта [Привилежедролесеттингс](../resources/privilegedrolesettings.md) в формате JSON.

В следующей таблице перечислены свойства, которые можно предоставить при обновлении параметров роли.

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|Елеватиондуратион|duration|Продолжительность активации роли. Обязательный.|
|id|string|Уникальный идентификатор для параметров роли. Только для чтения. Обязательный аргумент.|
|Исмфаонелеватионконфигурабле|логический|**значение true** , если мфаонелеватион является настраиваемым. **false** , если мфаонелеватион не является настраиваемым. Обязательный аргумент.|
|Ластглобаладмин|Boolean|Только для внутреннего использования.|
|Макселаватиондуратион|duration|Максимальная длительность активированной роли. Обязательный аргумент.|
|Мфаонелеватион|Boolean|**значение true** , если для активации роли требуется mfa. **false** , если MFA не требуется для активации роли. Обязательный аргумент.|
|Минелеватиондуратион|duration|Минимальная длительность активированной роли. Обязательный аргумент.|
|Нотификатионтаусеронелеватион|Boolean|**имеет значение true** , если вы отправляете уведомление конечному пользователю при активации роли. **значение false** , если уведомление не отправляется при активации роли. Обязательный аргумент.|
|Тиккетингинфунелеватион|Boolean|**имеет значение true** , если при активации роли требуются сведения о билетах. **false** , если при активации роли не требуются сведения о билетах. Обязательный аргумент.|
|Аппровалонелеватион|Boolean|**имеет значение true** , если при активации роли необходимо выполнить утверждение. **false** , если при активации роли не нужно утверждать. Обязательный аргумент.|
|Аппроверидс|Коллекция строк|Список идентификаторов утверждения, если для активации необходимо утверждение.|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Обратите внимание, что клиент должен быть зарегистрирован в PIM. В противном случае будет возвращен код состояния HTTP 403 запрещено.
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
##### <a name="response"></a>Отклик
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
