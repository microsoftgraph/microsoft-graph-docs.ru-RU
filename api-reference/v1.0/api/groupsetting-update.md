---
title: Обновление groupSetting
description: Обновление свойств для указанных объектов параметров группы.
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 604e4275f1b5d49fab3d866b6845d820f67cd0ec
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211279"
---
# <a name="update-groupsetting"></a>Обновление groupSetting

Пространство имен: microsoft.graph

Обновите свойства объекта [groupSetting](../resources/groupsetting.md) для параметров группы на уровне клиента [](../resources/group.md) или определенного параметра группы.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Directory.ReadWrite.All                     |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | Directory.ReadWrite.All                     |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

Обновим параметр на уровне клиента.

```http
PATCH /groupSettings/{groupSettingId}
```

<!-- { "blockType": "ignored" } -->

Обновим параметр для конкретной группы.

```http
PATCH /groups/{groupId}/settings/{groupSettingId}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание        |
| :------------ | :----------------- |
| Авторизация | {token}. Обязательно. |
| Content-Type  | application/json   |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.

| Свойство | Тип                                                    | Описание                                                                                                      |
| :------- | :------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------- |
| values   | [Коллекция settingValue](../resources/settingvalue.md) | Обновленный набор значений. Необходимо включить весь набор сбора. Невозможно обновить один набор значений. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-update-a-tenant-wide-group-setting"></a>Пример 1. Обновление параметра группы на уровне клиента

В этом примере `84af2ca5-c274-41bf-86e4-6e374ec4def6` используется идентификатор объекта **groupSetting на уровне** клиента.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_tenant_groupsetting"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/groupSettings/84af2ca5-c274-41bf-86e4-6e374ec4def6
Content-type: application/json

{
    "values": [
        {
            "name": "AllowToAddGuests",
            "value": "false"
        }
    ]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenant-groupsetting-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenant-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenant-groupsetting-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenant-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenant-groupsetting-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenant-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenant-groupsetting-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/update-tenant-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-tenant-groupsetting-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/update-tenant-groupsetting-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-group-setting"></a>Пример 2. Обновление определенного параметра группы

В этом примере `0167b5af-f3d1-4910-82d2-398747fa381c` — это идентификатор группы и `fa6df613-159b-4f94-add2-7093f961900b` идентификатор объекта groupSetting.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/groups/0167b5af-f3d1-4910-82d2-398747fa381c/settings/fa6df613-159b-4f94-add2-7093f961900b
Content-type: application/json

{
  "values": [
    {
      "name": "AllowToAddGuests",
      "value": "true"
    }
  ]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-groupsetting-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/update-groupsetting-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
