---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
ms.openlocfilehash: 674a69f5697f5abf6e654ea71419bdfdfd660343
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859115"
---
# <a name="create-governanceroleassignmentrequest"></a>Создание governanceRoleAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.

| Operation                                   | Тип        |
|:--------------------------------------------|:------------|
| Назначение роли                    | Админадд    |
| Активация подходящего назначения роли        | Усерадд     |
| Деактивация активированного назначения роли     | Усерремове  |
| Удаление назначения роли                    | Админремове |
| Обновление назначения роли                    | Админупдате |
| Запрос на расширение назначения роли        | Усерекстенд  |
| Расширение назначения роли                    | Админекстенд |
| Запрос на продление назначения роли с истекшим сроком действия | Усерренев   |
| Продление назначенной роли с истекшим сроком действия            | Админренев  |

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения                               |
|:---------------------------------------|:------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Привилежедакцесс. ReadWrite. Азурересаурцес |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                            |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание      |
|:--------------|:-----------------|
| Авторизация | Bearer {code}    |
| Content-Type  | application/json |

## <a name="request-body"></a>Тело запроса

В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.

| Свойство         | Тип                                                     | Описание |
|:-----------------|:---------------------------------------------------------|:--|
| resourceId       | String                                                   | Идентификатор ресурса. Обязательно. |
| Роледефинитионид | String                                                   | Идентификатор определения роли. Обязательно. |
| Субжектид        | String                                                   | ИДЕНТИФИКАТОР субъекта. Обязательно. |
| Ассигнментстате  | String                                                   | Состояние назначения. Значение может быть `Eligible` и `Active`. Обязательное. |
| type             | String                                                   | Тип запроса. Возможные значения: `AdminAdd`, `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `AdminRenew` `AdminExtend`,,,,, и. `UserExtend` `UserRenew` Обязательно. |
| причиной           | String                                                   | Необходимо указать причину для запроса на назначение роли для аудита и проверки. |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | Расписание запроса на назначение роли. `UserAdd`Для типа запроса `AdminAdd`,, `AdminUpdate`, и `AdminExtend`, он необходим. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.

### <a name="error-codes"></a>Коды ошибок

Этот API возвращает стандартные коды ошибок HTTP. Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.

| Код ошибки     | Сообщение об ошибке                               | Сведения       |
|:---------------|:--------------------------------------------|:--------------|
| 400 Бадрекуест | Роленотфаунд                                | Не `roleDefinitionId` удается найти указанный в тексте запроса. |
| 400 Бадрекуест | Ресаурцеислоккед                            | Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей. |
| 400 Бадрекуест | Субжектнотфаунд                             | Не `subjectId` удается найти указанный в тексте запроса. |
| 400 Бадрекуест | Пендингролеассигнментрекуест                | В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) . |
| 400 Бадрекуест | Ролеассигнментексистс                        | [GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе. |
| 400 Бадрекуест | Ролеассигнментдоеснотексист                  | [GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе. |
| 400 Бадрекуест | Ролеассигнментрекуестполицивалидатионфаилед | [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан. |

## <a name="examples"></a>Примеры

В следующих примерах показано, как использовать этот API.

### <a name="example-1-administrator-assigns-user-to-a-role"></a>Пример 1: Администратор назначает пользователю роль

В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.

 >**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.

| Свойство         | Тип                                                     | Обязательный                 | Значение |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| resourceId       | String                                                   | Да                      | \<resourceId\> |
| Роледефинитионид | String                                                   | Да                      | \<Роледефинитионид\> |
| Субжектид        | String                                                   | Да                      | \<Субжектид\> |
| Ассигнментстате  | String                                                   | Да                      | Подходящие/активные |
| type             | String                                                   | Да                      | Админадд |
| причиной           | String                                                   | зависит от параметров роли |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | Да                      |   |

#### <a name="request"></a>Запрос


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Eligible",
  "type": "AdminAdd",
  "reason": "Assign an eligible role",
  "schedule": {
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "type": "Once"
  }
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "1232e4ea-741a-4be5-8044-5edabdd61672",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminAdd",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Evaluate Only",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-2-user-activates-eligible-role"></a>Пример 2: пользователь активирует подходящие роли

В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.

| Свойство         | Тип                                                     | Обязательный                 | Значение |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| resourceId       | String                                                   | Да                      | \<resourceId\> |
| Роледефинитионид | String                                                   | Да                      | \<Роледефинитионид\> |
| Субжектид        | String                                                   | Да                      | \<Субжектид\> |
| Ассигнментстате  | String                                                   | Да                      | Активное |
| type             | String                                                   | Да                      | Усерадд |
| причиной           | String                                                   | зависит от параметров роли |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | Да                      |   |

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserAdd",
  "reason": "Activate the owner role",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "duration": "PT9H"
  },
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394"
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "3ad49a7c-918e-4d86-9f84-fab28f8658c0",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394",
  "type": "UserAdd",
  "assignmentState": "Active",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Activate the owner role",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "EligibilityRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      },
      {
        "key": "JustificationRule",
        "value": "Grant"
      },
      {
        "key": "ActivationDayRule",
        "value": "Grant"
      },
      {
        "key": "ApprovalRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "endDateTime": "0001-01-01T00:00:00Z",
    "duration": "PT9H"
  }
}
```

### <a name="example-3-user-deactivates-an-assigned-role"></a>Пример 3: пользователь отключает назначенную роль

В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.

| Свойство         | Тип                                                     | Обязательный | Значение |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| resourceId       | String                                                   | Да      | \<resourceId\> |
| Роледефинитионид | String                                                   | Да      | \<Роледефинитионид\> |
| Субжектид        | String                                                   | Да      | \<Субжектид\> |
| Ассигнментстате  | Строка                                                   | Да      | Активное |
| type             | Строка                                                   | Да      | Усерремове |
| причиной           | String                                                   | Нет       |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | Нет       |   |

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserRemove",
  "reason": "Deactivate the role",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "abfcdb57-8e5d-42a0-ae67-7598b96fddb1",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec",
  "type": "UserRemove",
  "assignmentState": "Active",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Evaluate only",
  "schedule": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  }
}
```

### <a name="example-4-administrator-removes-user-from-a-role"></a>Пример 4: Администратор удаляет пользователя из роли

В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.

 >**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.

| Свойство         | Тип                                                     | Обязательный | Значение |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| resourceId       | String                                                   | Да      | \<resourceId\> |
| Роледефинитионид | Строка                                                   | Да      | \<Роледефинитионид\> |
| Субжектид        | Строка                                                   | Да      | \<Субжектид\> |
| Ассигнментстате  | Строка                                                   | Да      | Подходящие/активные |
| type             | Строка                                                   | Да      | Админремове |
| причиной           | String                                                   | Нет       |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | Нет       |   |

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminRemove"
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminRemove",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  },
  "schedule": null
}
```

### <a name="example-5-administrator-updates-role-assignment"></a>Пример 5: "Администратор обновляет назначение ролей"

В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.

 >**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.

| Свойство         | Тип                                                     | Обязательный                | Значение |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| resourceId       | String                                                   | Да                     | \<resourceId\> |
| Роледефинитионид | Строка                                                   | Да                     | \<Роледефинитионид\> |
| Субжектид        | Строка                                                   | Да                     | \<Субжектид\> |
| Ассигнментстате  | Строка                                                   | Да                     | Подходящие/активные |
| type             | Строка                                                   | Да                     | Админупдате |
| причиной           | String                                                   | зависит от Ролесеттингс |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | Да                     |   |

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState": "Eligible",
  "type": "AdminUpdate",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31.000Z"
  }
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminUpdate",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-6-administrator-extends-expiring-role-assignment"></a>Пример 6: администратор расширяет назначение ролей с истекшим сроком действия

В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.

 >**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.

| Свойство         | Тип                                                     | Обязательный                | Значение |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| resourceId       | String                                                   | Да                     | \<resourceId\> |
| Роледефинитионид | Строка                                                   | Да                     | \<Роледефинитионид\> |
| Субжектид        | String                                                   | Да                     | \<Субжектид\> |
| Ассигнментстате  | String                                                   | Да                     | Подходящие/активные |
| type             | String                                                   | Да                     | Админекстенд |
| причиной           | String                                                   | зависит от Ролесеттингс |   |
| schedule         | [governanceSchedule](../resources/governanceschedule.md) | Да                     |   |

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminExtend",
  "reason": "extend role assignment",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z"
  }
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminExtend",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "extend role assignment",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z",
    "duration": "PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
