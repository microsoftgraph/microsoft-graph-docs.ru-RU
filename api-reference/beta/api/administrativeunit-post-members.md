---
title: Добавление участника
description: Используйте этот API для добавления участника (пользователя, группы или устройства) в административное подразделение.
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cfe40b6d418759c3087eb31f4e0b9dcf5fd87fe9
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63669412"
---
# <a name="add-a-member"></a>Добавление участника

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте этот API, чтобы добавить члена (пользователя, группы или устройства) в административное подразделение или создать новую группу в административном подразделении. Все [типы групп](/graph/api/resources/groups-overview) могут быть созданы в административном блоке.

**Примечание:** В настоящее время в административное подразделение можно добавлять только один член одновременно.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="permissions-to-add-an-existing-user-group-or-device"></a>Разрешения на добавление существующего пользователя, группы или устройства
|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AdministrativeUnit.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | AdministrativeUnit.ReadWrite.All |

### <a name="permissions-to-create-a-new-group"></a>Разрешения на создание новой группы
|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.ReadWrite.All, Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Следующий запрос добавляет существующего пользователя, группы или устройства в административное подразделение.
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```

Следующий запрос создает новую группу в административном подразделении.
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members
```

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {token}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

### <a name="adding-an-existing-user-or-group"></a>Добавление существующего пользователя или группы
В теле запроса укажи`id`, что [пользователь, группа](../resources/user.md)[,](../resources/group.md) [устройство](../resources/device.md) или [directoryObject](../resources/directoryobject.md) будут добавлены.

### <a name="creating-a-new-group"></a>Создание новой группы
В следующей таблице показаны свойства группового [ресурса,](../resources/group.md) которые необходимо указать при создании группы в административном блоке. 

| Свойство | Тип | Описание|
|:---------------|:--------|:----------|
| displayName | string | Имя, которое следует отобразить в адресной книге для группы. Обязательно. |
| description | строка | Описание группы. Необязательно. |
| isAssignableToRole | Логическое | Значение **true**, чтобы группу можно было назначить роли Azure AD. Только администратор привилегированных ролей и глобальный администратор может настроить значение этого свойства. Необязательно. |
| mailEnabled | boolean | Установите значение **true** для групп, поддерживающих почту. Обязательно. |
| mailNickname | string | Почтовый псевдоним для группы. Такие символы нельзя использовать в mailNickName: `@()\[]";:.<>,SPACE`. Обязательный. |
| securityEnabled | boolean | Значение **true** для групп безопасности, включая группы Microsoft 365. Обязательный. |
| owners | Коллекция [directoryObject](../resources/directoryobject.md) | Это свойство представляет владельцев группы на момент создания. Необязательно. |
| members | Коллекция [directoryObject](../resources/directoryobject.md) | Это свойство представляет участников группы на момент создания. Необязательно. |
|visibility|String|Определяет видимость группы Microsoft 365. Возможные значения: `Private`, `Public`, `HiddenMembership` или пустое значение (обрабатывается как `Public`).|

## <a name="response"></a>Отклик

Если это успешно, добавление существующего объекта (с помощью `$ref`) возвращает `204 No Content` код ответа. Метод не возвращает данные в теле отклика. 

При создании новой группы (без `$ref`) `201 Created` этот метод возвращает код [ответа и объект](../resources/group.md) группы в тексте ответа. Отклик включает в себя только свойства по умолчанию для группы.

## <a name="examples"></a>Примеры
### <a name="example-1-add-an-existing-user-or-group"></a>Пример 1. Добавление существующего пользователя или группы
Ниже приводится добавление существующего пользователя или группы в административное подразделение.

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_administrativeunits_members_ref"
} -->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-administrativeunits-members-ref-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-administrativeunits-members-ref-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-administrativeunits-members-ref-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-administrativeunits-members-ref-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/post-administrativeunits-members-ref-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/post-administrativeunits-members-ref-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



В теле запроса укажи `id` объект [пользователя](../resources/user.md)[, группы](../resources/group.md) или [устройства](../resources/device.md), который необходимо добавить.

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
 
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "post_administrativeunits_members_ref"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-create-a-new-group"></a>Пример 2. Создание новой группы
В следующем примере создается новая группа в административном подразделении.

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_administrativeunits_members"
} -->
``` http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#Microsoft.Graph.Group",
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-administrativeunits-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-administrativeunits-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-administrativeunits-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-administrativeunits-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/post-administrativeunits-members-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



В теле запроса укажи свойства объекта [группы](../resources/group.md) , который необходимо добавить.

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "post_administrativeunits_members"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
     "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-22T02:21:05Z",
     "description": "Self help community for golf",
     "displayName": "Golf Assist",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
   "isAssignableToRole": null,
     "mail": "golfassist@contoso.com",
     "mailEnabled": true,
     "mailNickname": "golfassist",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:golfassist@contoso.onmicrosoft.com"
     ],
     "renewedDateTime": "2018-12-22T02:21:05Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
   "securityIdentifier": "S-1-12-1-1753967289-1089268234-832641959-555555555",
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```
