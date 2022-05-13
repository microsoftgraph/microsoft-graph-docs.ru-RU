---
title: Тип ресурса governanceResource
description: Представляет ресурсы, которыми может управлять управление привилегированными пользователями (PIM). Для ресурсов Azure это может быть подписка, группа ресурсов и ресурс, например виртуальная машина, база данных SQL и т. д.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 0be4deb0ae3e96ff1c5a19b7d398ff980c2760ae
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397500"
---
# <a name="governanceresource-resource-type"></a>Тип ресурса governanceResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Представляет ресурсы, которыми может управлять управление привилегированными пользователями (PIM). Для ресурсов Azure это может быть подписка, группа ресурсов и ресурс, например виртуальная машина, база данных SQL и т. д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:----------|
|[Перечисление](../api/governanceresource-list.md) | [Коллекция governanceResource](../resources/governanceresource.md)|Перечисление коллекции ресурсов, к которой у запрашиваемого объекта есть доступ.|
|[Получение](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |Чтение свойств и связей сущности ресурса, указанной идентификатором.|
|[Регистрация](../api/governanceresource-register.md) | |Зарегистрируйте неуправляемую подписку Azure или группу управления в службе PIM. |

Нет `POST`, `PUT`, `PATCH`не поддерживаются `DELETE` в `roleDefinitions` наборе сущностей.

## <a name="properties"></a>Свойства
| Свойство          |Тип         |Описание|
|:------------------|:----------|:----------|
|id                 |String     |Идентификатор ресурса. Он имеет формат GUID.|
|externalId           |String   |Внешний идентификатор ресурса, представляющий его исходный идентификатор во внешней системе. Например, внешний идентификатор ресурса подписки может быть "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac". |
|type               |String     |Обязательный. Тип ресурса. Например, для ресурсов Azure типом может быть "Subscription", "ResourceGroup", "Microsoft.Sql/server" и т. д.|
|displayName        |String     |Отображаемое имя ресурса.|
|status             |String     |Состояние заданного ресурса. Например, он может представлять, заблокирован ли ресурс (значения: `Active`/`Locked`). Примечание. Это свойство может быть расширено в будущем для поддержки дополнительных сценариев.|
|registeredDateTime|DateTimeOffset      |Представляет дату регистрации ресурса в PIM.|
|registeredRoot|String      |ExternalId корневой области ресурса, зарегистрированной в PIM. Корневой областью могут быть родительские, родительские, родительские или более высокие ресурсы-предки.|
|roleAssignmentCount|Int32      |Необязательный. Количество назначений ролей для данного ресурса. Чтобы получить свойство, используйте его в `$select=roleAssignmentCount` запросе.|
|roleDefinitionCount|Int32      |Необязательный. Количество определений ролей для данного ресурса. Чтобы получить свойство, используйте его в `$select=roleDefinitionCount` запросе.|
|permissions|[governancePermission](../resources/governancepermission.md)      |Необязательное. Он представляет состояние доступа запрашиваемого объекта к ресурсу. Чтобы получить свойство, используйте его в `$select=permissions` запросе.|

## <a name="relationships"></a>Связи
| Связь   | Тип                                         |Описание|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[Коллекция governanceRoleAssignment](../resources/governanceroleassignment.md)|Коллекция назначений ролей для ресурса.|
|roleDefinitions |[Коллекция governanceRoleDefinition](../resources/governanceroledefinition.md)|Коллекция назначений ролей для ресурса.|
|roleAssignmentRequests |[Коллекция governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Коллекция запросов на назначение ролей для ресурса.|
|roleSettings |[Коллекция governanceRoleSetting](../resources/governancerolesetting.md)|Коллекция параметров роли для ресурса.|
|родитель          |[governanceResource](../resources/governanceresource.md)           |Только для чтения. Родительский ресурс. Для `pimforazurerbac` сценария он может представлять подписку, к которой принадлежит ресурс.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "registeredRoot": "String",
  "roleAssignmentCount": 12356,
  "roleDefinitionCount": 12356,
  "permissions": {
    "@odata.type": "microsoft.graph.governancePermission"
  }
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
  "suppressions": []
}
-->


