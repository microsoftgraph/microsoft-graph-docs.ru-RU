---
title: Управление экспортомRoleAssignmentRequests
description: Извлеките коллекцию файлов governanceRoleAssignmentRequests в формате, которые можно .csv в `application/octet-stream` браузере.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8faff2bbd4b41eda693467b55641204cb6bbaef3
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350854"
---
# <a name="export-governanceroleassignmentrequests"></a>Управление экспортомRoleAssignmentRequests

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлеките коллекцию [файлов governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) в формате, которые можно .csv в `application/octet-stream` браузере.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).

### <a name="azure-resources"></a>Ресурсы Azure

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Application | PrivilegedAccess.Read.AzureResources |

### <a name="azure-ad"></a>Azure AD

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Application | PrivilegedAccess.Read.AzureAD |

### <a name="groups"></a>Группы

|Тип разрешения | Разрешения |
|:-------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureADGroup |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Application | PrivilegedAccess.Read.AzureADGroup |


## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
Экспорт коллекции [governanceRoleAssignmentRequests на](../resources/governanceroleassignmentrequest.md) ресурсе
    
>**Примечание:** Помимо области разрешений, для этого запроса требуется, чтобы у запросителя было по крайней мере одно назначение ролей на ресурсе. 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

Экспорт коллекции [моих произведений governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)
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

## <a name="response"></a>Ответ
В случае успешной работы этот метод возвращает код `200 OK` ответа и содержимое `application/octet-stream` типа.

## <a name="example"></a>Пример
В этом примере сохраняется все назначения ролей в .csv в подписной папке Wingtip Toys — Prod. 

##### <a name="request"></a>Запрос
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a>Ответ
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


