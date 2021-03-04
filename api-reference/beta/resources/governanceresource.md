---
title: тип ресурсов governanceResource
description: Представляет ресурсы, которыми может управлять привилегированное управление удостоверениями (PIM). Для ресурсов Azure это может быть подписка, группа ресурсов и такие ресурсы, как виртуальная машина, SQL базы данных и т.д.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e0cf42593a35103996217d1ce18bd9938b48a185
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443119"
---
# <a name="governanceresource-resource-type"></a>тип ресурсов governanceResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурсы, которыми может управлять привилегированное управление удостоверениями (PIM). Для ресурсов Azure это может быть подписка, группа ресурсов и такие ресурсы, как виртуальная машина, SQL базы данных и т.д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:----------|
|[Список](../api/governanceresource-list.md) | [коллекция governanceResource](../resources/governanceresource.md)|Перечислить коллекцию ресурсов, к которые имеет доступ запросчик.|
|[получение](../api/governanceresource-get.md); | [governanceResource](../resources/governanceresource.md) |Чтение свойств и связей объекта ресурсов, указанного в id.|
|[Зарегистрировать](../api/governanceresource-register.md) | |Зарегистрируйте неуправленную подписку или группу управления Azure в службу PIM. |

`POST`Нет, `PUT` `PATCH` `DELETE` поддерживаются в `roleDefinitions` наборе сущности на данный момент.

## <a name="properties"></a>Свойства
| Свойство          |Тип         |Описание|
|:------------------|:----------|:----------|
|id                 |String     |Id ресурса. Он находится в формате GUID.|
|externalId           |String   |Внешний id ресурса, представляющий его исходный id во внешней системе. Например, внешний id ресурса подписки может быть "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac". |
|type               |String     |Обязательный. Тип ресурса. Например, для ресурсов Azure тип может быть "Подписка", "ResourceGroup", "Microsoft.Sql/server" и т.д.|
|displayName        |String     |Имя отображения ресурса.|
|status             |String     |Состояние данного ресурса. Например, он может представлять, заблокирован ресурс или нет (значения: `Active` / `Locked` ). Примечание. Это свойство может быть расширено в будущем, чтобы поддерживать дополнительные сценарии.|
|registeredDateTime|DateTimeOffset      |Представляет время даты регистрации ресурса в PIM.|
|registeredRoot|String      |ExternalId корневой области ресурса, зарегистрированной в PIM. Корневой областью могут быть родительские, бабушки и дедушки или более высокие ресурсы предка.|
|roleAssignmentCount|Int32      |Необязательный. Количество назначений ролей для данного ресурса. Чтобы получить свойство, используйте его в `$select=roleAssignmentCount` запросе.|
|roleDefinitionCount|Int32      |Необязательный. Количество определений ролей для данного ресурса. Чтобы получить свойство, используйте его в `$select=roleDefinitionCount` запросе.|
|permissions|[governancePermission](../resources/governancepermission.md)      |Необязательное. Он представляет состояние доступа запросителя к ресурсу. Чтобы получить свойство, используйте его в `$select=permissions` запросе.|

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


