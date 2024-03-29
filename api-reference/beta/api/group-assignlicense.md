---
title: 'group: assignLicense'
description: Добавьте или удалите лицензии в группе. Лицензии, назначенные группе, будут назначены всем пользователям в группе.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 46b1f78f3341fcd06bb0c2cf592aa8b6c6ceda4b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210726"
---
# <a name="group-assignlicense"></a>group: assignLicense

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавьте или удалите лицензии в группе. Лицензии, назначенные группе, будут назначены всем пользователям в группе. Дополнительные сведения о групповом лицензировании см. в статье о [групповом](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal) лицензировании в Azure Active Directory.

Чтобы получить подписки, доступные в каталоге, выполните [запрос GET subscribedSkus](subscribedsku-list.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)  |
| :------------------------------------- | :------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Group.ReadWrite.All, Directory.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                               |
| Для приложений                            | Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/assignLicense
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                       |
| :------------ | :-------------------------- |
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр      | Тип                                                          | Описание                                                                                                                                                                                                                                                                    |
| :------------- | :------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| addLicenses    | Коллекция [assignedLicense](../resources/assignedlicense.md) | Коллекция объектов [assignedLicense](../resources/assignedlicense.md), указывающих добавляемые лицензии. Вы можете отключить servicePlans, связанные с лицензией, заданное свойство **disabledPlans** для [объекта assignedLicense](../resources/assignedlicense.md) . |
| removeLicenses | Коллекция объектов Guid                                               | Коллекция идентификаторов skuId, определяющий удаляемую лицензию.                                                                                                                                                                                                                   |

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код `202 Accepted` отклика и целевой [объект группы](../resources/group.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-add-licenses-to-the-group"></a>Пример 1. Добавление лицензий в группу

В следующем примере лицензии добавляются в группу.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}-->

```http
POST https://graph.microsoft.com/beta/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/assignLicense
Content-type: application/json

{
  "addLicenses": [
    {
      "disabledPlans": [
        "113feb6c-3fe4-4440-bddc-54d774bf0318",
        "14ab5db5-e6c4-4b20-b4bc-13e36fd2227f"
      ],
      "skuId": "b05e124f-c7cc-45a0-a6aa-8cf78c946968"
    },
    {
      "disabledPlans": [
        "a413a9ff-720c-4822-98ef-2f37c2a21f4c"
      ],
      "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
    }
  ],
  "removeLicenses": []
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-assignlicense-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/group-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-assignlicense-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/group-assignlicense-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/group-assignlicense-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/group-assignlicense-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ответ — это обновленный объект группы.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/e8e96c2a-d787-4eb1-98d7-9e57c965f1de/directoryObjects/1132b215-826f-42a9-8cfe-1643d19d17fd/Microsoft.DirectoryServices.Group

{
  "id": "1132b215-826f-42a9-8cfe-1643d19d17fd",
  "createdDateTime": "2021-03-12T11:15:03Z",
  "groupTypes": [],
  "securityEnabled": true,
}
```

### <a name="example-2-remove-licenses-from-the-group"></a>Пример 2. Удаление лицензий из группы

В следующем примере лицензии удаляются из группы.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_removelicense"
}-->

```http
POST https://graph.microsoft.com/beta/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/assignLicense
Content-type: application/json

{
  "addLicenses": [],
  "removeLicenses": [
    "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "b05e124f-c7cc-45a0-a6aa-8cf78c946968"
  ]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removelicense-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/group-removelicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-removelicense-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/group-removelicense-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/group-removelicense-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/group-removelicense-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ответ — это обновленный объект группы.

> **Примечание:** Показанный здесь объект ответа может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/e8e96c2a-d787-4eb1-98d7-9e57c965f1de/directoryObjects/1132b215-826f-42a9-8cfe-1643d19d17fd/Microsoft.DirectoryServices.Group

{
  "id": "1132b215-826f-42a9-8cfe-1643d19d17fd",
  "createdDateTime": "2021-03-12T11:15:03Z",
  "groupTypes": [],
  "securityEnabled": true,
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
