---
title: Назначение рецензентов определению обзора доступа с помощью API Graph Microsoft
description: Узнайте, как использовать API обзоров доступа в Microsoft Graph для назначения рецензентов доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: f892e74f5bf7a7aa934872186208e21ede19780a
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579870"
---
# <a name="assign-reviewers-to-your-access-review-definition-using-the-microsoft-graph-api"></a>Назначение рецензентов определению обзора доступа с помощью API Graph Microsoft

API обзоров доступа Azure [AD](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) позволяет программным образом просмотреть доступ пользователей, директоров служб или групп к ресурсам Azure AD.

> [!NOTE]
> API [обзоров доступа](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) в настоящее время доступен только в конечной точке Graph Microsoft. Не используйте его в производственных приложениях, так как оно может изменяться без уведомления.

Основные рецензенты настроены в свойстве **рецензентов** ресурса [accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true)  Кроме того, вы можете указать рецензенты откатов с помощью **свойства fallbackReviewers.** Эти свойства не требуются при создании самообзора (когда пользователи просматривают собственный доступ).

## <a name="configure-reviewers"></a>Настройка рецензентов

Чтобы настроить рецензентов и рецензентов, задайте значения **запросов,** **queryRoot** и **queryType** свойств **accessReviewReviewerScope**. Описание этих свойств см. в виде [ресурса accessReviewReviewerScope.](/graph/api/resources/accessreviewreviewerscope?view=graph-rest-beta&preserve-view=true)

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
