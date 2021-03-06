---
title: Создание plannerRosterMember
description: Создание объекта plannerRosterMember.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: e7dac57941d50ee8b543c53982c216c4c19d5d07
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272443"
---
# <a name="create-plannerrostermember"></a>Создание plannerRosterMember
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавьте член в объект [plannerRoster.](../resources/plannerrostermember.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Tasks.ReadWrite|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /planner/rosters/{plannerRosterId}/members
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса укажу представление объекта [plannerRosterMember](../resources/plannerrostermember.md) в JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта plannerRosterMember.](../resources/plannerrostermember.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|Идентификатор .|
|tenantId|String|Идентификатор клиента, к котором принадлежит пользователь. Необязательный параметр. В настоящее время участники группы не могут быть из разных клиентов.|
|roles|Набор строк|Дополнительные роли, назначенные пользователю. Необязательный параметр. В настоящее время для пользователей не доступны дополнительные роли.|



## <a name="response"></a>Ответ

В случае успеха этот метод возвращает код отклика и объект `201 Created` [plannerRosterMember](../resources/plannerrostermember.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerrostermember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members
Content-Type: application/json
Content-length: 78

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "userId": "String"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerrostermember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerrostermember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerrostermember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerrostermember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRosterMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "id": "670095cd-95cd-6700-cd95-0067cd950067",
  "userId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
  "roles": [
  ]
}
```

