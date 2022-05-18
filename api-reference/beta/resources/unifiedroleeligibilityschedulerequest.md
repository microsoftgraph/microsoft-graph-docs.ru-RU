---
title: Тип ресурса unifiedRoleEligibilityScheduleRequest
description: Представляет запрос на допустимые операции назначения ролей через Azure AD управление привилегированными пользователями.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 82224699c7bbe80e9ec14e39494fd8a37c1d31be
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461354"
---
# <a name="unifiedroleeligibilityschedulerequest-resource-type"></a>Тип ресурса unifiedRoleEligibilityScheduleRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос на назначение допустимой роли через Azure AD управление привилегированными пользователями.

**unifiedRoleEligibilityScheduleRequest** — это сущность с моделью билета, используемая для управления жизненным циклом допустимых назначений ролей в каталоге. Он представляет намерение или решение пользователей и администраторов, а также обеспечивает гибкость для реализации повторяющегося планирования, `POST``PUT``DELETE` шлюзов утверждения и т. д. по сравнению с предоставлением непосредственного доступа и операциями с ресурсами **unifiedRoleEligibilitySchedule** и **unifiedRoleEligibilityInstance**.

Администраторы могут использовать **unifiedRoleEligibilityScheduleRequest** для создания и (или) обновления допустимых назначений ролей с использованием или без времени начала и окончания. Хотя соответствующие администраторы могут использовать его для создания запроса на продление или продление соответствующих назначений.

Наследуется от [запроса](request.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление unifiedRoleEligibilityScheduleRequests](../api/rbacapplication-list-roleeligibilityschedulerequests.md)|[Коллекция unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Получение списка объектов [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и их свойств.|
|[Создание unifiedRoleEligibilityScheduleRequest](../api/rbacapplication-post-roleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Создайте объект [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) .|
|[Получение unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Чтение свойств и связей объекта [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) .|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)|[Коллекция unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Получение списка объектов [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и их свойств, связанных с определенным пользователем.|
|[cancel](../api/unifiedroleeligibilityschedulerequest-cancel.md)|Нет|Немедленно [отменяет unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и помечает его для удаления через 30 дней.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|Строка|Представляет тип операции с назначением соответствия роли. Возможные значения: <ul><li>`AdminAssign`: администраторы могут назначать роли пользователям или группам.</li><li>`AdminExtend`: администраторы могут продлить назначения с истекающим сроком действия.</li><li>`AdminUpdate`: администраторы могут изменять существующие назначения ролей.</li><li>`AdminRenew`: чтобы администраторы продлевали назначения с истекшим сроком действия.</li><li>`AdminRemove`: администраторы могут удалять пользователей или группы из соответствующих ролей.</li><li>`UserAdd`: чтобы пользователи могли активировать соответствующие назначения.</li><li>`UserExtend`: чтобы пользователи запрашивали продление допустимых назначений с истекающим сроком действия.</li><li>`UserRemove`: для отключения активных подходящих назначений пользователями.</li><li>`UserRenew`: чтобы пользователи запрашивали продление допустимых назначений с истекшим сроком действия.</li></ul>|
|approvalId|Строка|Идентификатор утверждения запроса. Наследуется от [запроса](request.md).|
|appScopeId|Строка|Идентификатор области, относяшейся к приложению, если область назначения предназначена для конкретного приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами.|
|completedDateTime|DateTimeOffset|Время даты завершения запроса. Наследуется от [запроса](request.md).|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот запрос. Наследуется от [запроса](request.md).|
|createdDateTime|DateTimeOffset|Дата создания запроса. Наследуется от [запроса](request.md).|
|Customdata|Строка|Поле "Бесплатный текст" для определения любых пользовательских данных для запроса. Не используется. Наследуется от [запроса](request.md).|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением.|
|id|String|Уникальный идентификатор объекта unifiedRoleEligibilityScheduleRequest. Только для чтения.|
|isValidationOnly|Boolean|Логическое значение, определяющее, является ли вызов проверкой или фактическим вызовом. Задайте это свойство только в том случае, если вы хотите проверить, применяется ли активация к дополнительным правилам, таким как MFA, перед фактической отправкой запроса.|
|Обоснование|String|Сообщение, предоставленное пользователями и администраторами при создании запроса о том, зачем он нужен.|
|principalId|Строка| Идентификатор субъекта, которому предоставляется назначение. Например, пользователь или группа. Для групп они должны быть назначены ролям, то есть **isAssignableToRole** свойства группы, для которого задано значение `true`.|
|roleDefinitionId|Строка|Идентификатор объекта unifiedRoleDefinition, для который предназначено назначение. Только для чтения.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса на назначение роли.|
|status|String|Объект расписания запроса на участие в роли. Наследуется от [запроса](request.md).|
|targetScheduleId|Строка|Период времени, в течение которого допустимо назначение соответствия требованиям.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Сведения о номере билета и системе билета, присоединенной к запросу на назначение роли.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если область назначения предназначена для конкретного приложения. Сущность containment.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на объект каталога, который является областью назначения. Предоставляется для того, чтобы вызывающие объекты могли получить объект каталога `$expand` , используя одновременно с получением назначения роли. Только для чтения.|
|Основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на субъект, который получает назначение роли через запрос. Предоставляется для того, чтобы вызывающие объекты `$expand` могли получить субъект одновременно с получением назначения роли. Только для чтения. |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее roleDefinition, для которых предназначено назначение. Предоставляется для того, чтобы вызывающие объекты могли получить определение роли `$expand` одновременно с получением назначения роли. roleDefinition.Id будет автоматически развернут.|
|targetSchedule|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)| Свойство, указывающее расписание назначения подходящей роли. |

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

