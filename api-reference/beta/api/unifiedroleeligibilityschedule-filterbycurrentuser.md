---
title: 'unifiedRoleEligibilitySchedule: filterByCurrentUser'
description: Получите список объектов unifiedRoleEligibilitySchedule и их свойств, отфильтрованных определенным пользователем
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7a95b6a3af83f6d9da4f6403505a355909ea47eb
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695925"
---
# <a name="unifiedroleeligibilityschedule-filterbycurrentuser"></a>unifiedRoleEligibilitySchedule: filterByCurrentUser
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [unifiedRoleEligibilitySchedule](../resources/unifiedRoleEligibilitySchedule.md) и их свойств, связанных с определенным основным объектом.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET roleManagement/directory/roleEligibilitySchedules/filterByCurrentUser(on='principal')
```

## <a name="function-parameters"></a>Параметры функции
В следующей таблице показаны параметры, которые можно использовать с помощью этого метода.

|Параметр|Тип|Описание|
|:---|:---|:---|
|on|roleEligibilityScheduleFilterByCurrentUserOptions|Пользователь, в настоящее время подписанный. Разрешено значение `principal` .|

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметр `$select` запроса OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) в теле ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedule_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilitySchedules/filterByCurrentUser(on='principal')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleeligibilityschedule-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleeligibilityschedule-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleeligibilityschedule-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleeligibilityschedule-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик

Ниже приводится пример ответа с указанием расписания приемлемости, определяемого групповым назначением.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilitySchedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(unifiedRoleEligibilitySchedule)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.unifiedRoleEligibilitySchedule",
            "id": "6938d75d-ad66-4c7d-9028-0c9b00296945",
            "principalId": "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
            "directoryScopeId": "/",
            "appScopeId": null,
            "createdUsing": "6938d75d-ad66-4c7d-9028-0c9b00296945",
            "createdDateTime": "2021-08-09T10:15:05.96Z",
            "modifiedDateTime": "0001-01-01T08:00:00Z",
            "status": "Provisioned",
            "memberType": "Direct",
            "scheduleInfo": {
                "startDateTime": "2021-08-09T10:15:05.96Z",
                "recurrence": null,
                "expiration": {
                    "type": "noExpiration",
                    "endDateTime": null,
                    "duration": null
                }
            }
        }
    ]
}
```

