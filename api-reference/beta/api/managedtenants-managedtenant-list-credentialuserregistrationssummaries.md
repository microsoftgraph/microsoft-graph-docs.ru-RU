---
title: Список credentialUserRegistrationsSummaries
description: Получите список объектов credentialUserRegistrationsSummary и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: fcb42f7c00a518e270d4e937156e1e6f39b4b692
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402436"
---
# <a name="list-credentialuserregistrationssummaries"></a>Список credentialUserRegistrationsSummaries
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Reports.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
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

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_credentialuserregistrationssummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.credentialUserRegistrationsSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#credentialUserRegistrationsSummaries",
  "value": [
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "mfaAndSsprCapableUserCount": 2,
      "ssprEnabledUserCount": 9,
      "mfaRegisteredUserCount": 3,
      "ssprRegisteredUserCount": 2,
      "totalUserCount": 9,
      "securityDefaultsEnabled": false,
      "mfaConditionalAccessPolicyState": "enabled",
      "lastRefreshedDateTime": "2021-07-11T09:58:11.5730661Z",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    },
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "mfaAndSsprCapableUserCount": 0,
      "ssprEnabledUserCount": 1,
      "mfaRegisteredUserCount": 0,
      "ssprRegisteredUserCount": 0,
      "totalUserCount": 7,
      "securityDefaultsEnabled": false,
      "mfaConditionalAccessPolicyState": "enabledForReportingButNotEnforced",
      "lastRefreshedDateTime": "2021-07-11T11:15:52.9375367Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    }
  ]
}
```
