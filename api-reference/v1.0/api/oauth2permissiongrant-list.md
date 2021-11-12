---
title: Список oAuth2PermissionGrants (делегирование разрешений)
description: Получение списка объектов oauth2PermissionGrant, представляющих делегированную дотации разрешений.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 63b96796732d73f841e4d6f7b874e80a9a614bdd
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891174"
---
# <a name="list-oauth2permissiongrants-delegated-permission-grants"></a>Список oauth2PermissionGrants (делегирование разрешений)

Пространство имен: microsoft.graph

Получение списка [объектов oAuth2PermissionGrant,](../resources/oauth2permissiongrant.md) представляющих делегированную лицензию, выданную для клиентских приложений для доступа к API от имени пользователей, входиющих в нее.

> [!NOTE]
> При запросе могут происходить задержки репликации для предоставленных делегированных разрешений, которые были недавно созданы, обновлены или удалены. При указании фильтра эта задержка будет сведена `clientId` к минимуму.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_oauth2permissiongrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#oauth2PermissionGrants",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/oauth2PermissionGrants/AVs6JuUDjkCFV7q2gd8QTPimBBgj5iBFj0C6GwwRxC0",
            "clientId": "263a5b01-03e5-408e-8557-bab681df104c",
            "consentType": "AllPrincipals",
            "id": "AVs6JuUDjkCFV7q2gd8QTPimBBgj5iBFj0C6GwwRxC0",
            "principalId": null,
            "resourceId": "1804a6f8-e623-4520-8f40-ba1b0c11c42d",
            "scope": "User.Read Group.ReadWrite.All"
        },
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/oauth2PermissionGrants/AVs6JuUDjkCFV7q2gd8QTOQDNpSH5-lPk9HjD3Sarjk",
            "clientId": "263a5b01-03e5-408e-8557-bab681df104c",
            "consentType": "AllPrincipals",
            "id": "AVs6JuUDjkCFV7q2gd8QTOQDNpSH5-lPk9HjD3Sarjk",
            "principalId": null,
            "resourceId": "943603e4-e787-4fe9-93d1-e30f749aae39",
            "scope": "Tasks.ReadWrite Files.ReadWrite.All Files.ReadWrite Contacts.ReadWrite Calendars.ReadWrite Mail.ReadWrite Directory.AccessAsUser.All Directory.ReadWrite.All Group.ReadWrite.All Group.Read.All User.ReadWrite Mail.ReadWrite.Shared Mail.Send.Shared Calendars.ReadWrite.Shared Contacts.ReadWrite.Shared Tasks.ReadWrite.Shared Sites.ReadWrite.All Files.ReadWrite.AppFolder Files.ReadWrite.Selected Notes.ReadWrite Notes.ReadWrite.All MailboxSettings.ReadWrite DeviceManagementManagedDevices.PrivilegedOperations.All DeviceManagementManagedDevices.ReadWrite.All DeviceManagementRBAC.ReadWrite.All DeviceManagementApps.ReadWrite.All DeviceManagementConfiguration.ReadWrite.All openid profile Directory.Read.All User.Read.All User.ReadWrite.All ChannelMember.ReadWrite.All DeviceManagementServiceConfiguration.ReadWrite.All"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

