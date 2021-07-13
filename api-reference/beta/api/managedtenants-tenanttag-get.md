---
title: Get tenantTag
description: Ознакомьтесь с свойствами и отношениями объекта tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 5094df9488292e521cbddfedd380a0846385f147
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403120"
---
# <a name="get-tenanttag"></a>Get tenantTag
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями объекта [tenantTag.](../resources/managedtenants-tenanttag.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ManagedTenants.Read.All, ManagedTenants.WriteRead.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_tenanttag"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantTags/$entity",
    "id": "913391c0-5466-42b4-900d-0a7501399cb0",
    "displayName": "Onboarding",
    "description": "Tenants that we are currently onboarding",
    "tenantIds": [
        "38227791-a88b-4fcc-81c5-58cf77668320",
        "34298981-4fc8-4974-9486-c8909ed1521b",
        "4d262a25-c70a-430b-9e8e-46c31dec116b"
    ],
    "isDeleted": null,
    "createdDateTime": "2021-06-16T20:36:31.086644Z",
    "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
    "lastActionDateTime": "2021-06-28T20:46:09.0071888Z",
    "lastActionByUserId": "08ea0285-30cb-46cc-abc8-3d8422e21ecb",
    "tenants": [
        {
            "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
        },
        {
            "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
        },
        {
            "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
        }
    ]
}
```
