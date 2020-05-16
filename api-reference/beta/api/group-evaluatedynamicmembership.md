---
title: 'Группа: Евалуатединамикмембершип'
description: Оцените, является ли пользователь или устройство участником динамической группы.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b49f89da63b68f15329f7f700cc7699ff07e6208
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272856"
---
# <a name="group-evaluatedynamicmembership"></a>Группа: Евалуатединамикмембершип

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Оценка того, является ли пользователь или устройство участником динамической группы. Правило членства возвращается вместе с другими сведениями, использованными в ходе оценки. Эту операцию можно выполнить следующими способами: 

- Оценка того, является ли пользователь или устройство членом указанной динамической группы.  
- Оценка того, будет ли пользователь или устройство участником динамической группы на основе идентификатора пользователя или устройства и правила членства.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a>Оценка динамического членства с ИДЕНТИФИКАТОРом участника и ИДЕНТИФИКАТОРом группы

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| :-------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись) | Для пользователя: Group. Read. ALL и User. Read. ALL, Directory. Read. ALL<br>Для Device: Group. Read. ALL и Device. Read. ALL, Directory. Read. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a>Оценка динамического членства с ИДЕНТИФИКАТОРом участника и правилом членства

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| :-------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись) | Для пользователя: User. Read. ALL, Directory. Read. ALL<br>Для Device: Device. Read. ALL, Directory. Read. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
| :--- | :---------- |
| Authorization | Bearer {token} |
| Content-Type  | application/json |

## <a name="request-body"></a>Тело запроса

В тексте запроса укажите необходимые свойства.

В следующей таблице перечислены свойства, которые необходимы при оценке членства в группе.

| Параметр | Тип | Описание |
| :-------- | :--- | :---------- |
| Идентификатора | Коллекция объектов string | memberId это идентификатор объекта для оцениваемого пользователя или устройства. |
| membershipRule | Коллекция объектов string | Правило, используемое для оценки членства. Если это свойство не указано, оценивается правило для существующей группы. Если это свойство указано, то пользователь или устройство оцениваются для возможного членства в группе с тем же правилом. Дополнительные сведения см. [в статье динамическое правило членства для групп в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [евалуатединамикмембершипресулт](../resources/evaluatedynamicmembershipresult.md) .

## <a name="examples"></a>Примеры

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a>Пример 1: Оценка того, является ли пользователь или устройство участником существующей группы

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33"
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}

```

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a>Пример 2: Оценка того, будет ли пользователь или устройство участником группы на основе правила членства

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership"
}-->

```http
POST https://graph.microsoft.com/beta/groups/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33",
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")"
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: evaluateDynamicMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
