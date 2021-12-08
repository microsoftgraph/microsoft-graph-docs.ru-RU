---
title: Списки accessPackageAssignments
description: Извлечение списка объектов accesspackageassignment.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2304102961ce44f1bab74796394b8887803a985f
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346619"
---
# <a name="list-assignments"></a>Перечисление заданий

Пространство имен: microsoft.graph

В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)извлекайте список [объектов accessPackageAssignment.](../resources/accesspackageassignment.md)

Для администраторов, доступных по каталогам, в итоговом списке содержатся все назначения, текущие и просроченные, которые вызываемая имеет доступ к считывке во всех каталогах и пакетах доступа.  Если звонивший от имени делегирования пользователя, которому назначены только делегированная административная роль в каталоге, запрос должен предоставить фильтр, чтобы указать определенный пакет доступа, например: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` .


## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/assignments
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры `$select` `$filter` запроса OData и OData для настройки `$expand` ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

### <a name="example-scenarios-for-using-query-parameters"></a>Примеры сценариев использования параметров запроса

- Если звонивший от имени делегирования пользователя, которому назначены только делегированная административная роль в каталоге, запрос должен предоставить фильтр, чтобы указать определенный пакет доступа, например: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` .
- Чтобы вернуть целевой объект и пакет доступа, включай `$expand=target,accessPackage` .
- Чтобы получить только доставленные назначения, можно включить запрос `$filter=assignmentState eq 'Delivered'` .
- Чтобы получить только назначения для конкретного пользователя, можно включить запрос с назначениями, нацеленными на объект ID этого пользователя: `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` .
- Чтобы получить только назначения для конкретного пользователя и определенного пакета доступа, можно включить запрос с назначениями, нацеленными на этот пакет доступа, и ID объекта этого пользователя: `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` .


## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [accessPackageAssignment](../resources/accesspackageassignment.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageassignment"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignments
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accesspackageassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "2a353749-3749-2a35-4937-352a4937352a",
      "state": "delivered",
      "status": "Delivered",
      "expiredDateTime": "2019-04-25T23:45:40.42Z",
      "schedule": {
        "@odata.type": "microsoft.graph.entitlementManagementSchedule"
      }
    }
  ]
}
```



