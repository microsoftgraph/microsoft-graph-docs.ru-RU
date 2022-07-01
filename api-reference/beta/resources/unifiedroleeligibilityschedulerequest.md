---
title: Тип ресурса unifiedRoleEligibilityScheduleRequest
description: Представляет запрос на допустимые операции назначения ролей через Azure AD управление привилегированными пользователями.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 557f67028190621c817b24188f5f44eb3c4c8dca
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446352"
---
# <a name="unifiedroleeligibilityschedulerequest-resource-type"></a>Тип ресурса unifiedRoleEligibilityScheduleRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос на право на роль для субъекта через PIM. Право на получение роли может быть безвозвратно допустимо без даты окончания срока действия или временно допустимой с датой окончания срока действия. Наследуется от [запроса](../resources/request.md).

Дополнительные сведения о сценариях PIM, которые можно определить с помощью типа ресурса **unifiedRoleEligibilityScheduleRequest** , см. в статье "Общие сведения об управлении ролями с помощью API управления привилегированными пользователями [(PIM](privilegedidentitymanagementv3-overview.md))".

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление unifiedRoleEligibilityScheduleRequests](../api/rbacapplication-list-roleeligibilityschedulerequests.md)|[Коллекция unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Получение запросов на получение прав на роль для субъектов, выполненных с помощью объекта unifiedRoleEligibilityScheduleRequest.|
|[Создание unifiedRoleEligibilityScheduleRequest](../api/rbacapplication-post-roleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Запрос права на роль для субъекта через объект unifiedRoleEligibilityScheduleRequest.|
|[Получение unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Ознакомьтесь с подробными сведениями о запросе на получение прав на роль, выполненном с помощью объекта unifiedRoleEligibilityScheduleRequest.|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)|[Коллекция unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|В PIM получите запросы о допустимости ролей для определенного субъекта. Субъект может быть создателем или утверждающим объектом unifiedRoleEligibilityScheduleRequest или быть целевым объектом для доступа к роли.|
|[cancel](../api/unifiedroleeligibilityschedulerequest-cancel.md)|Нет|Немедленно отмените **объект unifiedRoleEligibilityScheduleRequest**`Granted`, состояние которого имеет состояние и система автоматически удаляет отмененный запрос через 30 дней.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|String|Представляет тип операции в запросе на получение прав на роль. Возможные значения: <br/><ul><li>`AdminAssign`: администраторы могут назначать субъектам допустимые роли.</li><li>`AdminRemove`: чтобы администраторы удаляли допустимые роли из субъектов.</li><li> `AdminUpdate`: чтобы администраторы меняли существующие права на роль.</li><li>`AdminExtend`: чтобы администраторы расширяли права на роль с истекающим сроком действия.</li><li>`AdminRenew`: чтобы администраторы продлевали просроченные права доступа.</li><li>`UserAdd`: чтобы пользователи могли активировать соответствующие назначения.</li><li>`UserRemove`: для отключения активных подходящих назначений пользователями.</li><li>`UserExtend`: чтобы пользователи запрашивали продление допустимых назначений с истекающим сроком действия.</li><li>`UserRenew`: чтобы пользователи запрашивали продление допустимых назначений с истекшим сроком действия.</li></ul>|
|approvalId|String|Идентификатор утверждения запроса. Наследуется от [запроса](../resources/request.md).|
|appScopeId|String|Идентификатор области, относяшейся к приложению, если доступ к роли определяется приложением. Область действия роли определяет набор ресурсов, к которым субъект имеет право доступа. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|completedDateTime|DateTimeOffset|Время даты завершения запроса. Наследуется от [запроса](../resources/request.md).|
|createdBy|[identitySet](../resources/identityset.md)|Субъект, создавшего этот запрос. Наследуется от [запроса](../resources/request.md).|
|createdDateTime|DateTimeOffset|Дата создания запроса. Наследуется от [запроса](../resources/request.md).|
|Customdata|String|Поле "Бесплатный текст" для определения любых пользовательских данных для запроса. Не используется. Наследуется от [запроса](../resources/request.md).|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область допустимости роли. Область действия роли определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|id|String|Уникальный идентификатор объекта **unifiedRoleEligibilityScheduleRequest** . Ключ, не допускающий значения NULL, только для чтения.  Наследуется от [сущности](../resources/entity.md).|
|isValidationOnly|Boolean|Определяет, является ли вызов проверкой или фактическим вызовом. Задайте это свойство только в том случае, если вы хотите проверить, применяется ли активация к дополнительным правилам, таким как MFA, перед фактической отправкой запроса.|
|Обоснование|String|Сообщение, предоставляемое пользователями и администраторами при создании объекта **unifiedRoleEligibilityScheduleRequest** .|
|principalId|String|Идентификатор участника, которой предоставлено право на роль. Поддерживает `$filter` (`eq`, `ne`).|
|roleDefinitionId|String|Идентификатор объекта [unifiedRoleDefinition](unifiedroledefinition.md) , назначаемого субъекту. Поддерживает `$filter` (`eq`, `ne`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Период допустимости роли. В настоящее время повторяющиеся расписания не поддерживаются.|
|status|String|Состояние запроса на участие в роли. Наследуется от [запроса](../resources/request.md). Только для чтения. Поддерживает `$filter` (`eq`, `ne`).|
|targetScheduleId|String|Идентификатор объекта расписания, связанного с запросом на приемлемость. Поддерживает `$filter` (`eq`, `ne`).|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Сведения о билете, связанные с запросом на участие в роли, включая сведения о номере билета и системе билетов. Необязательное свойство.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если права на роль относятся к приложению. Допускается значение null. Поддерживает `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью действия роли. Только для чтения. Поддерживает `$expand`.|
|Основной|[directoryObject](../resources/directoryobject.md)|Субъект, который получает право на роль в запросе. Поддерживает `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Подробные сведения об [объекте unifiedRoleDefinition](../resources/unifiedroledefinition.md) , на который ссылаются через свойство **roleDefinitionId** . Поддерживает `$expand`.|
|targetSchedule|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Расписание для допустимости роли, на которую ссылаются через свойство **targetScheduleId** . Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest",
  "baseType": "microsoft.graph.request",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
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

