---
title: Обновление accessReviewScheduleDefinition
description: Обновление свойств объекта accessReviewScheduleDefinition.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: dbcf0095cb2f3a5fece6ea12821183f9a77d63dd
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697689"
---
# <a name="update-accessreviewscheduledefinition"></a>Обновление accessReviewScheduleDefinition
Пространство имен: microsoft.graph

Обновление свойств объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .

Все обновления accessReviewScheduleDefinition применяются только к будущим экземплярам. В настоящее время не удается обновить запущенные экземпляры. Кроме того, этот API не предназначен для обновления свойств, включая решения, на уровне accessReviewInstance. Дополнительные сведения об экземплярах см. в [accessReviewInstance](../resources/accessreviewinstance.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|AccessReview.ReadWrite.All|

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
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Основной текст запроса
В тексте запроса добавьте представление объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в формате JSON.

В следующей таблице показаны свойства, принятые для обновления accessReviewScheduleDefinition.

| Свойство | Тип | Описание |
|:-------------|:------------|:------------|
| displayName | String | Имя ряда проверки доступа. |
| descriptionForAdmins | String | Контекст проверки, предоставленной администраторам. |
| descriptionForReviewers | Строка | Контекст проверки, предоставленной рецензентам. |
| fallbackReviewers |[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Коллекция областей рецензентов, используемых для определения списка резервных рецензентов, которые получают уведомление о том, что нужно принять меры, если пользователи не найдены в указанном списке рецензентов. Это может произойти, если владелец группы указан в качестве рецензента, но владелец группы не существует, или руководитель указан в качестве рецензента, но руководитель пользователя не существует.|
| Авторам | [Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|  Определяет, кто является рецензентом. Если они не указаны, проверка выполняется самостоятельно (пользователи проверяют собственный доступ). Свойство **рецензентов** можно обновить только в том случае, если отдельные пользователи назначены рецензентами. См [. accessReviewReviewerScope](../resources/accessreviewreviewerscope.md). |
| settings | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md) | Параметры для ряда проверки доступа. См [. accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md). |

Запрос **PUT** ожидает передачи полного объекта, который включает все записываемые свойства, а не только обновляемые свойства.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `204 No Content` отклика без текста ответа.

## <a name="examples"></a>Примеры
Это пример обновления displayName существующего ряда проверки доступа.

### <a name="request"></a>Запрос

В тексте запроса добавьте представление новых свойств объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в формате JSON.



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
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "instanceEnumerationScope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
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
