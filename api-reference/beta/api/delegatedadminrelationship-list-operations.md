---
title: Операции со списком
description: Получите список объектов делегированияAdminRelationshipOperation и их свойств.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8493c222acea2fe481da3fc43c613301a87f9dfb
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589907"
---
# <a name="list-operations"></a>Операции со списком
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [делегированияAdminRelationshipOperation и](../resources/delegatedadminrelationshipoperation.md) их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| DelegatedAdminRelationship.Read.All, DelegatedAdminRelationship.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Для приложений| Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/operations
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры `$expand`запросов , `$select`, `$filter`, , `$top`и `$skipToken``$count`[OData](/graph/query-parameters), чтобы помочь настроить ответ.  

`$top` поддерживает до 300 объектов.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной `200 OK` работы этот метод возвращает код ответа и коллекцию объектов [делегированияAdminRelationshipOperation в](../resources/delegatedadminrelationshipoperation.md) тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_delegatedadminrelationshipoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/operations
```

### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedAdminRelationshipOperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#operations",
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedAdminRelationshipOperation",
      "@odata.etag": "W/\"JyIwMzAwZTM0ZS0wMDAwLTAyMDAtMDAwMC02MTRjZjI1YzAwMDAiJw==\"",
      "id": "e7de9158-df46-478e-820c-d6eff099d27b",
      "operationType": "delegatedAdminAccessAssignmentUpdate",
      "data": "{\"id\":\"a97a9b4c-f43e-4c47-bbd6-50d8d3c88d94\",\"accessContainer\":{\"accessContainerId\":\"11cc3849-c298-455f-9a11-b7be350ef352\",\"accessContainerType\":\"securityGroup\"},\"accessDetails\":{\"unifiedRoles\":[{\"roleDefinitionId\":\"f2ef992c-3afb-46b9-b7cf-a126ee74c451\"},{\"roleDefinitionId\":\"62e90394-69f5-4237-9190-012177145e10\"}]},\"status\":\"active\"}",
      "status": "complete",
      "createdDateTime": "2022-02-09T22:17:43.9821847Z",
      "lastModifiedDateTime": "2022-02-09T22:17:43.9821847Z"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminRelationshipOperation",
      "@odata.etag": "W/\"JyIwMzAwZTM0ZS0wMKMh5TAyMDAtMDAwMC02MTRjZjI1YzAwMDAiJw==\"",
      "id": "f7a7dad4-8cc4-40d7-be44-dd3501b1f4e0",
      "operationType": "delegatedAdminAccessAssignmentUpdate",
      "data": "{\"id\":\"a97a9b4c-f43e-4c47-bbd6-50d8d3c88d94\",\"accessContainer\":{\"accessContainerId\":\"8d56bce3-440f-4b4f-b5c2-cc0bcbd0199c\",\"accessContainerType\":\"securityGroup\"},\"accessDetails\":{\"unifiedRoles\":[{\"roleDefinitionId\":\"29232cdf-9323-42fd-ade2-1d097af3e4de\"},{\"roleDefinitionId\":\"88d8e3e3-8f55-4a1e-953a-9b9898b8876b\"}]},\"status\":\"active\"}",
      "status": "complete",
      "createdDateTime": "2022-02-11T20:32:05.4659288Z",
      "lastModifiedDateTime": "2022-02-11T20:34:42.9202474Z"
    }
  ]
}
```

