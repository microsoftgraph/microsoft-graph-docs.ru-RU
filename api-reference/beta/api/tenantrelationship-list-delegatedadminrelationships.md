---
title: Список делегированAdminRelationships
description: Получите список объектов делегированияAdminRelationship и их свойств.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0d3d2b3b78a8f2c72ed025dbe866031f2919f4e1
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64590032"
---
# <a name="list-delegatedadminrelationships"></a>Список делегированAdminRelationships
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [делегированияAdminRelationship](../resources/delegatedadminrelationship.md) и их свойств.

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
GET /tenantRelationships/delegatedAdminRelationships
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры `$select`запросов , `$filter`, `$top`, , `$orderBy`и `$skipToken``$count`[OData](/graph/query-parameters), чтобы помочь настроить ответ.  

`$top` поддерживает до 300 объектов.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной `200 OK` работы этот метод возвращает код ответа и коллекцию объектов [делегированияAdminRelationship](../resources/delegatedadminrelationship.md) в тексте ответа.

**Каждый объект делегированияAdminRelationship** **содержит свойство @odata.etag** по RFC2616.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_delegatedadminrelationship"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedAdminRelationship)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminRelationships",
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
      "@odata.etag": "W/\"JyIwMzAwZTM0ZS0wMDAwLTAyMDAtMDAwMC02MTRjZjI1YzAwMDAiJw==\"",
      "id": "5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836",
      "displayName": "Contoso admin relationship",
      "duration": "P730D",
      "customer": {
        "tenantId": "52eaad04-13a2-4a2f-9ce8-93a294fadf36",
        "displayName": "Contoso Inc"
      },
      "accessDetails": {
        "unifiedRoles": [
          {
            "roleDefinitionId": "dd4db9a0-cc4a-4213-9f9f-70242232d97e"
          }
        ]
      },
      "status": "active",
      "createdDateTime": "2022-02-10T11:24:42.3148266Z",
      "lastModifiedDateTime": "2022-02-10T11:26:44.9941884Z",
      "activatedDateTime": "2022-02-10T11:26:44.9941884Z",
      "endDateTime": "2024-02-10T11:24:42.3148266Z"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
      "@odata.etag": "W/\"JyIwMzAwZTM0ZS0wKklILTAyMDAtMDAwMC02MTRjZjI1YzAwMDAiJw==\"",
      "id": "1041ef52-a99b-4245-a3be-cbd3fa7c5ed1-8777b240-c6f0-4469-9e98-a3205431b836",
      "displayName": "Contoso subsidiary relationship",
      "duration": "P30D",
      "customer": {
        "tenantId": "4b827261-d21f-4aa9-b7db-7fa1f56fb163",
        "displayName": "Contoso subsidiary Inc"
      },
      "accessDetails": {
        "unifiedRoles": [
          {
            "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
          },
          {
            "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
          }
        ]
      },
      "status": "terminated",
      "createdDateTime": "2021-09-29T16:52:39.6133896Z",
      "lastModifiedDateTime": "2021-10-29T16:57:20.2101088Z",
      "activatedDateTime": "2021-09-29T16:55:20.2101088Z",
      "endDateTime": "2021-10-29T16:57:20.2101088Z"
    }
  ]
}
```

