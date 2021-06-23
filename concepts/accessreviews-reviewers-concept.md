---
title: Назначение рецензентов для проверки доступа с помощью API Graph Microsoft
description: Узнайте, как использовать API обзоров доступа в Microsoft Graph для назначения рецензентов доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 656541211226f133045a7cdbf74a72b4bcd8c369
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060516"
---
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a>Назначение рецензентов для проверки доступа с помощью API Graph Microsoft

API обзоров доступа Azure [AD](/graph/api/resources/accessreviewsv2-root) позволяет программным образом просмотреть доступ пользователей, директоров служб или групп к ресурсам Azure AD.

Основные рецензенты настроены в свойстве **рецензентов** ресурса [accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition)  Кроме того, вы можете указать рецензенты откатов с помощью **свойства fallbackReviewers.** Эти свойства не требуются при создании самообзора (когда пользователи просматривают собственный доступ).

## <a name="configure-reviewers"></a>Настройка рецензентов

Чтобы настроить рецензентов и рецензентов, задайте значения **запросов,** **queryRoot** и **queryType** свойств **accessReviewReviewerScope**. Описание этих свойств см. в виде [ресурса accessReviewReviewerScope.](/graph/api/resources/accessreviewreviewerscope)

### <a name="example-1-a-specific-user-as-the-reviewer"></a>Пример 1. Конкретный пользователь в качестве рецензента

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-2-members-of-a-group-as-reviewers"></a>Пример 2. Члены группы в качестве рецензентов

```http
"reviewers": [
    {
        "query": "/groups/{group id}}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-3-group-owners-as-reviewers"></a>Пример 3. Владельцы групп в качестве рецензентов
```http
"reviewers": [
    {
        "query": "./owners",
        "queryType": "MicrosoftGraph"
    }
]
```

Назначение только владельцев групп из определенной страны в качестве рецензентов:

```http
"reviewers": [
    {
        "query": "/groups/{group id}/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq 'USA'",
        "type": "MicrosoftGraph”
    }
]
```

### <a name="example-4-people-managers-as-reviewers"></a>Пример 4. Менеджеры людей в качестве рецензентов

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```
Поскольку `./manager` это относительный запрос, укажите **свойство queryRoot** со значением `decisions` .

## <a name="see-also"></a>См. также

+ [Настройка области определения обзора доступа](/graph/accessreviews-scope-concept)
