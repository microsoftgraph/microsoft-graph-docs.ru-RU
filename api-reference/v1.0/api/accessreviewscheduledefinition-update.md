---
title: Обновление accessReviewScheduleDefinition
description: Обновление свойств объекта accessReviewScheduleDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 72fcf71b4b0e78006ad30b2091b6906342e18edf
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384056"
---
# <a name="update-accessreviewscheduledefinition"></a>Обновление accessReviewScheduleDefinition
Пространство имен: microsoft.graph

Обновление свойств объекта [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)

Любые обновления accessReviewScheduleDefinition применяются только к будущим экземплярам. В настоящее время запущенные экземпляры не могут быть обновлены. Кроме того, этот API не предназначен для обновления свойств, включая решения, на уровне accessReviewInstance. Дополнительные сведения о экземплярах см. в [accessReviewInstance.](../resources/accessreviewinstance.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)

В следующей таблице показаны свойства, принятые для обновления accessReviewScheduleDefinition.

| Свойство | Тип | Описание |
|:-------------|:------------|:------------|
| displayName | String | Имя серии обзоров доступа. |
| descriptionForAdmins | Строка | Контекст обзора, предоставленного администраторам. |
| descriptionForReviewers | Строка | Контекст обзора, предоставленного рецензентам. |
| settings | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md) | Параметры для серии обзоров доступа. См. [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md). |
| рецензенты | [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|  Определяет, кто такие рецензенты. Если нет указаны, обзор является самообнаверяемой (пользователи просматривают собственный доступ). Свойство **рецензентов** может быть updatable только в том случае, если отдельные пользователи назначены в качестве рецензентов. См. [accessReviewReviewerScope.](../resources/accessreviewreviewerscope.md) |
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|Коллекция областей рецензентов, используемых для определения списка рецензентов откатов, которые уведомлены о необходимости принятия мер, если пользователи не найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует.|

Запрос **PUT** предполагает, что будет передан полный объект, который включает в себя все свойства, которые можно использовать, а не только обновляемые свойства.

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код `204 No Content` ответа и не возвращает текст ответа.

## <a name="examples"></a>Примеры
Это пример обновления displayName существующей серии обзоров доступа.

### <a name="request"></a>Запрос

В теле запроса поставляют представление JSON о новых свойствах [объекта accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewscheduledefinition"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6
Content-type: application/json

{
  "id": "60860cdd-fb4d-4054-91ba-f75e04444aa6",
  "displayName": "Test world UPDATED NAME!",
  "descriptionForAdmins": "Test world",
  "descriptionForReviewers": "Test world",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "instanceEnumerationScope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 3,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-15"
      }
    }
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
