---
title: 'accessReviewStage: остановка'
description: Остановите этап проверки доступа, который продолжается.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 977f46ff45ec63c1b2ca1e932a8fd8df119faa03
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816189"
---
# <a name="accessreviewstage-stop"></a>accessReviewStage: остановка
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Остановите [этап проверки](../resources/accessReviewStage.md) доступа, который является `inProgress`. После остановки этапа проверки доступа **состояние стадии** `Completed` будет и рецензенты больше не смогут вводить ввод. Если существуют последующие этапы, зависят от завершаемой стадии, будет создан следующий этап. 

[Объекты accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) всегда будут отражать последние решения, записанные на всех этапах заданного времени, независимо от состояния этапов.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application                            | AccessReview.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}/stop
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "accessreviewstage_stop"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stages/5d431f4b-56f2-4a50-938b-fb1e4e2c91b9/stop
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

