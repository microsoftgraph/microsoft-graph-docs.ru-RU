---
title: 'accessReviewInstance: batchRecordDecisions'
description: Emable reviewers to review all accessReviewInstanceDecisionItems in batches.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a8bd6778d54100340b0c846230fd8b91b696f1fb
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507503"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a>accessReviewInstance: batchRecordDecisions
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Включить рецензенты для просмотра всех [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) пакетами с помощью `principalId` , или ни `resourceId` один.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReviews.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|AccessReviews.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
| решение  | String | Решение о доступе для проверяемого объекта. Возможные значения: `Approve`, `Deny`, `NotReviewed`, `DontKnow`. Обязательно.  |
|  обоснование | String | Контекст обзора, предоставленного администраторам. Обязательно, **если justificationRequiredOnApproval** находится `True` на **accessReviewScheduleDefinition**.  |
|principalId|String|В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **principalId.** Если они не будут предоставлены, все **principalIds** будут рассмотрены.|
|resourceId|String|В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **resourceId.** Если они не будут предоставлены, **все resourceIds** будут рассмотрены.|



## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
Content-Type: application/json
Content-length: 113

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-batchrecorddecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-batchrecorddecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-batchrecorddecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-batchrecorddecisions-java-snippets.md)]
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
