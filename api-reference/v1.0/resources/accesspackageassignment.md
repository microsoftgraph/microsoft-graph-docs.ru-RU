---
title: тип ресурса accessPackageAssignment
description: Назначение пакета доступа — это назначение пакета доступа определенному субъекту в течение определенного периода времени.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bd2493b96043286c4585bec60b5af6f47130cf77
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651325"
---
# <a name="accesspackageassignment-resource-type"></a>тип ресурса accessPackageAssignment

Пространство имен: microsoft.graph

В [Azure AD Entitlement Management](entitlementmanagement-overview.md)назначение пакета доступа — это назначение пакета доступа определенному субъекту в течение определенного периода времени.  Например, в назначении пакета доступа может быть установлено, что пользователю Алисе назначен доступ через пакет продаж пакета доступа за период с января 2019 г. по июль 2019 г.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Списки accessPackageAssignments](../api/entitlementmanagement-list-assignments.md)|[коллекция accessPackageAssignment](accesspackageassignment.md)|Извлечение списка **объектов accessPackageAssignment.** |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Извлечение списка **объектов accessPackageAssignment,** фильтруемых на входе пользователя.|

> [!NOTE]
> Чтобы создать или удалить назначение пакета доступа для пользователя, используйте [метод accessPackageAssignmentRequest.](../api/entitlementmanagement-post-assignmentrequests.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|expiredDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String|Только для чтения.|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|Когда назначение доступа должно быть на месте. Только для чтения.|
|state|accessPackageAssignmentState|Состояние назначения пакета доступа. Допустимые значения: `delivering`, `partiallyDelivered`, `delivered`, `expired`, `deliveryFailed`, `unknownFutureValue`. Только для чтения. Поддерживает `$filter` (`eq`).|
|status|String|Дополнительные сведения о жизненном цикле назначения.  Возможные значения включают `Delivering` `Delivered` , или `NearExpiry1DayNotificationTriggered` `ExpiredNotificationTriggered` .  Только для чтения.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackage|[accessPackage](accesspackage.md)|Только для чтения. Допускается значение null. Поддерживает `$filter` `eq` () параметры **свойства id** `$expand` и запроса.|
|target|[accessPackageSubject](accesspackagesubject.md)|Тема назначения пакета доступа. Только для чтения. Допускается значение null. Поддерживает `$expand`. Поддерживает `$filter` `eq` () на **objectId**.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "id": "String (identifier)",
  "state": "String",
  "status": "String",
  "expiredDateTime": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


