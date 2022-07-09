---
title: Тип ресурса accessPackageAssignmentRequest
description: Запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета для доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cdf2e4111daeea48babd57aac912006bd2418187
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698361"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>Тип ресурса accessPackageAssignmentRequest

Пространство имен: microsoft.graph


В [Azure AD управления правами](entitlementmanagement-overview.md) запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа, или от его имени. Если запрос выполнен успешно, при наличии необходимых утверждений пользователь получает назначение пакета для доступа и является субъектом полученного назначения пакета доступа.  Azure AD также автоматически создает запросы на назначение пакетов для отслеживания удаления доступа.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление accessPackageAssignmentRequests](../api/entitlementmanagement-list-assignmentrequests.md)|[Коллекция accessPackageAssignmentRequest](accesspackageassignmentrequest.md)|Получение списка объектов **accesspackageassignmentrequest** . |
| [Создание accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Создает объект **accessPackageAssignmentRequest** . |
|[Получение accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md)|[accessPackageAssignmentRequest](accesspackageassignmentrequest.md)|Чтение свойств и связей объекта **accessPackageAssignmentRequest** . |
|[Удаление accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md)|Отсутствует|Удаление **объекта accessPackageAssignmentRequest**. |
|[filterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[Коллекция accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Получение списка объектов **accessPackageAssignmentRequest** , отфильтрованных по пользователю, выполнившего вход.|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|[Коллекция accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Отмена **объекта accessPackageAssignmentRequest** , который находится в состоянии отмены.|
|[Повторная обработка](../api/accesspackageassignmentrequest-reprocess.md) | Отсутствует | Автоматически повторите запрос пользователя на доступ к пакету доступа.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|Дата окончания обработки (успешного или неудачного) запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|id|String|Только для чтения.|
|requestType|accessPackageRequestType|Тип запроса. Возможные значения: `notSpecified`, , `userAdd`, `userUpdate`, `userRemove`, `adminAdd`, `adminRemove``adminUpdate`, `systemAdd`, `systemUpdate``systemRemove`, `onBehalfAdd``unknownFutureValue`. Запрос от пользователя должен иметь значение requestType или `UserAdd` `UserRemove`. Это свойство нельзя изменить после задания.|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|Диапазон дат, которые необходимо назначить инициатору запроса. Это свойство нельзя изменить после задания.|
|state|accessPackageRequestState|Состояние запроса. Возможные значения: `submitted`, `pendingApproval`, `delivering`, `delivered`, `deliveryFailed`, `denied`, `scheduled`, `canceled`, `partiallyDelivered`, `unknownFutureValue`. Только для чтения.|
|status|String|Дополнительные сведения о состоянии обработки запроса. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|Пакет доступа, связанный с accessPackageAssignmentRequest. Пакет доступа определяет коллекции ролей ресурсов и политики того, как один или несколько пользователей могут получить доступ к этим ресурсам. Только для чтения. Допускается значение null. <br/><br/> Поддерживает `$expand`.|
|Назначения|[accessPackageAssignment](../resources/accesspackageassignment.md)|Для **requestType** или `UserAdd` `AdminAdd`, это назначение пакета доступа, запрашиваемого для создания.  Для **requestType** или `UserRemove``AdminRemove` `SystemRemove`, это свойство `id` существующего назначения, которое необходимо удалить.  <br/><br/> Поддерживает `$expand`.|
|Запрашивающего|[accessPackageSubject](../resources/accesspackagesubject.md)|Субъект, который запрашивал или, если было назначено прямое назначение. Только для чтения. Допускается значение null. Поддерживает `$expand`.|

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
  "completedDateTime": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


