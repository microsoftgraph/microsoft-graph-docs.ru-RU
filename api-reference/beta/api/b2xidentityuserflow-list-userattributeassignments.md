---
title: Список Усераттрибутеассигнментс
description: Получение ресурсов Идентитюсерфловаттрибутеассигнмент из свойства навигации Усераттрибутеассигнментс.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: db2c57500f266700d8dbf3669ed0d8d457c8a24d
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581339"
---
# <a name="list-userattributeassignments"></a>Список Усераттрибутеассигнментс

Пространство имен: microsoft.graph

Получение ресурсов Идентитюсерфловаттрибутеассигнмент из свойства навигации Усераттрибутеассигнментс в [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/userAttributeAssignments
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает `$select` Параметры и `$expand` для получения сведений об атрибуте пользовательского процесса. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-list-userattributeassignments-in-a-b2xidentityuserflow"></a>Пример 1: List Усераттрибутеассигнментс in a b2xIdentityUserFlow

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/userAttributeAssignments
```

#### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.identityUserFlowAttributeAssignment)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
    "value": [
        {
            "id": "City",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "RadioSingleSelect",
            "displayName": "City",
            "userAttributeValues": [
                {
                    "name": "S",
                    "value": "1",
                    "isDefault": true
                }
            ]
        },
        {
            "id": "extension_guid_shoeSize",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "TextBox",
            "displayName": "Shoe size",
            "userFlowId": "B2C_1_Consumer",
            "userAttributeValues": []
        }
    ]
}
```

### <a name="example-2-list-userattributeassignments-in-a-b2xidentityuserflow-and-expand-userattribute"></a>Пример 2: List Усераттрибутеассигнментс in a b2xIdentityUserFlow и Expand Усераттрибуте

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/userAttributeAssignments?$expand=userAttribute
```

#### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.identityUserFlowAttributeAssignment)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
    "value": [
        {
            "id": "City",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "RadioSingleSelect",
            "displayName": "City",
            "userAttributeValues": [
                {
                    "name": "S",
                    "value": "1",
                    "isDefault": true
                }
            ],
            "userAttribute": {
                "@odata.type": "#Microsoft.Graph.BuiltInUserFlowAttribute",
                "id": "City",
                "displayName": "City",
                "description": "your city",
                "userFlowAttributeType": "builtIn",
                "dataType": "string"
            }
        },
        {
            "id": "extension_guid_shoeSize",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "TextBox",
            "displayName": "Shoe size",
            "userFlowId": "B2C_1_Consumer",
            "userAttributeValues": [],
            "userAttribute": {
                "@odata.type": "#Microsoft.Graph.CustomUserFlowAttribute",
                "id": "extension_guid_shoeSize",
                "displayName": "Shoe size",
                "description": "Your shoe size",
                "userFlowAttributeType": "custom",
                "dataType": "string"
            }
        }
    ]
}
```
