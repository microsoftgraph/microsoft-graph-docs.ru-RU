---
title: Перечисление serviceManagementDetails
description: Получение списка объектов delegatedAdminServiceManagementDetail и их свойств.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 42fbe45443ffbdbe19a80ee457c69e0eabf49328
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202448"
---
# <a name="list-servicemanagementdetails"></a>Перечисление serviceManagementDetails
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [delegatedAdminServiceManagementDetail](../resources/delegatedAdminServiceManagementDetail.md) и их свойств.

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
GET /tenantRelationships/delegatedAdminCustomers/{delegatedAdminCustomerId}/serviceManagementDetails
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод не поддерживает параметры запроса OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters). 

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения `200 OK` этот метод возвращает код отклика и коллекцию объектов [delegatedAdminServiceManagementDetail](../resources/delegatedAdminServiceManagementDetail.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_delegatedAdminServiceManagementDetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminCustomers/4fdbff88-9d6b-42e0-9713-45c922ba8001/serviceManagementDetails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-delegatedadminservicemanagementdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-delegatedadminservicemanagementdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-delegatedadminservicemanagementdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-delegatedadminservicemanagementdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-delegatedadminservicemanagementdetails-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedAdminServiceManagementDetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminCustomers/4fdbff88-9d6b-42e0-9713-45c922ba8001/serviceManagementDetails",
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedAdminServiceManagementDetail",
      "id": "fa5fa04e-13df-4b7c-9e99-92573ba1fa55",
      "serviceManagementUrl": "https://aad.portal.azure.com/contoso.onmicrosoft.com",
      "serviceName": "Azure Active Directory"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminServiceManagementDetail",
      "id": "5d0273c3-0f0e-4e00-90e8-e792c8860fb5",
      "serviceManagementUrl": "https://lighthouse.microsoft.com",
      "serviceName": "Microsoft 365 Lighthouse"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminServiceManagementDetail",
      "id": "2b565abc-b0de-4974-97c0-bed0abb14a0f",
      "serviceManagementUrl": "https://businesscentral.dynamics.com/55beae45-27a6-4e7a-8c7c-2eae70816cfa/admin",
      "serviceName": "Dynamics 365 Business Central"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminServiceManagementDetail",
      "id": "ce0b42f4-bfde-4abe-a5f7-add83f104b23",
      "serviceManagementUrl": "https://admin.teams.microsoft.com/?delegatedOrg=contoso.onmicrosoft.com",
      "serviceName": "Teams"
    }
  ]
}
```

