---
title: Тип ресурса unifiedRoleAssignmentScheduleRequest
description: Представляет запрос на активные операции назначения ролей через Azure AD управление привилегированными пользователями.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 37d58a30835448655f3f26845e5a5fe7b3f3d699
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461480"
---
# <a name="unifiedroleassignmentschedulerequest-resource-type"></a>Тип ресурса unifiedRoleAssignmentScheduleRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос на активные операции назначения ролей через Azure Active Directory (Azure AD) управление привилегированными пользователями.

**unifiedRoleAssignmentScheduleRequest** — это сущность с моделью билета, используемая для управления жизненным циклом активных назначений ролей в каталоге. Он представляет намерение или решение пользователей и администраторов, а также обеспечивает гибкость для реализации повторяющегося планирования, шлюзов утверждения и т. д., `POST`по сравнению с предоставлением прямого доступа, `unifiedRoleAssignmentSchedule` `PUT``DELETE` `unifiedRoleAssignmentInstance`а также операций с и .

Администраторы могут использовать для `unifiedRoleAssignmentScheduleRequest` создания активных назначений ролей с временем начала и окончания или без нее. Хотя администратор может использовать его для создания запроса на активацию допустимого назначения роли, представленного [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md).

Наследуется от [запроса](request.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление unifiedRoleAssignmentScheduleRequests](../api/rbacapplication-list-roleassignmentschedulerequests.md)|[Коллекция unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Получение списка объектов [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и их свойств.|
|[Создание unifiedRoleAssignmentScheduleRequest](../api/rbacapplication-post-roleassignmentschedulerequests.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Создайте объект [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) .|
|[Получение unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Чтение свойств и связей объекта [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) .|
|[filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)|[Коллекция unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Получение списка объектов [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и их свойств, связанных с определенным пользователем.|
|[cancel](../api/unifiedroleassignmentschedulerequest-cancel.md)|Нет|Немедленно [отменяет unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и помечает его для удаления через 30 дней.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|Строка|Представляет тип операции назначения роли. Возможные значения: <ul><li>`AdminAssign`: администраторы могут назначать роли пользователям или группам.</li><li>`AdminRemove`: администраторы могут удалять пользователей или группы из ролей.</li><li> `AdminUpdate`: администраторы могут изменять существующие назначения ролей.</li><li>`AdminExtend`: администраторы могут продлить назначения с истекающим сроком действия.</li><li>`AdminRenew`: чтобы администраторы продлевали назначения с истекшим сроком действия.</li><li>`SelfActivate`: для активации назначений пользователями.</li><li>`SelfDeactivate`: для отключения активных назначений пользователями.</li><li>`SelfExtend`: пользователи должны запрашивать продление назначений с истекающим сроком действия.</li><li>`SelfRenew`: чтобы пользователи запрашивали продление назначений с истекшим сроком действия.</li></ul>|
|approvalId|Строка|Идентификатор утверждения запроса. Наследуется от [запроса](request.md).|
|appScopeId|Строка|Идентификатор области, относяшейся к приложению, если область назначения предназначена для конкретного приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами.|
|completedDateTime|DateTimeOffset|Время даты завершения запроса. Наследуется от [запроса](request.md).|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот запрос. Наследуется от [запроса](request.md).|
|createdDateTime|DateTimeOffset|Дата создания запроса. Наследуется от [запроса](request.md).|
|Customdata|Строка|Поле "Бесплатный текст" для определения любых пользовательских данных для запроса. Не используется. Наследуется от [запроса](request.md).|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением.|
|id|String|Уникальный идентификатор объекта unifiedRoleAssignmentScheduleRequest. Ключ, не допускающий значения NULL, только для чтения.|
|isValidationOnly|Boolean|Логическое значение, определяющее, является ли вызов проверкой или фактическим вызовом. Задайте это свойство только в том случае, если вы хотите проверить, применяется ли активация к дополнительным правилам, таким как MFA, перед фактической отправкой запроса.|
|Обоснование|String|Сообщение, предоставленное пользователями и администраторами при создании запроса о том, зачем он нужен.|
|principalId|Строка| Идентификатор субъекта, которому предоставляется назначение.|
|roleDefinitionId|Строка|Идентификатор объекта unifiedRoleDefinition, для который предназначено назначение. Только для чтения.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса на назначение роли.|
|status|String|Объект расписания запроса на назначение роли. Наследуется от [запроса](request.md).|
|targetScheduleId|Строка|Идентификатор объекта расписания, присоединенного к назначению.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Объект ticketInfo, присоединенный к запросу на назначение роли, который содержит сведения о номере билета и системе билетов.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Если запрос от допустимого администратора для активации роли, этот параметр отобразит связанное допустимое назначение для этой активации.|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если область назначения предназначена для конкретного приложения. Сущность containment.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на объект каталога, который является областью назначения. Предоставляется для того, чтобы вызывающие объекты могли получить объект каталога `$expand` , используя одновременно с получением назначения роли. Только для чтения. |
|Основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на субъект, который получает назначение роли через запрос. Предоставляется для того, чтобы вызывающие объекты `$expand` могли получить субъект одновременно с получением назначения роли. Только для чтения. |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее roleDefinition, для которых предназначено назначение. Предоставляется для того, чтобы вызывающие объекты могли получить определение роли `$expand` одновременно с получением назначения роли. roleDefinition.Id будет автоматически развернут.|
|targetSchedule|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)| Свойство, указывающее расписание назначения подходящей роли. |

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

