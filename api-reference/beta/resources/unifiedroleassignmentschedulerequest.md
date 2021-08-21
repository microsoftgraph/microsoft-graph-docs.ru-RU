---
title: тип ресурса unifiedRoleAssignmentScheduleRequest
description: Представляет запрос на активные операции назначения ролей через Azure AD управление привилегированными пользователями.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 540f3a0e4f9fa7017dafebb1a7ee5bc51def9788
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454005"
---
# <a name="unifiedroleassignmentschedulerequest-resource-type"></a>тип ресурса unifiedRoleAssignmentScheduleRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос на активные операции назначения ролей через Azure Active Directory (Azure AD) управление привилегированными пользователями.

**unifiedRoleAssignmentScheduleRequest** — это объект, моделируемый билетами, используемый для управления жизненным циклом активных назначений ролей в каталоге. Он представляет намерения или решения пользователей и администраторов, а также обеспечивает гибкость, чтобы включить реализацию повторяющихся планирования, ворот утверждения и так далее, по сравнению с непосредственной разоблачения , и операций и `POST` `PUT` `DELETE` `unifiedRoleAssignmentSchedule` `unifiedRoleAssignmentInstance` .

Администраторы могут использовать для создания активных назначений ролей с началом и конечным временем или без `unifiedRoleAssignmentScheduleRequest` него. Хотя администратор может использовать его для создания запроса на активацию назначения подходящих ролей, представленного [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md).

Наследует от [запроса](request.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список unifiedRoleAssignmentScheduleRequests](../api/unifiedroleassignmentschedulerequest-list.md)|[коллекция unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Получите список объектов [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и их свойств.|
|[Создание unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-post-unifiedroleassignmentschedulerequests.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Создайте новый [объект unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)|
|[Get unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)|
|[filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)|[коллекция unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Получите список объектов [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и их свойств, связанных с определенным пользователем.|
|[cancel](../api/unifiedroleassignmentschedulerequest-cancel.md)|Нет|Немедленно [отменяет унифицированнуюRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и отмечает его для удаления в течение 30 дней|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|String|Представляет тип операции при назначении ролей. Возможные значения: <ul><li>`AdminAssign`: Чтобы администраторы назначали роли пользователям или группам.</li><li>`AdminRemove`: Чтобы администраторы удаляли пользователей или группы из ролей.</li><li> `AdminUpdate`: Чтобы администраторы изменили существующие назначения ролей.</li><li>`AdminExtend`: Чтобы администраторы продлили назначения по истечении срока действия.</li><li>`AdminRenew`. Чтобы администраторы возобновляли истекаемы назначения.</li><li>`SelfActivate`: Чтобы пользователи активировали свои назначения.</li><li>`SelfDeactivate`: Чтобы пользователи отключались от активных назначений.</li><li>`SelfExtend`. Чтобы пользователи просили продлить срок действия назначений.</li><li>`SelfRenew`: Чтобы пользователи запрашивали продление истеканий назначений.</li></ul>|
|approvalId|String|Идентификатор утверждения запроса. Унаследовано от [запроса](request.md).|
|appScopeId|String|Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId,** чтобы ограничить область для определенных объектов каталогов, например административных единиц.|
|completedDateTime|DateTimeOffset|Время завершения запроса. Унаследовано от [запроса](request.md).|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот запрос. Унаследовано от [запроса](request.md).|
|createdDateTime|DateTimeOffset|Время создания запроса. Унаследовано от [запроса](request.md).|
|customData|String|Свободное текстовое поле для определения настраиваемой информации для запроса. Не используется. Унаследовано от [запроса](request.md).|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения.|
|id|String|Уникальный идентификатор для unifiedRoleAssignmentScheduleRequest. Key, not nullable, Read-only.|
|isValidationOnly|Логический|Boolean, определяющая, является ли вызов проверкой или фактическим вызовом. Только задайте это свойство, если необходимо проверить, подчиняется ли активация дополнительным правилам, таким как MFA, перед отправкой запроса.|
|обоснование|String|Сообщение, предоставленное пользователями и администраторами при создании запроса о необходимости.|
|principalId|String| Идентификатор основного, которому предоставляется назначение.|
|roleDefinitionId|String|Идентификатор унифицированногоRoleDefinition для назначения. Только для чтения.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса назначения ролей.|
|status|String|Объект расписания запроса назначения ролей. Унаследовано от [запроса](request.md).|
|targetScheduleId|String|Идентификатор объекта расписания, присоединенного к назначению.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Объект ticketInfo, присоединенный к запросу назначения ролей, который включает сведения о номере билета и системе билетов.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Если запрос от администратора, который имеет право на активацию роли, этот параметр покажет связанное назначение для этой активации.|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на объект каталога, который является областью назначения. При условии, что вызыватели могут получать объект каталога с помощью одновременно с назначением `$expand` ролей. Только для чтения. |
|основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на главного, получаюного назначение ролей через запрос. При условии, что звонители могут получать основное использование одновременно с `$expand` назначением ролей. Только для чтения. |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее рольDefinition для назначения. При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли. roleDefinition.Id будет автоматически расширена.|
|targetSchedule|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)| Свойство, указывающее расписание назначения подходящих ролей. |

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

