---
title: Обновление группы
description: Обновление свойств [группового](../resources/group.md) объекта.
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 537d0d778c434b0c11448af43621d2f15746d552
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030113"
---
# <a name="update-group"></a>Update group

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств [группового](../resources/group.md) объекта.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Укажите в тексте запроса *только* значения обновляемых свойств. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. 

В следующей таблице указаны свойства, которые можно обновить. 

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|allowExternalSenders|Логический|Значение по умолчанию: `false`. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.|
|autoSubscribeNewMembers|Логический|Значение по умолчанию: `false`. Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте. **AutoSubscribeNewMembers** не может быть `true`, если в группе установлено `false` для **subscriptionEnabled**.|
|description|String|Необязательное описание для группы.|
|displayName|String|Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. |
|mailNickname|String|Почтовый псевдоним для группы (уникальный в организации). Максимальная длина: 64 символа. Это свойство может содержать только символы из [набора символов ASCII от 0 до 127](/office/vba/language/reference/user-interface-help/character-set-0127), за исключением следующих: ` @ () \ [] " ; : . <> , SPACE`. |
|preferredDataLocation|String|Предпочтительное расположение данных для группы Microsoft 365. Чтобы обновить это свойство, вызывающему пользователю должна быть назначена одна из указанных ниже ролей Azure AD. <br><ul><li> Глобальный администратор <li> Администратор учетных записей пользователей <li> Поддержка партнеров уровня 1 или уровня 2 <li>Редактор каталогов <li> Администратор Exchange <li> Администратор SharePoint </ul> <br/>Дополнительные сведения об этом свойстве см. в статье [OneDrive Online с поддержкой нескольких регионов](/sharepoint/dev/solution-guidance/multigeo-introduction).|
|securityEnabled|Логический|Указывает, является ли группа группой безопасности, в том числе Microsoft 365 группами. |
|visibility|String|Определяет видимость группы Microsoft 365. Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).|

Поскольку **ресурс группы** поддерживает [расширения,](/graph/extensibility-overview)вы можете использовать операцию для добавления, обновления или удаления собственных данных, определенных для приложения, в настраиваемом свойстве расширения в существующем экземпляре `PATCH` группы. 

> [!IMPORTANT]
>
> + Чтобы обновить следующие свойства, укажите их в собственном запросе PATCH, не включая другие свойства, перечисленные в таблице выше: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.
>
> + Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](/graph/known-issues#groups).
>
> + Правила обновления групп безопасности, поддерживающих почту, в Microsoft Exchange Server могут быть сложными. Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange Server](/Exchange/recipients/mail-enabled-security-groups).



## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `204 No Content`, за исключением кода отклика `200 OK` при обновлении следующих свойств: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.

## <a name="examples"></a>Примеры

### <a name="example-1-update-display-name-and-description-of-a-group"></a>Пример 1. Обновление имени отображения и описания группы
#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json

{
   "description":"Contoso Life v2.0",
   "displayName":"Contoso Life Renewed"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-group-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-a-microsoft-365-group"></a>Пример 2. Применение метки конфиденциальности к группе Microsoft 365
#### <a name="request"></a>Запрос

Вы можете получить ID метки, которая будет применяться к группе Microsoft 365 с помощью [метки List.](informationprotectionpolicy-list-labels.md) Затем вы можете обновить свойство [назначенногоLabels](../resources/assignedlabel.md) группы с помощью ID метки. 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json

{
  "assignedLabels": 
  [
    {
        "labelId" : "45cd0c48-c540-4358-ad79-a3658cdc5b88"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-group-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](/graph/extensibility-open-users)
- [Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
