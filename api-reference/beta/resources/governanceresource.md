---
title: тип ресурсов governanceResource
description: Представляет ресурсы, которыми может управлять управление привилегированными пользователями (PIM). Для ресурсов Azure это может быть подписка, группа ресурсов и такие ресурсы, как виртуальная машина, SQL базы данных и т.д.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: 5eacdb75d6607827eaf288b3eed17d41cce07f66
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510564"
---
# <a name="governanceresource-resource-type"></a>тип ресурсов governanceResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Представляет ресурсы, которыми может управлять управление привилегированными пользователями (PIM). Для ресурсов Azure это может быть подписка, группа ресурсов и такие ресурсы, как виртуальная машина, SQL базы данных и т.д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:----------|
|[Список](../api/governanceresource-list.md) | [коллекция governanceResource](../resources/governanceresource.md)|Перечислить коллекцию ресурсов, к которые имеет доступ запросчик.|
|[Получение](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |Чтение свойств и связей объекта ресурсов, указанного в id.|
|[Регистрация](../api/governanceresource-register.md) | |Зарегистрируйте неуправленную подписку или группу управления Azure в службу PIM. |

Нет`POST`, `PUT`поддерживаются `DELETE` `PATCH`в наборе `roleDefinitions` сущности на данный момент.

## <a name="properties"></a>Свойства
| Свойство          |Тип         |Описание|
|:------------------|:----------|:----------|
|id                 |Строка     |Id ресурса. Он находится в формате GUID.|
|externalId           |String   |Внешний id ресурса, представляющий его исходный id во внешней системе. Например, внешний id ресурса подписки может быть "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac". |
|type               |Строка     |Обязательный. Тип ресурса. Например, для ресурсов Azure тип может быть "Подписка", "ResourceGroup", "Microsoft.Sql/server" и т.д.|
|displayName        |Строка     |Имя отображения ресурса.|
|status             |String     |Состояние данного ресурса. Например, он может представлять, заблокирован ресурс или нет (значения: `Active`/`Locked`). Примечание. Это свойство может быть расширено в будущем, чтобы поддерживать дополнительные сценарии.|
|registeredDateTime|DateTimeOffset      |Представляет время даты регистрации ресурса в PIM.|
|registeredRoot|Строка      |ExternalId корневой области ресурса, зарегистрированной в PIM. Корневой областью могут быть родительские, бабушки и дедушки или более высокие ресурсы предка.|
|roleAssignmentCount|Int32      |Необязательный. Количество назначений ролей для данного ресурса. Чтобы получить свойство, используйте его в `$select=roleAssignmentCount` запросе.|
|roleDefinitionCount|Int32      |Необязательный. Количество определений ролей для данного ресурса. Чтобы получить свойство, используйте его в `$select=roleDefinitionCount` запросе.|
|permissions|[governancePermission](../resources/governancepermission.md)      |Необязательно. Он представляет состояние доступа запросителя к ресурсу. Чтобы получить свойство, используйте его в `$select=permissions` запросе.|

## <a name="relationships"></a>Связи
| Связь   | Тип                                         |Описание|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[коллекция governanceRoleAssignment](../resources/governanceroleassignment.md)|Коллекция назначений ролей для ресурса.|
|roleDefinitions |[коллекция governanceRoleDefinition](../resources/governanceroledefinition.md)|Коллекция defintions роли для ресурса.|
|roleAssignmentRequests |[коллекция governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Коллекция запросов на назначение ролей для ресурса.|
|roleSettings |[коллекция governanceRoleSetting](../resources/governancerolesetting.md)|Коллекция параметров ролей для ресурса.|
|родитель          |[governanceResource](../resources/governanceresource.md)           |Только для чтения. Родительский ресурс. для `pimforazurerbac` сценария он может представлять подписку, к которой принадлежит ресурс.|

## <a name="json-representation"></a>Представление JSON

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


