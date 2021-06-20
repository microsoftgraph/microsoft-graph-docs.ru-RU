---
title: 'accessReviewInstance: batchRecordDecisions'
description: Позволяет рецензентам просмотреть все accessReviewInstanceDecisionItems пакетами.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ea22d510bb70ab8d7047f952f7b4c0e265d57197
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031333"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a>accessReviewInstance: batchRecordDecisions
Пространство имен: microsoft.graph

Позволяет рецензентам просмотреть все [объекты accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) пакетами с помощью **principalId,** **resourceId** или ни того, ни другго.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложений|AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса подарите JSON представление [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).

В следующей таблице перечислены свойства, которые можно использовать для просмотра [объектов accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)

|Параметр|Тип|Описание|
|:---|:---|:---|
|решение|String|Решение о доступе для проверяемого объекта. Возможные значения: `Approve`, `Deny`, `NotReviewed`, `DontKnow`. Обязательный.|
|обоснование|String|Контекст обзора, предоставленного администраторам. Требуется, **если обоснованиеRequiredOnApproval** свойства параметров **accessReviewScheduleDefinition** является `true` .|
|principalId|String|В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **значениям principalId.** Если они не будут предоставлены, **все accessReviewInstanceDecisionItems** будут рассмотрены.|
|resourceId|String|В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **resourceId.** Если они не будут предоставлены, **все accessReviewInstanceDecisionItems** будут рассмотрены.|

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-6778-8868-9999c7f4cc06/batchRecordDecisions
Content-type: application/json

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
