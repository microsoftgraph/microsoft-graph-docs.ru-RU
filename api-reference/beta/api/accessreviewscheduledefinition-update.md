---
title: Обновление accessReviewScheduleDefinition
description: Обнови существующий объект accessReviewScheduleDefinition, чтобы изменить одно или несколько его свойств.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 149ea6004caf2c3f74003fd17815bda92d74b0b2
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "62815862"
---
# <a name="update-accessreviewscheduledefinition"></a>Обновление accessReviewScheduleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обнови [существующий объект accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) , чтобы изменить одно или несколько его свойств.

>[!NOTE]
>Любые обновления, сделанные в accessReviewScheduleDefinition, применяются только к будущим экземплярам. В настоящее время запущенные экземпляры не могут быть обновлены.
>Кроме того, этот API не предназначен для обновления свойств, включая решения, на уровне accessReviewInstance. Дополнительные сведения о экземплярах см. в [accessReviewInstance](../resources/accessreviewinstance.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application                            | AccessReview.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
|Авторизация|Bearer {token}. Обязательный.|
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .

В следующей таблице показаны свойства, принятые для обновления accessReviewScheduleDefinition.

| Свойство | Тип | Описание |
|:-------------|:------------|:------------|
| descriptionForAdmins | Строка | Контекст обзора, предоставленного администраторам. |
| descriptionForReviewers | Строка | Контекст обзора, предоставленного рецензентам. |
| displayName | String | Имя серии обзоров доступа. |
| fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|Коллекция областей рецензентов, используемых для определения списка рецензентов откатов, которые уведомлены о необходимости принятия мер, если пользователи не найдены из указанного списка рецензентов. Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует.|
| рецензенты | [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|  Определяет, кто такие рецензенты. Если нет указаны, обзор является самообнаверяемой (пользователи просматривают собственный доступ). Свойство **рецензентов** может быть updatable только в том случае, если отдельные пользователи назначены в качестве рецензентов. См [. accessReviewReviewerScope](../resources/accessreviewreviewerscope.md). |
|stageSettings|[accessReviewStageSettings](../resources/accessreviewstagesettings.md) collection| Определяет, сколько этапов будет иметь каждый экземпляр серии обзоров доступа. Этапы будут создаваться последовательно на основе **свойства dependsOn** . На каждом этапе может быть разный набор рецензентов, рецензентов и параметров. Только рецензенты и рецензенты отката являются updatable. См [. в странице accessReviewStageSettings](../resources/accessreviewstagesettings.md). Необязательное свойство.|
| settings | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md) | Параметры для серии обзоров доступа. См [. accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md). |
| backupReviewers (обесценив)|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection| Это свойство было заменено **на fallbackReviewers**. Однако указание резервных **копийReviewers** или **fallbackReviewers** автоматически заполняет те же значения для другого свойства. |

Запрос **PUT** предполагает, что будет передан полный объект, который включает в себя все свойства, которые можно использовать, а не только обновляемые свойства.

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код `204 No Content` ответа и не возвращает текст ответа.

## <a name="examples"></a>Примеры

Это пример обновления displayName существующей серии обзоров доступа.

### <a name="request"></a>Запрос
В теле запроса поставляют представление JSON о новых свойствах [объекта accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewScheduleDefinition"
}-->
```http
PUT https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6
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
