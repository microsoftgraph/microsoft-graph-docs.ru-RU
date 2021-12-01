---
title: Списки подключенныхОрганизацией
description: Извлечение списка объектов connectedOrganization.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0e2be6b037e70a4b3c5b1f588583cbd1e020713f
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242973"
---
# <a name="list-connectedorganizations"></a>Списки подключенныхОрганизацией

Пространство имен: microsoft.graph


Извлечение списка [объектов connectedOrganization.](../resources/connectedorganization.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
| Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="optional-query-parameters"></a>Необязательные параметры запроса
Этот метод поддерживает параметры `$select` `$filter` запроса oData и OData для настройки ответа. Например, чтобы получить только подключенные организации с определенным именем отображения, добавьте `$filter=displayName eq 'Name'` . Аналогичным образом, чтобы получить только подключенные организации с источником удостоверений определенного клиента, добавьте `$filter=identitySources/any(is:is/microsoft.graph.azureActiveDirectoryTenant/tenantId eq '72f988bf-86f1-41af-91ab-2d7cd011db47')` . Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов connectedOrganization](../resources/connectedorganization.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "list_connectedorganization"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/connectedOrganizations
```

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.connectedOrganization)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "04e7fa5f-fa5f-04e7-5ffa-e7045ffae704",
      "displayName": "Wingtip Toys",
      "description": "Wingtip Toys",
      "createdDateTime": "2020-05-13T15:18:04.81Z",
      "modifiedDateTime": "2020-05-13T15:18:04.81Z",
      "identitySources": [
        {
          "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
          "displayName": "Wingtip Toys Co"
        }
      ],
      "state": "configured"
    }
  ]
}
```

