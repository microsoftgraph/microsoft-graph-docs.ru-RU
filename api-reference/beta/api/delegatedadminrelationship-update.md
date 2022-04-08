---
title: Обновление delegatedAdminRelationship
description: Обновление свойств объекта delegatedAdminRelationship.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: a248385d5ff066bf03306bf49eaca40203b15969
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704277"
---
# <a name="update-delegatedadminrelationship"></a>Обновление delegatedAdminRelationship
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [delegatedAdminRelationship](../resources/delegatedadminrelationship.md) . Связь может быть обновлена только в том случае, если она **в состоянии.**`created`

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
PATCH /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|If-Match|If-match: {etag}. Последнее известное значение ETag для **обновляемого объекта delegatedAdminRelationship** . Получение значения ETag из операции LIST или GET. Обязательно.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|accessDetails|[microsoft.graph.delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Идентификаторы административных ролей, к которые партнер запрашивает или имеет доступ в клиенте клиента.|
|Клиентов|[microsoft.graph.delegatedAdminRelationshipCustomerParticipant](../resources/delegatedadminrelationshipcustomerparticipant.md)|Отображаемое имя и уникальный идентификатор клиента связи.|
|displayName|String|Отображаемое имя связи, используемой для упрощения идентификации. Должен быть уникальным для *всех делегированных* отношений администратора партнера.|
|duration|Длительность|Длительность связи в формате ISO 8601. Должно быть значением между инклюзивным `P1D` `P2Y` .|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и обновленный объект [delegatedAdminRelationship](../resources/delegatedadminrelationship.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_delegatedadminrelationship"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836
If-Match: W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw=="
Content-Type: application/json

{
  "displayName": "Updated Contoso admin relationship",
  "duration": "P31D",
  "customer": {
    "tenantId": "52eaad04-13a2-4a2f-9ce8-93a294fadf36"
  },
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "44367163-eba1-44c3-98af-f5787879f96a"
      },
      {
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
      },
      {
        "roleDefinitionId": "69091246-20e8-4a56-aa4d-066075b2a7a8"
      },
      {
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
      }
    ]
  }
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminRelationship"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminRelationships/$entity",
  "@odata.etag": "W/\"JyIwMzAwZTM0ZS0wMDAwLTAyMDAtMDAwMC02MTRjZjI1YzAwMDAiJw==\"",
  "id": "5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836",
  "displayName": "Updated Contoso admin relationship",
  "duration": "P31D",
  "status": "created",
  "createdDateTime": "2022-02-10T11:24:42.3148266Z",
  "lastModifiedDateTime": "2022-02-10T11:26:44.9941884Z",
  "customer": {
    "tenantId": "52eaad04-13a2-4a2f-9ce8-93a294fadf36"
  },
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "44367163-eba1-44c3-98af-f5787879f96a"
      },
      {
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
      },
      {
        "roleDefinitionId": "69091246-20e8-4a56-aa4d-066075b2a7a8"
      },
      {
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
      }
    ]
  }
}
```

