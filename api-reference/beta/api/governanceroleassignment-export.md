---
title: Экспорт governanceRoleAssignmentRequests
description: Извлеките коллекцию governanceRoleAssignmentRequests `application/octet-stream`в формате, который можно проанализировать как .csv в браузере.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: c95c544313e0696e340867b2ae4fe538d1e8f9fa
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397658"
---
# <a name="export-governanceroleassignmentrequests"></a>Экспорт governanceRoleAssignmentRequests

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Получение коллекции [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) `application/octet-stream`в формате, который можно проанализировать как .csv в браузере.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).

### <a name="azure-resources"></a>Ресурсы Azure

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | PrivilegedAccess.Read.AzureResources |

### <a name="azure-ad"></a>Azure AD

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | PrivilegedAccess.Read.AzureAD |

### <a name="groups"></a>Группы

|Тип разрешения | Разрешения |
|:-------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureADGroup |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | PrivilegedAccess.Read.AzureADGroup |


## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
Экспорт коллекции [governanceRoleAssignmentRequests для](../resources/governanceroleassignmentrequest.md) ресурса
    
>**Примечание:** Помимо области разрешений, этот запрос требует, чтобы инициатор запроса должен иметь по крайней мере одно назначение роли для ресурса. 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

Экспорт коллекции [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `200 OK` отклика и содержимое типа `application/octet-stream`.

## <a name="example"></a>Пример
В этом примере все назначения ролей .csv в подписке Wingtip Toys — Prod. 

##### <a name="request"></a>Запрос
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


