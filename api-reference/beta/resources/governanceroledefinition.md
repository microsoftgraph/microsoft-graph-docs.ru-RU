---
title: Тип ресурса governanceRoleDefinition
description: Представляет определения ролей. Для Azure ресурсов может представлять роли Azure RBAC, такие как владелец, чтения, участник, и т.д.
localization_priority: Normal
ms.openlocfilehash: 3f94dd1a741545760951875fbc064307823a65dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842453"
---
# <a name="governanceroledefinition-resource-type"></a>Тип ресурса governanceRoleDefinition

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается. 


Представляет определения ролей. Для Azure ресурсов может представлять роли Azure RBAC, такие как владелец, чтения, участник, и т.д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) коллекции |Список коллекцию определений ролей для ресурса.|
|[получение](../api/governanceroledefinition-get.md); | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Чтение свойства и связи с указанным идентификатором сущности определения роли.|
Не `POST`, `PUT`, `PATCH`, `DELETE` поддерживается на `roleDefinitions` набора сущностей в данный момент.
## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----|:----------|:----------|:----------|
|id         |Строка     |Идентификатор определения роли. |
|resourceId |Строка     |Обязательный. Идентификатор ресурса, связанного с определением роли. |
|externalId   |String     |Внешний идентификатор определения роли.|
|displayName|Строка     |Отображаемое имя определения роли.|
|subjectCount|Int32     |Необязательное. Число субъектов, которые были им назначены роли. Он представляет состояние запрашивающего доступ к ресурсу. Чтобы получить свойство, рекомендуется использовать явным образом `$select=subjectCount` в запросе.|
|eligibleAssignmentCount|Int32|Необязательное. Число назначений подходящими ролей, связанных с определением роли. Чтобы получить свойство, рекомендуется использовать явным образом `$select=eligibleAssignmentCount` в запросе.|
|activeAssignmentCount|Int32    |Необязательное. Число назначений active ролей, связанных с определением роли.  Чтобы получить свойство, рекомендуется использовать явным образом `$select=activeAssignmentCount` в запросе.|


## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Связанные ресурсов для определения роли.|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|Параметр связанных ролей для определения роли.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
