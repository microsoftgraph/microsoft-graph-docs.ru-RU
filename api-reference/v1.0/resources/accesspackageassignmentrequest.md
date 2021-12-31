---
title: тип ресурса accessPackageAssignmentRequest
description: Запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ca963bd2a538cad8efe8692e82c6e1da678c0a21
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651451"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>тип ресурса accessPackageAssignmentRequest

Пространство имен: microsoft.graph


В [Azure AD Entitlement Management](entitlementmanagement-overview.md)запрос на назначение пакета доступа создается пользователем или от имени пользователя, который хочет получить назначение пакета доступа. Если запрос является успешным, с любыми необходимыми утверждениями, пользователь получает назначение пакета доступа и является субъектом этого назначения пакета доступа.  Azure AD также создает запросы на назначение пакетов доступа автоматически для отслеживания удаления доступа.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список accessPackageAssignmentRequests](../api/entitlementmanagement-list-assignmentrequests.md)|[accessPackageAssignmentRequest collection](accesspackageassignmentrequest.md)|Извлечение списка **объектов accesspackageassignmentrequest.** |
| [Создание accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Создает новый **объект accessPackageAssignmentRequest.** |
|[Получить accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md)|[accessPackageAssignmentRequest](accesspackageassignmentrequest.md)|Чтение свойств и связей объекта **accessPackageAssignmentRequest.** |
|[Удаление accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md)|Нет|Удаление **accessPackageAssignmentRequest**. |
|[filterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Извлечение списка **объектов accessPackageAssignmentRequest,** фильтруемых на входе пользователя.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Отмена **объекта accessPackageAssignmentRequest,** который находится в отменяемом состоянии.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|completedDate|DateTimeOffset|Дата окончания обработки , успешной или неудачной, запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|id|String|Только для чтения.|
|requestType|accessPackageRequestType|Тип запроса. Возможные значения: `notSpecified` , , , , , , , , `userAdd` `userUpdate` `userRemove` `adminAdd` `adminUpdate` `adminRemove` `systemAdd` `systemUpdate` `systemRemove` `onBehalfAdd` `unknownFutureValue` . Запрос от самого пользователя будет иметь requestType или `UserAdd` `UserRemove` . Это свойство нельзя изменить после набора.|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|Диапазон дат, которые должен быть назначен запросчику. Это свойство нельзя изменить после набора.|
|state|accessPackageRequestState|Состояние запроса. Возможные значения: `submitted`, `pendingApproval`, `delivering`, `delivered`, `deliveryFailed`, `denied`, `scheduled`, `canceled`, `partiallyDelivered`, `unknownFutureValue`. Только для чтения.|
|status|String|Дополнительные сведения о состоянии обработки запросов. Только для чтения.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|Пакет доступа, связанный с accessPackageAssignmentRequest. Пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам для одного или более пользователей. Только для чтения. Допускается значение null. <br/><br/> Поддерживает `$expand`.|
|назначение|[accessPackageAssignment](../resources/accesspackageassignment.md)|Для **requestType** или , это назначение пакета `UserAdd` `AdminAdd` доступа, запрашиваемого для создания.  Для **requestType** или , это свойство существующего `UserRemove` `AdminRemove` `SystemRemove` `id` назначения, которые будут удалены.  <br/><br/> Поддерживает `$expand`.|
|запросчик|[accessPackageSubject](../resources/accesspackagesubject.md)|Субъекту, который запрашивал или, если прямое назначение, было назначено. Только для чтения. Допускается значение null. Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "id": "String (identifier)",
  "requestType": "String",
  "state": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "completedDate": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


