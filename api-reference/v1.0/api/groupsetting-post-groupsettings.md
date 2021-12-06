---
title: Создание параметра группы
description: Создайте новый параметр на основе шаблонов, доступных в groupSettingTemplates.
ms.localizationpriority: medium
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e3d12a07920f7c27386be09ec19b2e677dfd86a3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993130"
---
# <a name="create-a-group-setting"></a>Создание параметра группы

Пространство имен: microsoft.graph

Используйте этот API для создания нового параметра на основе шаблонов, доступных в [groupSettingTemplates.](../resources/groupsettingtemplate.md) Эти параметры могут быть на уровне клиента или на уровне группы. Запрос на создание должен предоставить [параметрValues](../resources/settingvalue.md) для всех параметров, определенных в шаблоне. Для параметров, определенных для группы, можно установить только параметр, регуляющий, могут ли члены группы приглашать гостевых пользователей. Это будет регулировать такое поведение после того, как будет доступна возможность добавлять гостевых пользователей в группу. Для конечных точек бета-версии используйте [directorySettingTemplates.](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta&preserve-view=true)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---------------|:----------|
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type | application/json |

## <a name="request-body"></a>Текст запроса
В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON. Отображаемое имя для параметра будет задано с учетом имени указанного шаблона параметров.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [groupSetting](../resources/groupsetting.md) в теле отклика.

## <a name="example-1-create-a-new-setting-for-all-microsoft-365-groups-in-the-tenant"></a>Пример 1. Создание нового параметра для всех Microsoft 365 групп в клиенте

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json

{
  "displayName": "Group.Unified",
  "templateId": "62375ab9-6b52-47ed-826b-58e47e0e304b",
  "values": [
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": "https://privacy.contoso.com/privacystatement"
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "true"
    },
    {
      "name": "EnableMIPLabels",
      "value": "true"
    },
    {
      "name": "PrefixSuffixNamingRequirement",
      "value": "[Contoso-][GroupName]"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-groupsetting-from-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-groupsetting-from-groupsettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON.

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettings/$entity",
  "id": "b11b99c5-f0a3-4c32-a250-548cf11cae1c",
  "displayName": "Group.Unified",
  "templateId": "62375ab9-6b52-47ed-826b-58e47e0e304b",
  "values": [
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": "https://privacy.contoso.com/privacystatement"
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "true"
    },
    {
      "name": "EnableMIPLabels",
      "value": "true"
    },
    {
      "name": "PrefixSuffixNamingRequirement",
      "value": "[Contoso-][GroupName]"
    }
  ]
}
```

## <a name="example-2-create-a-setting-to-block-guests-for-a-specific-microsoft-365-group"></a>Пример 2. Создание параметра для блокировки гостей для определенной Microsoft 365 группы

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings_for_guests"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/055a5d18-a3a9-4338-b9c5-de92559b7ebf/settings
Content-type: application/json

{
  "displayName": "Group.Unified.Guest",
  "templateId": "08d542b9-071f-4e16-94b0-74abb372e3d9",
  "values": [
    {
      "name": "AllowToAddGuests",
      "value": "false"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-groupsetting-from-groupsettings-for-guests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-for-guests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-for-guests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-for-guests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-groupsetting-from-groupsettings-for-guests-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON.

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettings/$entity",
  "id": "2a0248a2-fde9-4a80-a53e-c0141f68e03d",
  "displayName": "Group.Unified.Guest",
  "templateId": "08d542b9-071f-4e16-94b0-74abb372e3d9",
  "values": [
    {
      "name": "AllowToAddGuests",
      "value": "false"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

