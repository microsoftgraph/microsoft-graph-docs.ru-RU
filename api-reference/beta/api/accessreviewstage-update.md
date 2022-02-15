---
title: Обновление accessReviewStage
description: Обновление свойств объекта accessReviewStage.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3441d93ab31270915fb1139e30c65e67ab28a197
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816186"
---
# <a name="update-accessreviewstage"></a>Обновление accessReviewStage
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [accessReviewStage](../resources/accessreviewstage.md) . Обновить **можно только свойства** **рецензентов и fallbackReviewers** . В свойство **fallbackReviewers** можно добавить только рецензентов, но не удалить существующие **fallbackReviewers**.

Чтобы обновить **accessReviewStage**, его **состояние** должно быть `NotStarted`, или `Initializing``InProgress`.

> [!NOTE]
> 
> Обновление **accessReviewStage** будет обновлять только этот этап. Родительский **accessReviewInstance** и любые будущие **объекты accessReviewStage** не изменятся. Чтобы сделать обновления, применимые ко всем будущим экземплярам и этапам, обновите родительский [объект accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .

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
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|рецензенты|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|Эта коллекция областей обзора доступа используется для определения того, кто такие рецензенты. Примеры вариантов назначения рецензентов см. в примере Назначение рецензентов определению обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-scope-concept) Необязательное свойство. Updatable.|
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|Эта коллекция областей рецензентов используется для определения списка рецензентов откатов. Эти рецензенты откатов будут уведомлены о необходимости принятия мер, если пользователи не будут найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует. Необязательное свойство. Updatable.|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` отклика и обновленный [объект accessReviewStage](../resources/accessreviewstage.md) в тексте ответа.

Попытка удалить существующие **fallbackReviewers** возвращает код `409 Conflict` ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_accessreviewstage"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5dcfcc88-da88-4252-8629-a0807b4b076d/instances/720b8ee0-cee4-42ac-b164-894c48703acc/stages/7d244ab1-4ab1-7d24-b14a-247db14a247d
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewStage",
  "reviewers": [
      {
          "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
          "queryType": "MicrosoftGraph"
      }
  ],
  "fallbackReviewers": [
      {
          "query": "/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
          "queryType": "MicrosoftGraph"
      },
      {
          "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
          "queryType": "MicrosoftGraph"
      }
  ]
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewStage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewStage",
  "id": "7d244ab1-4ab1-7d24-b14a-247db14a247d",
  "startDateTime": "2021-12-14T11:15:43.207Z",
  "endDateTime": "2021-12-15T11:15:43.207Z",
  "status": "InProgress",
  "reviewers": [
      {
          "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
          "queryType": "MicrosoftGraph"
      }
  ],
  "fallbackReviewers": [
      {
          "query": "/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
          "queryType": "MicrosoftGraph"
      },
      {
          "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
          "queryType": "MicrosoftGraph"
      }
  ]
}
```

