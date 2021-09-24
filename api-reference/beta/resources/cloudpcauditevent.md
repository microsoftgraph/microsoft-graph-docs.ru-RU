---
title: тип ресурса cloudPcAuditEvent
description: Представляет объект событий аудита.
author: ecmadao
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 155ecf60bcd160877fe905ef1bd6b328b60bb49d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507517"
---
# <a name="cloudpcauditevent-resource-type"></a>тип ресурса cloudPcAuditEvent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект событий аудита.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список объектов auditEvent](../api/virtualendpoint-list-auditevents.md)|[коллекция cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Список всех [объектов cloudPcAuditEvent](../resources/cloudpcauditevent.md) в клиенте.|
|[Get cloudPcAuditEvent](../api/cloudpcauditevent-get.md)|[cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcAuditEvent.](../resources/cloudpcauditevent.md)|
|[Функция getAuditActivityTypes](../api/cloudpcauditevent-getauditactivitytypes.md)|Коллекция строк|Получите типы действий аудита.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта аудита. Только для чтения.|
|displayName|String|Отображаемое имя события. Только для чтения.|
|componentName|String|Имя компонента. Только для чтения.|
|actor|[cloudPcAuditActor](../resources/cloudpcauditactor.md)|Пользователь и приложение Azure AD, связанные с событием аудита. Только для чтения.|
|activity|String|Понятное имя действия.Необязательное свойство.|
|activityDateTime|DateTimeOffset|Дата и время выполнения действия (в формате UTC).Только для чтения.|
|activityType|String|Тип выполняемой деятельности.Только для чтения.|
|activityOperationType|[cloudPcAuditActivityOperationType](#cloudpcauditactivityoperationtype-values)|Тип операции HTTP для действия. Возможные значения включают  `create` `delete` , и `patch` `other` . Только для чтения.|
|activityResult|[cloudPcAuditActivityResult](#cloudpcauditactivityresult-values)|Результат действия.Только для чтения.|
|correlationId|String|Идентификатор клиентского запроса, используемый для сопоставления действий в системе.Только для чтения.|
|resources|[коллекция cloudPcAuditResource](../resources/cloudpcauditresource.md)|Список объектов cloudPcAuditResource.Только для чтения.|
|category|[cloudPcAuditCategory](#cloudpcauditcategory-values)|Категория аудита. Только для чтения.|

### <a name="cloudpcauditactivityoperationtype-values"></a>значения cloudPcAuditActivityOperationType

|Member|Описание|
|:---|:---|
|create|Создание операции.|
|delete|Удаление операции.|
|исправление|Операция исправлений.|
|другие|Другая операция.|

### <a name="cloudpcauditactivityresult-values"></a>значения cloudPcAuditActivityResult

|Member|Описание|
|:---|:---|
|success|Операция прошла успешно.|
|clientError|Операция не удалась из-за ошибки клиента.|
|сбой|Не удалось выполнить операцию.|
|timeExceeded|Операция не справилась с периодией времени.|
|другие|Другой результат.|

### <a name="cloudpcauditcategory-values"></a>значения cloudPcAuditCategory

|Member|Описание|
|:---|:---|
|cloudPC|Категория облачного КОМПЬЮТЕРА.|
|другие |Другая категория.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcAuditEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.cloudPcAuditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
        "displayName": "String",
        "roleScopeTagId": "String"
      }
    ],
    "remoteTenantId": "String",
    "remoteUserId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.cloudPcAuditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```
