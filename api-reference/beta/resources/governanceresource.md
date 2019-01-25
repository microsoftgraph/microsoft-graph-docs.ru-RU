---
title: Тип ресурса governanceResource
description: Представляет ресурсы, которые может осуществляться по управления правами Identity (PIM). Azure ресурсах может быть подписки, группы ресурсов и ресурсов, таких как виртуальную машину, базы данных SQL, и т.д.
localization_priority: Normal
ms.openlocfilehash: 92a738350a47cc9eaf436382d020330fac89db1f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528559"
---
# <a name="governanceresource-resource-type"></a>Тип ресурса governanceResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурсы, которые может осуществляться по управления правами Identity (PIM). Azure ресурсах может быть подписки, группы ресурсов и ресурсов, таких как виртуальную машину, базы данных SQL, и т.д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | [governanceResource](../resources/governanceresource.md) коллекции|Список коллекцию ресурсов, которыми запрашивающего доступ к.|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |Чтение свойства и связи с указанным идентификатором сущности ресурсов.|
|Регистрация | |Зарегистрируйте неуправляемые Azure подписки или управление группу для службы управления персональными данными. |

Не `POST`, `PUT`, `PATCH`, `DELETE` поддерживаются в `roleDefinitions` набора сущностей в данный момент.

## <a name="properties"></a>Свойства
| Свойство          |Тип         |Описание|
|:------------------|:----------|:----------|
|id                 |String     |Идентификатор ресурса. Это в формате GUID.|
|externalId           |String   |Внешний идентификатор ресурса, представляющее его исходный идентификатор во внешней системе. Например ресурсов подписки внешний идентификатор может быть «/ подписок/c14ae696-5e0c-4e5d-88cc-bef6637737ac». |
|type               |Строка     |Обязательный. Тип ресурса Например для Azure ресурсы тип может быть «Подписки», «Группа ресурсов», «Microsoft.Sql/server», и т.д.|
|displayName        |String     |Отображаемое имя ресурса.|
|status             |String     |Состояние указанного ресурса. Например, он может представлять ли ресурс заблокирован или нет (значения: `Active` / `Locked`). Примечание: Это свойство может быть расширен в будущем для поддержки дополнительных сценариев.|
|registeredDateTime|DateTimeOffset      |Представляет при регистрации ресурса в PIM даты и времени.|
|registeredRoot|String      |ExternalId область корневой ресурсов, зарегистрированные в PIM. Область корневой может быть родительский элемент или выше ресурсы предков.|
|roleAssignmentCount|Int32      |Необязательный параметр. Число назначений ролей для указанного ресурса. Чтобы получить свойство, рекомендуется использовать явным образом `$select=roleAssignmentCount` в запросе.|
|roleDefinitionCount|Int32      |Необязательный параметр. Количество определений ролей для указанного ресурса. Чтобы получить свойство, рекомендуется использовать явным образом `$select=roleDefinitionCount` в запросе.|
|permissions|[governancePermission](../resources/governancepermission.md)      |Необязательный параметр. Он представляет состояние запрашивающего доступ к ресурсу. Чтобы получить свойство, рекомендуется использовать явным образом `$select=permissions` в запросе.|

## <a name="relationships"></a>Отношения
| Связь   | Тип                                         |Описание|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md) коллекции|Коллекция назначения ролей для ресурса.|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md) коллекции|Коллекция файлов определения ролей для ресурса.|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) коллекции|Коллекция запросы назначения ролей для ресурса.|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md) коллекции|Коллекция параметров роли для ресурса.|
|Parent          |[governanceResource](../resources/governanceresource.md)           |Только для чтения. Родительский ресурс. для `pimforazurerbac` сценарий, он может представлять подписки, принадлежит ресурс.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceResource"
}-->
```json
{
  "id": "String (identifier)",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
