---
title: Управление спискамиActions
description: Получите список объектов managementAction и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 03aedec0464908bf25deb004e6cbe4bdb5027acb
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402435"
---
# <a name="list-managementactions"></a>Управление спискамиActions
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [managementAction](../resources/managedtenants-managementaction.md) и их свойств.

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
GET /tenantRelationships/managedTenants/managementActions
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

В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов managementAction](../resources/managedtenants-managementaction.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_managementaction"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementAction)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActions",
    "value": [
        {
            "id": "4274db74-99c4-40be-bbeb-da4351136be2",
            "referenceTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
            "displayName": "Baseline - Require MFA for end users",
            "description": null,
            "category": "identity",
            "workloadActions": [
                {
                    "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                    "category": "automated",
                    "displayName": "ConditionalAccessPolicy",
                    "description": null,
                    "service": "AAD",
                    "settings": [
                        {
                            "valueType": "string",
                            "displayName": "DisplayName",
                            "overwriteAllowed": false,
                            "jsonValue": "\"Baseline - Require MFA for end users\""
                        },
                        {
                            "valueType": "string",
                            "displayName": "State",
                            "overwriteAllowed": false,
                            "jsonValue": "\"enabledForReportingButNotEnforced\""
                        },
                        {
                            "valueType": "stringCollection",
                            "displayName": "ClientAppTypes",
                            "overwriteAllowed": false,
                            "jsonValue": "[\"All\"]"
                        },
                        {
                            "valueType": "stringCollection",
                            "displayName": "IncludeApplications",
                            "overwriteAllowed": false,
                            "jsonValue": "[\"All\"]"
                        },
                        {
                            "valueType": "stringCollection",
                            "displayName": "IncludeUsers",
                            "overwriteAllowed": false,
                            "jsonValue": "[\"None\"]"
                        },
                        {
                            "valueType": "stringCollection",
                            "displayName": "IncludeLocations",
                            "overwriteAllowed": false,
                            "jsonValue": "[\"All\"]"
                        },
                        {
                            "valueType": "string",
                            "displayName": "GrantControls.Operator",
                            "overwriteAllowed": false,
                            "jsonValue": "\"OR\""
                        },
                        {
                            "valueType": "stringCollection",
                            "displayName": "GrantControls.BuiltInControls",
                            "overwriteAllowed": false,
                            "jsonValue": "[\"mfa\"]"
                        }
                    ]
                }
            ]
        }
    ]
}
```
