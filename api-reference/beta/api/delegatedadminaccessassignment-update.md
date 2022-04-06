---
title: Обновление делегированияAdminAccessAssignment
description: Обновление свойств объекта делегированияAdminAccessAssignment.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 52bee21df148af0bd02bb6a72d52d7c24db3c75f
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589883"
---
# <a name="update-delegatedadminaccessassignment"></a>Обновление делегированияAdminAccessAssignment
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [делегированияAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| DelegatedAdminRelationship.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Для приложений| Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/accessAssignments/{delegatedAdminAccessAssignmentId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|If-Match|If-match: etag}. Последнее известное значение ETag для **делегированияAdminAccessAssignment** , который необходимо обновить. Обязательно.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|Свойство|Тип|Описание|
|:---|:---|:---|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Идентификаторы административных ролей, которые партнеру назначены в клиенте клиента|


## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` `202 Accepted` ответа или код ответа.

## <a name="response-headers"></a>Заголовки откликов
|Имя|Описание|
|:---|:---|
|Content-Type|application/json.|
|Расположение|Расположение длительной операции.|
|Retry-After|Время, после которого можно сделать следующий вызов API в URL-адрес Location, чтобы проверить состояние длительной операции.|

Этот метод обычно возвращает код `202 Accepted` ответа с URL-адресом для длительной операции в загонах  ответов Location, которые можно отслеживать для завершения. Если значения, указанные в вызове, идентичны значениям существующего объекта, API `200 OK` возвращает код ответа с исходным делегированным [объектомAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_delegatedadminaccessassignment",
  "@odata.type": "microsoft.graph.delegatedAdminAccessAssignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5e5594d3-6f82-458b-b567-77db4811f0cd-00000000-0000-0000-0000-000000001234/accessAssignments/da9d6cf90-083a-47dc-ace2-1da98be3f344
If-Match: W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw=="
Content-Type: application/json

{
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
      },
      {
        "roleDefinitionId": "44367163-eba1-44c3-98af-f5787879f96a"
      },
      {
        "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
      }
    ]
  }
}
```

### <a name="response"></a>Отклик
Ниже приводится пример ответа, который возвращает `202 Accepted` код ответа вместе с заглавными заглавами **Location** и **Retry-After** .
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminAccessAssignment"
}
-->
``` http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5e5594d3-6f82-458b-b567-77db4811f0cd-00000000-0000-0000-0000-000000001234/operations/d8dbb27b-7fe7-4523-a3df-f766355fe0f2
Retry-After: 10
Content-Type: application/json

{
}
```