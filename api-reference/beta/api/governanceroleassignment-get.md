---
title: Получение governanceRoleAssignment
description: Получение свойств и связей объекта governanceRoleAssignment.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: f4b89a61919ed9635a14c7b734dbf4a55e6b7bf0
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399140"
---
# <a name="get-governanceroleassignment"></a>Получение governanceRoleAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Получение свойств и связей [объекта governanceRoleAssignment](../resources/governanceroleassignment.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).

### <a name="azure-resources"></a>Ресурсы Azure

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложения | PrivilegedAccess.Read.AzureResources |

### <a name="azure-ad"></a>Azure AD

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложения | PrivilegedAccess.Read.AzureAD |

### <a name="groups"></a>Группы

|Тип разрешения | Разрешения |
|:-------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureADGroup |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложения | PrivilegedAccess.Read.AzureADGroup |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
1. Получение [governanceRoleAssignment](../resources/governanceroleassignment.md) для ресурса

    *Примечание. Помимо области разрешений, инициатор запроса должен иметь по крайней мере одно назначение роли для ресурса.* 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. Получение [объекта governanceRoleAssignment](../resources/governanceroleassignment.md)
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод не **поддерживает** параметры [запроса OData](/graph/query-parameters)`$filter`, кроме настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `200 OK` отклика и [объект governanceRoleAssignment](../resources/governanceroleassignment.md) в теле отклика.
## <a name="example"></a>Пример
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
Получение [governanceRoleAssignment в](../resources/governanceroleassignment.md) подписке Wingtip Toys — Prod
##### <a name="request"></a>Запрос
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments/$entity",
    "id": "0ba78f41-ee7a-4227-adb9-1499431b2164",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "74487eb5-1630-4fa8-9581-0bb076ea5de3",
    "linkedEligibleRoleAssignmentId": null,
    "externalId": null,
    "startDateTime": "2018-01-22T23:47:19.687Z",
    "endDateTime": "2018-07-21T23:47:02.887Z",
    "memberType": "Direct",
    "assignmentState": "Eligible",
    "status": "Provisioned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


