---
title: Обновление АкцессревиевинстанцедеЦисионитем
description: Обновление существующего объекта АкцессревиевинстанцедеЦисионитем, для которого вызывающий пользователь является проверяющим.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2f14ed26169c659354af16963e03e449f246421c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214387"
---
# <a name="update-accessreviewinstancedecisionitem"></a>Обновление АкцессревиевинстанцедеЦисионитем

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление решений Access, известных как [акцессревиевинстанцедеЦисионитемс](../resources/accessreviewinstancedecisionitem.md), для которых пользователь является рецензентом.

>[!NOTE]
>Любые изменения, внесенные в **акцессревиевинстанцедеЦисионитем** , могут выполняться только вызываемыми пользователями, указанными в качестве проверяющего для родительского [акцессревиевинстанце](../resources/accessreviewinstance.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из следующих разрешений. Делегированные разрешения для личных учетных записей Майкрософт не поддерживаются. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
|Авторизация|Bearer {токен}. Обязательный.|
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В следующей таблице приведены свойства, принятые для обновления `accessReviewInstanceDecisionItem` .

| Свойство     | Тип       | Описание |
|:-------------|:------------|:------------|
| решении  | String | Решение о доступе к проверяемой сущности. Возможные значения: `Approve` `Deny` `NotReviewed` `DontKnow` . Обязательный.  |
|  текста | String | Контекст проверки, предоставленной администраторам. Является обязательным, если Жустификатионрекуиредонаппровал имеет значение true для Акцессревиевсчедуледефинитион.  |

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `204, NoContent` код отклика и без текста отклика.

### <a name="request"></a>Запрос
## <a name="examples"></a>Примеры

Это пример утверждающего доступа для пользователя, представленного в `accessReviewInstanceDecisionItem` .


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/654b34e7-b48f-4772-a2d4-08f1d0dd014c

{
  "decision": "Approve",
  "justification": "I trust this person"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
