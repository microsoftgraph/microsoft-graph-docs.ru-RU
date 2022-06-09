---
title: Тип ресурса unifiedRoleAssignmentScheduleRequest
description: В PIM представляет запрос на назначение активной роли субъекту. Назначение роли может быть безвозвратно активным с датой окончания срока действия или временно активной после активации допустимого назначения.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1e88e893560273832de0d943e5e65d43aa759792
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971198"
---
# <a name="unifiedroleassignmentschedulerequest-resource-type"></a>Тип ресурса unifiedRoleAssignmentScheduleRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В PIM представляет запрос на назначение активной роли субъекту. Назначение роли может быть безвозвратно активным с датой окончания срока действия или временно активной после активации допустимого назначения. Наследуется от [запроса](../resources/request.md).

Дополнительные сведения о сценариях PIM, которые можно определить с помощью типа ресурса **unifiedRoleAssignmentScheduleRequest** , см. в обзоре управления ролями с помощью API управления привилегированными пользователями [(PIM](privilegedidentitymanagementv3-overview.md)).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление unifiedRoleAssignmentScheduleRequests](../api/rbacapplication-list-roleassignmentschedulerequests.md)|[Коллекция unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)| Извлеките запросы на активные назначения ролей, выполненные с помощью объекта [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) .|
|[Создание unifiedRoleAssignmentScheduleRequest](../api/rbacapplication-post-roleassignmentschedulerequests.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Создайте запрос на назначение активной и постоянной роли или активируйте, деактивируйте, продлить или продлить допустимое назначение ролей.|
|[Получение unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Получение запроса на назначение активной роли с помощью объекта [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) .|
|[cancel](../api/unifiedroleassignmentschedulerequest-cancel.md)|Нет| Отмена запроса на назначение активной роли. |
|[filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)|[Коллекция unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)| Получение запросов на активные назначения ролей для определенного субъекта.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|String|Представляет тип операции в запросе на назначение роли. Возможные значения: `adminAssign`, `adminUpdate`, `adminRemove`, `selfActivate`, `selfDeactivate`, `adminExtend`, `adminRenew`, `selfExtend`, `selfRenew`, `unknownFutureValue`. <br/><ul><li>`adminAssign`: администраторы могут назначать роли субъектам.</li><li>`adminRemove`: чтобы администраторы удаляли участников из ролей.</li><li> `adminUpdate`: администраторы могут изменять существующие назначения ролей.</li><li>`adminExtend`: администраторы могут продлить назначения с истекающим сроком действия.</li><li>`adminRenew`: чтобы администраторы продлевали назначения с истекшим сроком действия.</li><li>`selfActivate`: чтобы субъекты активировали свои назначения.</li><li>`selfDeactivate`: для деактивации активных назначений субъектами.</li><li>`selfExtend`: чтобы субъекты запрашивали продление назначений с истекающим сроком действия.</li><li>`selfRenew`: чтобы субъекты запрашивали продление назначений с истекшим сроком действия.</li></ul>|
|approvalId|Строка|Идентификатор утверждения запроса. Наследуется от [запроса](../resources/request.md).|
|appScopeId|Строка|Идентификатор области, относяшейся к конкретному приложению, если назначение предназначено для приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|completedDateTime|DateTimeOffset|Время даты завершения запроса. Наследуется от [запроса](../resources/request.md).|
|createdBy|[identitySet](../resources/identityset.md)|Субъект, создавшего этот запрос. Наследуется от [запроса](../resources/request.md). Только для чтения. `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|createdDateTime|DateTimeOffset|Дата создания запроса. Наследуется от [запроса](../resources/request.md). Только для чтения.|
|Customdata|Строка|Поле "Бесплатный текст" для определения любых пользовательских данных для запроса. Не используется. Наследуется от [запроса](../resources/request.md).|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|id|Строка|Уникальный идентификатор объекта **unifiedRoleAssignmentScheduleRequest** . Ключ, не допускающий значения NULL, только для чтения. Наследуется от [сущности](../resources/entity.md). Поддерживает `$filter` (`eq`, `ne`).|
|isValidationOnly|Boolean|Определяет, является ли вызов проверкой или фактическим вызовом. Задайте это свойство только в том случае, если вы хотите проверить, применяется ли активация к дополнительным правилам, таким как MFA, перед фактической отправкой запроса.|
|Обоснование|String|Сообщение, предоставляемое пользователями и администраторами при создании объекта **unifiedRoleAssignmentScheduleRequest** .|
|principalId|Строка|Идентификатор участника, которым было предоставлено назначение. Поддерживает `$filter` (`eq`, `ne`).|
|roleDefinitionId|Строка|Идентификатор объекта [unifiedRoleDefinition](unifiedroledefinition.md) , назначаемого субъекту. Поддерживает `$filter` (`eq`, `ne`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Период назначения роли. В настоящее время повторяющиеся расписания не поддерживаются.|
|status|String|Состояние запроса на назначение роли. Наследуется от [запроса](../resources/request.md). Только для чтения. Поддерживает `$filter` (`eq`, `ne`).|
|targetScheduleId|Строка|Идентификатор объекта расписания, связанного с запросом на назначение. Поддерживает `$filter` (`eq`, `ne`).|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Сведения о билете, связанные с запросом на назначение роли, включая сведения о номере билета и системе билетов.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Если запрос от допустимого администратора для активации роли, этот параметр отобразит связанное допустимое назначение для этой активации. В противном случае это .`null` Поддерживает `$expand`.|
|appScope|[appScope](../resources/appscope.md)| Свойство только для чтения с подробными сведениями об области приложения, если назначение предназначено для приложения. Допускается значение null. Поддерживает `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью назначения. Только для чтения. Поддерживает `$expand`.|
|Основной|[directoryObject](../resources/directoryobject.md)|Субъект, который получает назначение роли через запрос. Поддерживает `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Подробные сведения об [объекте unifiedRoleDefinition](../resources/unifiedroledefinition.md) , на который ссылаются через свойство **roleDefinitionId** . Поддерживает `$expand`.|
|targetSchedule|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Расписание назначения подходящей роли, на которое ссылаются через **свойство targetScheduleId** . Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "baseType": "microsoft.graph.request",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "id": "String (identifier)",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```

