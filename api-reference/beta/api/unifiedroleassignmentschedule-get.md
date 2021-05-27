---
title: Get unifiedRoleAssignmentSchedule
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleAssignmentSchedule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d4e608946dea3314359b90c3c8b6b859c0a62566
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680399"
---
# <a name="get-unifiedroleassignmentschedule"></a>Get unifiedRoleAssignmentSchedule
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentSchedule.](../resources/unifiedroleassignmentschedule.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|PrivilegedAccess.ReadWrite.AzureAD|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|PrivilegedAccess.Read.AzureAD|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules/{unifiedRoleAssignmentSchedulesId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/roleAssignmentSchedules/b1477448-2cc6-4ceb-93b4-54a202a89413
```


### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentSchedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "principalId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "roleDefinitionId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "directoryScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "appScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "createdUsing": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "createdDateTime": "2020-09-09T21:35:27.91Z",
    "modifiedDateTime": "2020-09-09T21:35:27.91Z",
    "status": "Provisioned",
    "scheduleInfo": {
      "@odata.type": "microsoft.graph.requestSchedule"
    },
    "assignmentType": "Eligible",
    "memberType": "direct"
  }
}
```

