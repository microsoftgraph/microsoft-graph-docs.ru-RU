---
title: Обновление accessReviewInstanceDecisionItem
description: Обновление свойств объекта accessReviewInstanceDecisionItem.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ca2f5c24f10bd287b73502ec3d8ba5b6c399da18
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209621"
---
# <a name="update-accessreviewinstancedecisionitem"></a>Обновление accessReviewInstanceDecisionItem
Пространство имен: microsoft.graph

Обновление свойств объекта [accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|AccessReview.ReadWrite.All|

Обновить **accessReviewInstanceDecisionItem** может только пользователь вызовов, который указан в качестве рецензента для родительского доступаReviewInstanceDecisionItem. [](../resources/accessreviewinstance.md)

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса подарите JSON представление [объекта accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)

В следующей таблице показаны свойства, которые принимаются при обновлении [accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|решение|String|Проверятель голосует о том, должен ли директор иметь доступ к просматриваемом ресурсу. Возможные значения: `Approve` `Deny` , или `DontKnow` . Обязательно.|
|обоснование|String|Причина принятия решения рецензентом. Требуется, если **обоснованиеRequiredOnApproval** свойства параметров [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) `true` является .|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 OK`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewinstancedecisionitem"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/4444f3b6-8ea4-4dea-90a5-9eac8fe95678/decisions/5555f3b6-8ea4-4dea-90a5-9eac8fe95555
Content-Type: application/json
Content-length: 691

{
  "decision": "Approve",
  "justification": "Kathleen still needs access to the Marketing group as she works in the Marketing organization."
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



### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
