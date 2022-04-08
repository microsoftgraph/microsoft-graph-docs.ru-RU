---
title: Перечисление delegatedAdminCustomers
description: Получение списка объектов delegatedAdminCustomer и их свойств.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 8d3e20b6f46ddf548f706c93680ac7d6b5b3b6ed
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704462"
---
# <a name="list-delegatedadmincustomers"></a>Перечисление delegatedAdminCustomers
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [delegatedAdminCustomer](../resources/delegatedadmincustomer.md) и их свойств.

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
GET /tenantRelationships/delegatedAdminCustomers
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры `$select`запроса , `$filter`, `$top`, `$orderBy`, `$count`и `$skipToken`  [OData](/graph/query-parameters) , чтобы помочь настроить ответ.

`$top` поддерживает до 300 объектов.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [delegatedAdminCustomer](../resources/delegatedadmincustomer.md) в теле отклика.

**Каждый объект delegatedAdminCustomer** **содержит свойство @odata.etag** согласно RFC2616.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_delegatedadmincustomer"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminCustomers
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedAdminCustomer)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminCustomers",
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedAdminCustomer",
      "@odata.etag": "W/\"JyIxODAwMTMzZi0wMDAwLTAyMDAtMDAwMC02MTNjMGFhZTAwMDAiJw==\"",
      "id": "4fdbff88-9d6b-42e0-9713-45c922ba8001",
      "tenantId": "4fdbff88-9d6b-42e0-9713-45c922ba8001",
      "displayName": "Contoso Inc"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminCustomer",
      "@odata.etag": "W/\"JyIwMDAwMTEwMS0wMDAwLTAyMDAtMDAwMC02MDI1OTQyMjAwMDAiJw==\"",
      "id": "1c0fa218-5dec-49db-8247-cfa457af8116",
      "tenantId": "1c0fa218-5dec-49db-8247-cfa457af8116",
      "displayName": "Contoso subsidiary Inc"
    }
  ]
}
```

