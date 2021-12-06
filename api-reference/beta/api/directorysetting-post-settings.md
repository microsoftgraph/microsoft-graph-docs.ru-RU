---
title: Создание параметра каталога
description: Используйте этот API для создания нового параметра на основе шаблонов, доступных в directorySettingTemplates.
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fc20d310f9b009ae30edf1936e2a33a1f49ee3b9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982084"
---
# <a name="create-a-directory-setting"></a>Создание параметра каталога

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте этот API для создания нового параметра на основе шаблонов, доступных в directorySettingTemplates. Эти параметры могут быть на уровне клиента или на уровне объекта (в настоящее время только для групп). Запрос на создание должен предоставить параметрValues для всех параметров, определенных в шаблоне. Для параметров, определенных для группы, можно установить только параметр, регуляющий, могут ли члены группы приглашать гостевых пользователей. Это будет регулировать такое поведение после того, как будет доступна возможность добавлять гостевых пользователей в группу.

> **Примечание.** Бета-версия этого API применяется только к группам. Версия /v1.0 этого API переименована в *Create groupSettings.*

Для списка шаблонов и свойств, которые они поддерживают в бета-версии, используйте [запрос directorySettingTemplate](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta). (Для конечных точек v1.0 вызываемая [группаSettingTemplates.)](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)


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
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [directorySetting.](../resources/directorysetting.md)  Однако имя отображения для параметра будет устанавливаться на основе имени шаблона ссылок параметров.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект directorySetting](../resources/directorysetting.md) в тексте ответа.

## <a name="example-1-create-a-new-setting-for-all-microsoft-365-groups-in-the-tenant"></a>Пример 1. Создание нового параметра для всех Microsoft 365 групп в клиенте

### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
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
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directorysetting-from-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directorysetting-from-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-directorysetting-from-settings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


В теле запроса поставляем представление JSON объекта [directorySetting.](../resources/directorysetting.md)

### <a name="response"></a>Отклик
Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#settings/$entity",
  "id": "f0b2d6f5-097d-4177-91af-a24e530b53cc",
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
  "name": "create_directorysetting_from_settings_for_guests"
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
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-settings-for-guests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-settings-for-guests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directorysetting-from-settings-for-guests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directorysetting-from-settings-for-guests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-directorysetting-from-settings-for-guests-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


В теле запроса поставляем представление JSON объекта [directorySetting.](../resources/directorysetting.md)

### <a name="response"></a>Отклик

Примечание. Показанный здесь объект ответа может быть сокращен для читаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#settings/$entity",
  "id": "a77ad44e-aa2a-4976-91b5-b947787b9577",
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
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
