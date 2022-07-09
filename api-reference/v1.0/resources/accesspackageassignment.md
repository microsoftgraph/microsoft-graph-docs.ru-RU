---
title: Тип ресурса accessPackageAssignment
description: Назначение пакета доступа — это назначение пакета доступа определенной теме на определенный период времени.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7a4f603ee7f3f1553d97c4d04b0b695e3c0c2c0e
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698046"
---
# <a name="accesspackageassignment-resource-type"></a>Тип ресурса accessPackageAssignment

Пространство имен: microsoft.graph

В [Azure AD управления правами](entitlementmanagement-overview.md) назначение пакета доступа — это назначение пакета доступа определенной теме на определенный период времени.  Например, назначение пакета доступа может указать, что пользователю Алисе был назначен доступ через пакет доступа Sales за период с января 2019 г. по июль 2019 г.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов accessPackageAssignment](../api/entitlementmanagement-list-assignments.md)|[Коллекция accessPackageAssignment](accesspackageassignment.md)|Получение списка объектов **accessPackageAssignment** . |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[Коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Получение списка объектов **accessPackageAssignment** , отфильтрованных по пользователю, выполнившего вход.|
|[Повторная обработка](../api/accesspackageassignment-reprocess.md) | Нет | Автоматически переоценка и принудительное применение назначений пользователя для определенного пакета доступа.|

> [!NOTE]
> Чтобы создать или удалить назначение пакета доступа для пользователя, используйте [метод accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) .

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|expiredDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String|Только для чтения.|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|Когда назначение доступа должно быть установлено. Только для чтения.|
|state|accessPackageAssignmentState|Состояние назначения пакета доступа. Допустимые значения: `delivering`, `partiallyDelivered`, `delivered`, `expired`, `deliveryFailed`, `unknownFutureValue`. Только для чтения. Поддерживает `$filter` (`eq`).|
|status|String|Дополнительные сведения о жизненном цикле назначения.  Возможные значения: `Delivering`, `Delivered`или `NearExpiry1DayNotificationTriggered``ExpiredNotificationTriggered`.  Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackage|[accessPackage](accesspackage.md)|Только для чтения. Допускается значение null. `$filter` Поддерживает (`eq`) для **свойства идентификатора** и параметров `$expand` запроса.|
|target|[accessPackageSubject](accesspackagesubject.md)|Тема назначения пакета доступа. Только для чтения. Допускается значение null. Поддерживает `$expand`. Поддерживает (`$filter``eq`) для **objectId**.|
|assignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)|Только для чтения. `$filter` Поддерживает (`eq`) для **свойства идентификатора** и параметров `$expand` запроса.|

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


