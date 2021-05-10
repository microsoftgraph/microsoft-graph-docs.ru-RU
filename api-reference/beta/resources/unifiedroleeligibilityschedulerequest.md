---
title: тип ресурса unifiedRoleEligibilityScheduleRequest
description: Представляет запрос на соответствующие операции назначения ролей через Azure AD управление привилегированными пользователями.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 812757ed3ab277c4a82da348686609ba284ffdbd
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299850"
---
# <a name="unifiedroleeligibilityschedulerequest-resource-type"></a>тип ресурса unifiedRoleEligibilityScheduleRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос на соответствующие операции назначения ролей через Azure AD управление привилегированными пользователями.

`unifiedRoleEligibilityScheduleRequest` — это объект, моделируемый билетами, используемый для управления жизненным циклом подходящих назначений ролей в каталоге. Он представляет намерения и решения пользователей и администраторов, а также обеспечивает гибкость, чтобы включить реализацию повторяющихся планирования, ворот утверждения и так далее, по сравнению с непосредственной разоблачения , и операций и `POST` `PUT` `DELETE` `unifiedRoleEligibilitySchedule` `unifiedRoleEligibilityInstance` .

Администраторы могут использовать для создания и/или обновления подходящих назначений ролей со временем начала и окончания или без `unifiedRoleEligibilityScheduleRequest` него. В то время как соответствующие администраторы могут использовать его для создания запроса на продление или продление соответствующих назначений.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список унифицированныхRoleEligibilityScheduleRequests](../api/unifiedroleeligibilityschedulerequest-list.md)|[коллекция unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Получите список объектов [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и их свойств.|
|[Создание unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-post-unifiedroleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Создайте новый [объект unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)|
|[Get unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)|
|[Обновление unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-update.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Обновление свойств объекта [unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)|[коллекция unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Получите список объектов [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и их свойств, связанных с определенным пользователем.|
|[cancel](../api/unifiedroleeligibilityschedulerequest-cancel.md)|Нет|Немедленно [отменяет унифицированнуюRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и отмечает его для удаления в течение 30 дней|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|Строка|Представление типа операции при назначении ролей. Значение может быть <ul><li>`AdminAdd`: Администраторы назначают пользователям и группам роли;</li><li>`UserAdd`: Пользователи активируют подходящие назначения;</li><li> `AdminUpdate`: Администраторы изменяют существующие назначения ролей</li><li>`AdminRemove`: Администраторы удаляют пользователей и группы из ролей;<li>`UserRemove`: Пользователи деактивируют активные назначения;<li>`UserExtend`: Пользователи просят продлить срок действия назначений;</li><li>`AdminExtend`. Администраторы расширяют назначения по истечении срока действия.</li><li>`UserRenew`: Пользователи просят продлить срок действия назначений;</li><li>`AdminRenew`. Администраторы расширяют назначения по истечении срока действия.</li></ul>|
|appScopeId|Строка|Id конкретной области приложения, когда область назначения является конкретной. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте "/" для области для клиента. Области приложений — это области, которые определяются и понимаются только этим приложением.|
|directoryScopeId|Строка|Id объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Области приложений — это области, которые определяются и понимаются только этим приложением.|
|id|Строка|Уникальный идентификатор для unifiedRoleEligibilityScheduleRequest.|
|isValidationOnly|Логический|Логический|Boolean, определяющая, является ли вызов проверкой или фактическим вызовом. Только задайте это свойство, если необходимо проверить, подчиняется ли активация дополнительным правилам, таким как MFA, перед отправкой запроса.|
|обоснование|Строка|Сообщение, предоставленное пользователями и администраторами при создании запроса о необходимости.|
|principalId|Строка| Объект объекта, которому предоставляется назначение.|
|roleDefinitionId|Строка|ID унифицированногоRoleDefinition для назначения. Только для чтения.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса назначения ролей.|
|targetScheduleId|Строка|ID объекта расписания, прикрепленного к назначению.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Объект ticketInfo, присоединенный к запросу назначения ролей, который включает сведения о номере билета и системе билетов.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на объект каталога, который является областью назначения. При условии, что вызыватели могут получать объект каталога с помощью одновременно с назначением `$expand` ролей. Только для чтения.|
|основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на главного, получаюного назначение ролей через запрос. При условии, что звонители могут получать основное использование одновременно с `$expand` назначением ролей. Только для чтения. |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее рольDefinition для назначения. При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли. roleDefinition.Id будет автоматически расширена|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest",
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

