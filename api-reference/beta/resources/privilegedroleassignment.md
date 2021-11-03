---
title: тип ресурса privilegedRoleAssignment
description: 'Представляет привилегированное назначение роли для конкретного пользователя. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 2786b2a7c2d231c8d3f87f8b538358e45b3fd3bc
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694176"
---
# <a name="privilegedroleassignment-resource-type-deprecated"></a>тип ресурса privilegedRoleAssignment (неподготовленный)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1AADRoles-deprecation](../../includes/pim-v1aadroles-deprecation.md)]

Представляет привилегированное назначение роли для конкретного пользователя. 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список коллекции privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)|Получите коллекцию объектов privilegedRoleAssignment.|
|[Получение privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Чтение свойств и связей объекта privilegedRoleAssignment.|
|[Создание задания](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Создайте новое назначение, разместив в коллекции назначений.|
|[Удаление](../api/privilegedroleassignment-delete.md) | Нет |Удаление объекта privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Выполнение назначения ролей как бессрочного.|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Выполнение назначения ролей как соответствующего требованиям.|
|[my](../api/privilegedroleassignment-my.md)|Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)|Получите привилегированные назначения ролей текущего пользователя.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|Время даты UTC, когда истекает срок действия временного назначения привилегированных ролей. Для назначения постоянных ролей значение null.|
|id|string| Уникальный идентификатор для назначения привилегированных ролей. Только для чтения. Он находится в формате "userId_roleId", где userId — это строка GUID для пользовательского id azure AD, а roleId — строка GUID для id роли администратора Azure.|
|isElevated|логический|**значение true,** если назначение роли активировано. **false,** если назначение роли отключено.|
|resultMessage|string|Сообщение результатов, за набором службы.|
|roleId|string|Идентификатор роли. В формате строк GUID.|
|userId|строка|Идентификатор пользователя. В формате строк GUID.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| Только для чтения. Допускается значение null. Связанные сведения о роли.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


