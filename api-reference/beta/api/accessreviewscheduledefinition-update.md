---
title: Обновление accessReviewScheduleDefinition
description: Обновление существующего объекта accessReviewScheduleDefinition, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 57d1be0916331e342c5d37a29daf2785afe3c644
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943597"
---
# <a name="update-accessreviewscheduledefinition"></a>Обновление accessReviewScheduleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление существующего [объекта accessReviewScheduleDefinition,](../resources/accessreviewscheduledefinition.md) чтобы изменить одно или несколько его свойств.

>[!NOTE]
>Любые обновления accessReviewScheduleDefinition применяются только к будущим экземплярам. В настоящее время не удается обновить запущенные экземпляры.
>Кроме того, этот API не предназначен для обновления свойств, включая решения, на уровне accessReviewInstance. Дополнительные сведения об [экземплярах см. в accessReviewInstance.](../resources/accessreviewinstance.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение                            | AccessReview.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
|Авторизация|Bearer {токен}. Обязательный.|
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса предопределение представления объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в JSON.

В следующей таблице показаны свойства, принятые для обновления объекта accessReviewScheduleDefinition.

| Свойство | Тип | Описание |
|:-------------|:------------|:------------|
| displayName | String | Название серии отзывов о доступе. |
| descriptionForAdmins | String | Контекст проверки, предоставленной администраторам. |
| descriptionForReviewers | String | Контекст отзыва, предоставленного рецензентам. |
| settings | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md) | Параметры для серии отзывов о доступе. См. [accessReviewScheduleSettings.](../resources/accessreviewscheduledefinition.md) |
| рецензенты | [Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|  Определяет, кто такие рецензенты. Если ни один из них не указан, отзыв будет самообнаправлением (пользователи просмотрели свой собственный доступ). Свойство "Рецензенты" может быть только updatable, если отдельные пользователи назначены как рецензенты. См. [accessReviewReviewerScope.](../resources/accessreviewscheduledefinition.md) | 

Обратите внимание, что запрос PUT предполагает, что будет передан весь объект, в который включаются все свойства, в которые можно вписать, а не только обновляемые свойства.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код `204, Accepted` отклика без тела отклика.

## <a name="examples"></a>Примеры

Это пример обновления displayName существующего ряда отзывов о доступе.

### <a name="request"></a>Запрос
В теле запроса предопределение представления новых свойств объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в JSON.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewScheduleDefinition"
}-->
```http
PUT https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6

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
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
