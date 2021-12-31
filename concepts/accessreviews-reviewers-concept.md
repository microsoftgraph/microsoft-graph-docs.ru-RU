---
title: Назначение рецензентов для проверки доступа с помощью API Graph Microsoft
description: Узнайте, как использовать API обзоров доступа в Microsoft Graph для назначения рецензентов доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 59acd960b0c3234262db05e05066bcef7ce98709
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651297"
---
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a>Назначение рецензентов для проверки доступа с помощью API Graph Microsoft

API обзоров доступа Azure [AD](/graph/api/resources/accessreviewsv2-overview) позволяет программным образом просмотреть доступ пользователей, директоров служб или групп к ресурсам Azure AD.

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

### <a name="example-5-application-owners-as-reviewers"></a>Пример 5. Владельцы приложений в качестве рецензентов

```http
"reviewers": [
    {
        "query": "/servicePrincipals/{id}/owners",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="next-steps"></a>Дальнейшие действия

+ [Настройка области определения обзора доступа](/graph/accessreviews-scope-concept)
+ [Узнайте, как](/graph/accessreviews-overview) использовать API обзоров доступа для проверки доступа к ресурсам Azure AD.