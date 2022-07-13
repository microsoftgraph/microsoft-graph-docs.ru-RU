---
title: Назначение рецензентов для проверки доступа с помощью microsoft API Graph
description: Используйте API проверок доступа в Microsoft Graph, чтобы назначать рецензентов доступа, таких как определенные пользователи, участники или владельцы группы, менеджеры пользователей или владельцы приложений.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 72f5fd24e3949d9cb291e094006461c5c4e90b92
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768128"
---
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a>Назначение рецензентов для проверки доступа с помощью microsoft API Graph

API Azure AD доступа позволяет [](/graph/api/resources/accessreviewsv2-overview) программно проверить доступ пользователей, субъектов-служб или групп к Azure AD ресурсам.

Основные рецензенты настраиваются в свойстве **рецензентов** ресурса [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) .  Кроме того, можно указать резервных рецензентов с помощью свойства **fallbackReviewers** . Эти свойства не требуются при создании самостоятельной проверки (когда пользователи проверяют собственный доступ).

Чтобы настроить рецензентов и резервных рецензентов, задайте значения свойств **query**, **queryRoot** и **queryType** **accessReviewReviewerScope**. Описание этих свойств см. в описании типа ресурса [accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope) .

## <a name="example-1-a-self-review"></a>Пример 1. Самообслуживка

```http
"reviewers": []
```

Для настройки самостоятельной проверки не указывайте свойство рецензентов или не указывайте в свойстве пустой объект.

Если соответствующая область проверки доступа предназначена для пользователей и команд прямого подключения B2B с общими каналами, владельцу команды будет назначено проверить доступ для пользователей прямого подключения B2B.

## <a name="example-2-a-specific-user-as-the-reviewer"></a>Пример 2. Конкретный пользователь в качестве рецензента

```http
"reviewers": [
    {
        "query": "/users/{userId}",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="example-3-members-of-a-group-as-reviewers"></a>Пример 3. Члены группы в качестве рецензентов

```http
"reviewers": [
    {
        "query": "/groups/{groupId}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="example-4-group-owners-as-reviewers"></a>Пример 4. Владельцы групп в качестве рецензентов

Если проверка доступа предназначена для группы, например пример [1.](accessreviews-scope-concept.md#example-1-review-all-users-assigned-to-a-group) Просмотр всех пользователей, назначенных группе, пример [2.](accessreviews-scope-concept.md#example-2-review-all-guest-users-assigned-to-a-group) Просмотр всех гостевых пользователей, назначенных группе, и пример [3.](accessreviews-scope-concept.md#example-3-review-all-users-and-groups-assigned-to-a-group) Просмотр всех пользователей и групп, назначенных группе.
```http
"reviewers": [
    {
        "query": "/groups/{groupId}/owners",
        "queryType": "MicrosoftGraph"
    }
]
```

Если проверка доступа предназначена для группы и назначает в качестве рецензентов только владельцев групп из определенной страны:

```http
"reviewers": [
    {
        "query": "/groups/{groupId}/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq 'USA'",
        "type": "MicrosoftGraph”
    }
]
```

Если проверка доступа предназначена для всех групп, например пример 4. Просмотр всех пользователей, назначенных всем группам [Microsoft 365](accessreviews-scope-concept.md#example-4-review-all-users-assigned-to-all-microsoft-365-groups), пример 5. Просмотр всех гостевых пользователей, назначенных всем группам [Microsoft 365](accessreviews-scope-concept.md#example-5-review-all-guest-users-assigned-to-all-microsoft-365-groups), и пример 6. Просмотр всех гостевых пользователей, назначенных всем [командам](accessreviews-scope-concept.md#example-6-review-all-guest-users-assigned-to-all-teams).

```http
"reviewers": [
    {
        "query": "./owners",
        "queryType": "MicrosoftGraph"
    }
]
```



## <a name="example-5-people-managers-as-reviewers"></a>Пример 5. Руководители людей в качестве рецензентов

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```

Так `./manager` как это относительный запрос, укажите свойство **queryRoot** со значением `decisions`.

Если соответствующая область проверки доступа предназначена для пользователей и команд прямого подключения B2B с общими каналами, владельцу команды будет назначено проверить доступ для пользователей прямого подключения B2B.

## <a name="example-6-application-owners-as-reviewers"></a>Пример 6. Владельцы приложений в качестве рецензентов

```http
"reviewers": [
    {
        "query": "/servicePrincipals/{servicePrincipalId}/owners",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="next-steps"></a>Дальнейшие действия

+ [Настройка области определения проверки доступа](/graph/accessreviews-scope-concept)
+ [Ознакомьтесь с руководствами](/graph/accessreviews-overview), чтобы узнать, как использовать API проверки доступа для проверки доступа к Azure AD ресурсам.
+ [Создание проверки доступа](/azure/active-directory/governance/create-access-review)
