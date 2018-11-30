---
title: Тип ресурса governanceRoleDefinition
description: Представляет определения ролей. Для Azure ресурсов может представлять роли Azure RBAC, такие как владелец, чтения, участник, и т.д.
ms.openlocfilehash: 057d74276b41abad47eb60ce48a99f1160c401ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076447"
---
# <a name="governanceroledefinition-resource-type"></a>Тип ресурса governanceRoleDefinition

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается. 


Представляет определения ролей. Для Azure ресурсов может представлять роли Azure RBAC, такие как владелец, чтения, участник, и т.д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) коллекции |Список коллекцию определений ролей для ресурса.|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Чтение свойства и связи с указанным идентификатором сущности определения роли.|
Не `POST`, `PUT`, `PATCH`, `DELETE` поддерживается на `roleDefinitions` набора сущностей в данный момент.
## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----|:----------|:----------|:----------|
|id         |String     |Идентификатор определения роли. |
|resourceId |String     |Обязательно. Идентификатор ресурса, связанного с определением роли. |
|externalId   |String     |Внешний идентификатор определения роли.|
|displayName|String     |Отображаемое имя определения роли.|
|subjectCount|Int32     |Необязательный атрибут. Число субъектов, которые были им назначены роли. Он представляет состояние запрашивающего доступ к ресурсу. Чтобы получить свойство, рекомендуется использовать явным образом `$select=subjectCount` в запросе.|
|eligibleAssignmentCount|Int32|Необязательный атрибут. Число назначений подходящими ролей, связанных с определением роли. Чтобы получить свойство, рекомендуется использовать явным образом `$select=eligibleAssignmentCount` в запросе.|
|activeAssignmentCount|Int32    |Необязательный атрибут. Число назначений active ролей, связанных с определением роли.  Чтобы получить свойство, рекомендуется использовать явным образом `$select=activeAssignmentCount` в запросе.|


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