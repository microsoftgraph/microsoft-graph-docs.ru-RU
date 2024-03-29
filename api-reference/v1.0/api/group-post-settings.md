---
title: Создание параметров
description: Создайте новый параметр на основе шаблонов, доступных в groupSettingTemplates.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ef409744ee99cbf39648252b3d192fb235060943
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211286"
---
# <a name="create-settings"></a>Создание параметров

Пространство имен: microsoft.graph

Создайте новый параметр на основе шаблонов, доступных в [groupSettingTemplates](../resources/groupsettingtemplate.md). Эти параметры могут быть на уровне клиента или на уровне группы.

Параметры группы применяются только к Microsoft 365 группам. Именованный `Group.Unified` шаблон можно использовать для настройки параметров группы Microsoft 365 на уровне клиента, `Group.Unified.Guest` а именованный шаблон можно использовать для настройки параметров конкретной группы.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Directory.ReadWrite.All                     |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | Directory.ReadWrite.All                     |

## <a name="http-request"></a>HTTP-запрос

Создайте параметр на уровне клиента.

<!-- { "blockType": "ignored" } -->

```http
POST /groupSettings
```

Создайте параметр для конкретной группы.

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/settings
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type  | application/json          |

## <a name="request-body"></a>Текст запроса

В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON. Отображаемое имя, templateId и описание наследуются от объекта [groupSettingTemplates](../resources/groupsettingtemplate.md) , на который указывает ссылка. Только свойство value можно изменить со значения по умолчанию.

При создании объекта [groupSetting](../resources/groupsetting.md) требуются следующие свойства.

| Параметр  | Тип                                                    | Описание                                                                                                                                                                          |
| :--------- | :------------------------------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| templateId | Строка                                                  | Уникальный идентификатор объекта [groupSettingTemplates](../resources/groupsettingtemplate.md) на уровне клиента, используемого для создания этого объекта параметров уровня группы. Только для чтения.              |
| values     | [Коллекция settingValue](../resources/settingvalue.md) | Коллекция пар "имя-значение", соответствующих свойствам **name** и **defaultValue** в объекте [groupSettingTemplates](../resources/groupsettingtemplate.md) , на который указывает ссылка. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [groupSetting](../resources/groupsetting.md) в теле отклика.

## <a name="example-1-create-a-new-setting-for-all-microsoft-365-groups-in-the-tenant"></a>Пример 1. Создание нового параметра для всех Microsoft 365 групп в клиенте

### <a name="request"></a>Запрос

Только [именованный объект groupSettingTemplates](../resources/groupsettingtemplate.md) `Group.Unified` может применяться ко Microsoft 365 групп на уровне клиента.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->

```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json

{
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
[!INCLUDE [sample-code](../includes/snippets/csharp/create-groupsetting-from-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-groupsetting-from-groupsettings-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/create-groupsetting-from-groupsettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

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
    "id": "844d252c-4de2-43eb-a784-96df77231aae",
    "displayName": null,
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

Свойство **displayName** и другие пары "имя-значение" будут заполнены значениями по умолчанию из объекта [groupSettingTemplates](../resources/groupsettingtemplate.md) , соответствующего **templateId**.

## <a name="example-2-create-a-setting-to-block-guests-for-a-specific-microsoft-365-group"></a>Пример 2. Создание параметра для блокировки гостей для определенной Microsoft 365 группы

### <a name="request"></a>Запрос

Только [именованный объект groupSettingTemplates](../resources/groupsettingtemplate.md) `Group.Unified.Guest` может применяться к определенным Microsoft 365 группам.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings_for_guests"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/055a5d18-a3a9-4338-b9c5-de92559b7ebf/settings
Content-type: application/json

{
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
[!INCLUDE [sample-code](../includes/snippets/csharp/create-groupsetting-from-groupsettings-for-guests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-for-guests-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-for-guests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-for-guests-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-for-guests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-for-guests-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-for-guests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-groupsetting-from-groupsettings-for-guests-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/create-groupsetting-from-groupsettings-for-guests-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

В теле запроса предоставьте описание объекта [groupSetting](../resources/groupsetting.md) в формате JSON.

### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

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
    "id": "a06fa228-3042-4662-bd09-33e298da1afe",
    "displayName": null,
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
