---
title: Обновление delegatedAdminAccessAssignment
description: Обновление свойств объекта delegatedAdminAccessAssignment.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 7c0a6e045d64aba40c2db8a323afab273ee7f517
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704291"
---
# <a name="update-delegatedadminaccessassignment"></a>Обновление delegatedAdminAccessAssignment
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) .

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
|If-Match|If-match: etag}. Последнее известное значение ETag для **обновляемого объекта delegatedAdminAccessAssignment** . Обязательно.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|Свойство|Тип|Описание|
|:---|:---|:---|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Идентификаторы административных ролей, назначенных партнеру в клиенте клиента.|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` ответа `202 Accepted` или код ответа.

## <a name="response-headers"></a>Заголовки откликов
|Имя|Описание|
|:---|:---|
|Content-Type|application/json.|
|Location|Расположение длительной операции.|
|Retry-After|Время, по истечении которого можно выполнить последующий вызов API к URL-адресу расположения для проверки состояния длительной операции.|

Этот метод обычно возвращает `202 Accepted` код отклика с URL-адресом длительной операции в заголовке ответа **Location** , который можно отслеживать для завершения. Если значения, указанные в вызове, идентичны значениям в существующем объекте, API `200 OK` возвращает код ответа с исходным [объектом delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) в теле отклика.

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
Ниже приведен пример ответа, который возвращает `202 Accepted` код ответа вместе с заголовками **Location** и **Retry-After** .
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