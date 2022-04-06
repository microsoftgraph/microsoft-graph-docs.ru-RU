---
title: Назначение рецензентов для проверки доступа с помощью microsoft API Graph
description: Узнайте, как использовать API обзоров доступа в Microsoft Graph для назначения рецензентов доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 099419f3c1998b94f1c57d983b8d25af0b653faf
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510655"
---
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a>Назначение рецензентов для проверки доступа с помощью microsoft API Graph

API обзоров доступа Azure [AD позволяет](/graph/api/resources/accessreviewsv2-overview) программным образом просмотреть доступ пользователей, директоров служб или групп к ресурсам Azure AD.

Основные рецензенты настроены в свойстве **рецензентов** ресурса [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) .  Кроме того, вы можете указать рецензенты откатов с помощью **свойства fallbackReviewers** . Эти свойства не требуются при создании самообзора (когда пользователи просматривают собственный доступ).

## <a name="configure-reviewers"></a>Настройка рецензентов

Чтобы настроить рецензентов и рецензентов, задайте значения свойств query **,** **queryRoot** и **queryType** **accessReviewReviewerScope**. Описание этих свойств см. в виде [ресурса accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope) .

### <a name="example-1-a-self-review"></a>Пример 1. Самообсвятие

```http
"reviewers": []
```

Чтобы настроить самообнавержение, не укажите свойство **рецензентов** или не покажите пустой объект свойству.

Если соответствующая область обзора  доступа нацелена на прямое подключение пользователей и групп B2B с общими каналами, владельцу группы будет назначено просмотреть доступ для пользователей прямого подключения B2B.

### <a name="example-2-a-specific-user-as-the-reviewer"></a>Пример 2. Конкретный пользователь в качестве рецензента

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-3-members-of-a-group-as-reviewers"></a>Пример 3. Члены группы в качестве рецензентов

```http
"reviewers": [
    {
        "query": "/groups/{group id}}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-4-group-owners-as-reviewers"></a>Пример 4. Владельцы групп в качестве рецензентов
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

### <a name="example-5-people-managers-as-reviewers"></a>Пример 5. Менеджеры людей в качестве рецензентов

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```

Поскольку `./manager` это относительный запрос, укажите **свойство queryRoot** со значением `decisions`.

Если соответствующая область обзора  доступа нацелена на прямое подключение пользователей и групп B2B с общими каналами, владельцу группы будет назначено просмотреть доступ для пользователей прямого подключения B2B.

### <a name="example-6-application-owners-as-reviewers"></a>Пример 6. Владельцы приложений в качестве рецензентов

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
+ [Создание обзора доступа](/azure/active-directory/governance/create-access-review)