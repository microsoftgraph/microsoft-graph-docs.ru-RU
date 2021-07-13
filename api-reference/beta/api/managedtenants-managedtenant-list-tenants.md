---
title: Список клиентов
description: Получите список объектов клиента и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a837f1db5990322311c0718d47e888fafd64284e
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403088"
---
# <a name="list-tenants"></a>Список клиентов
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [клиента](../resources/managedtenants-tenant.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ManagedTenants.Read.All, ManagedTenants.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenants
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` клиента в тексте ответа. [](../resources/managedtenants-tenant.md)

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_tenant"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "contract": {
        "displayName": "Fourth Coffee",
        "defaultDomainName": "fourthcoffe01.onmicrosoft.com",
        "contractType": 2
      },
      "tenantStatusInformation": {
        "onboardingStatus": "ineligible",
        "onboardingDateTime": "2012-02-20T00:00:00Z",
        "onboardedByUserId": "",
        "offboardedDateTime": "2012-02-20T00:00:00Z",
        "offboardedBy": "",
        "delegatedPrivilegeStatus": "delegatedAdminPrivileges",
        "workloadStatuses": [
          {
            "displayName": "Device Management",
            "onboardingStatus": "onboarded",
            "onboardedDateTime": "2012-02-20T00:00:00Z",
            "offboardedDateTime": null
          },
          {
            "displayName": "Cloud PC",
            "onboardingStatus": "notOnboarded",
            "onboardedDateTime": "2012-02-20T00:00:00Z",
            "offboardedDateTime": null
          }
        ]
      },
      "createdDateTime": "2012-02-20T00:00:00Z",
      "lastUpdatedDatetime": "2021-02-20T00:00:00Z"
    }
  ]
}
```
