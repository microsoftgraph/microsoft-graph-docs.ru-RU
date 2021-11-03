---
title: тип ресурса unifiedRoleEligibilityScheduleRequest
description: Представляет запрос на соответствующие операции назначения ролей через Azure AD управление привилегированными пользователями.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 446e5f32ab7443266c16b6d89a9d0fa9913e48e4
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695232"
---
# <a name="unifiedroleeligibilityschedulerequest-resource-type"></a>тип ресурса unifiedRoleEligibilityScheduleRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос на назначение подходящих ролей через Azure AD управление привилегированными пользователями.

**unifiedRoleEligibilityScheduleRequest** — это объект, моделируемый билетами, используемый для управления жизненным циклом подходящих назначений ролей в каталоге. Он представляет собой намерение или решение пользователей и администраторов, а также обеспечивает гибкость, чтобы включить реализацию повторяющихся планирования, ворот утверждения и так далее, по сравнению с непосредственной разоблачения , и операций на `POST` `PUT` `DELETE` **unifiedRoleEligibilitySchedule** и **unifiedRoleEligibilityInstance** ресурсов.

Администраторы могут использовать **unifiedRoleEligibilityScheduleRequest** для создания и/или обновления подходящих назначений ролей с началом или без времени начала и окончания. В то время как соответствующие администраторы могут использовать его для создания запроса на продление или продление соответствующих назначений.

Наследует от [запроса](request.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список унифицированныхRoleEligibilityScheduleRequests](../api/unifiedroleeligibilityschedulerequest-list.md)|[коллекция unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Получите список объектов [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и их свойств.|
|[Создание unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-post-unifiedroleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Создайте новый [объект unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)|
|[Get unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)|[коллекция unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Получите список объектов [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и их свойств, связанных с определенным пользователем.|
|[cancel](../api/unifiedroleeligibilityschedulerequest-cancel.md)|Нет|Немедленно [отменяет унифицированнуюRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и отмечает его для удаления в течение 30 дней|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|String|Представляет тип операции по назначению права на роль. Возможные значения: <ul><li>`AdminAssign`. Чтобы администраторы назначали права на роль пользователям или группам в роли.</li><li>`AdminExtend`: Чтобы администраторы продлили назначения по истечении срока действия.</li><li>`AdminUpdate`: Чтобы администраторы изменили существующие назначения ролей.</li><li>`AdminRenew`. Чтобы администраторы возобновляли истекаемы назначения.</li><li>`AdminRemove`: Чтобы администраторы удаляли пользователей или группы из подходящих ролей.</li><li>`UserAdd`: Чтобы пользователи активировали соответствующие назначения.</li><li>`UserExtend`: Чтобы пользователи просили продлить срок действия соответствующих назначений.</li><li>`UserRemove`. Чтобы пользователи отключались от активных назначений.</li><li>`UserRenew`. Чтобы пользователи просили продлить срок действия своих назначений, имеющих право на срок действия.</li></ul>|
|approvalId|String|Идентификатор утверждения запроса. Унаследовано от [запроса](request.md).|
|appScopeId|String|Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId,** чтобы ограничить область для определенных объектов каталогов, например административных единиц.|
|completedDateTime|DateTimeOffset|Время завершения запроса. Унаследовано от [запроса](request.md).|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот запрос. Унаследовано от [запроса](request.md).|
|createdDateTime|DateTimeOffset|Время создания запроса. Унаследовано от [запроса](request.md).|
|customData|String|Свободное текстовое поле для определения настраиваемой информации для запроса. Не используется. Унаследовано от [запроса](request.md).|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения.|
|id|String|Уникальный идентификатор для unifiedRoleEligibilityScheduleRequest. Только для чтения.|
|isValidationOnly|Логический|Boolean, определяющая, является ли вызов проверкой или фактическим вызовом. Только задайте это свойство, если необходимо проверить, подчиняется ли активация дополнительным правилам, таким как MFA, перед отправкой запроса.|
|обоснование|String|Сообщение, предоставленное пользователями и администраторами при создании запроса о необходимости.|
|principalId|String| Идентификатор основного, которому предоставляется назначение. Например, пользователь или группа. Для групп они должны назначаться ролям, то есть **isAssignableToRole** свойства группы, задаваемого `true` .|
|roleDefinitionId|String|Идентификатор унифицированногоRoleDefinition для назначения. Только для чтения.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса назначения ролей.|
|status|String|Объект расписания запроса на право на роль. Унаследовано от [запроса](request.md).|
|targetScheduleId|String|Период времени, для которого допустимо назначение.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Сведения о номере билета и системе билетов, присоединенных к запросу назначения ролей.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с сведениями о области, определенной для приложения, когда область назначения является конкретной для приложения. Объект containment.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на объект каталога, который является областью назначения. При условии, что вызыватели могут получать объект каталога с помощью одновременно с назначением `$expand` ролей. Только для чтения.|
|основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на главного, получаюного назначение ролей через запрос. При условии, что звонители могут получать основное использование одновременно с `$expand` назначением ролей. Только для чтения. |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее рольDefinition для назначения. При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли. roleDefinition.Id будет автоматически расширена.|
|targetSchedule|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)| Свойство, указывающее расписание назначения подходящих ролей. |

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

