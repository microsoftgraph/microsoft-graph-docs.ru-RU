---
title: Тип ресурса governanceResource
description: Представляет ресурсы, которыми можно управлять с помощью привилегированного управления удостоверениями (PIM). Для ресурсов Azure может быть подписка, Группа ресурсов и ресурс, такой как виртуальная машина, база данных SQL и т. д.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28af0f6ca55881bd0f0848cda27cfe56bd1d5eb5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497617"
---
# <a name="governanceresource-resource-type"></a>Тип ресурса governanceResource

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурсы, которыми можно управлять с помощью привилегированного управления удостоверениями (PIM). Для ресурсов Azure может быть подписка, Группа ресурсов и ресурс, такой как виртуальная машина, база данных SQL и т. д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | Коллекция [governanceResource](../resources/governanceresource.md)|Перечисление коллекции ресурсов, к которым у запрашивающего есть доступ.|
|[получение](../api/governanceresource-get.md); | [governanceResource](../resources/governanceresource.md) |Чтение свойств и связей объекта ресурса, указанного по идентификатору.|
|[Зарегистрировать](../api/governanceresource-register.md) | |Регистрация неуправляемой подписки Azure или группы управления для службы управления информационными данными. |

Нет `POST`, `PUT`, `PATCH`, `DELETE` поддерживаются в `roleDefinitions` наборе сущностей в настоящее время.

## <a name="properties"></a>Свойства
| Свойство          |Тип         |Описание|
|:------------------|:----------|:----------|
|id                 |String     |Идентификатор ресурса. Он указан в формате GUID.|
|externalId           |String   |Внешний идентификатор ресурса, представляющий его исходный идентификатор во внешней системе. Например, внешний идентификатор ресурса подписки может иметь значение "/Subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac". |
|type               |String     |Обязательный. Тип ресурса. Например, для ресурсов Azure типом может быть "Subscription", "ResourceGroup", "Microsoft. SQL/Server" и т. д.|
|displayName        |Строка     |Отображаемое имя ресурса.|
|status             |String     |Состояние данного ресурса. Например, он может представлять, заблокирован ли ресурс (значения: `Active` / `Locked`). Примечание: это свойство может быть расширено в будущем для поддержки дополнительных сценариев.|
|регистереддатетиме|DateTimeOffset      |Представляет дату и время, когда ресурс регистрируется в PIM.|
|регистередрут|String      |Екстерналид из корневой области ресурса, зарегистрированной в PIM. В качестве корневой области можно указать родительские, бабушке или более поздние ресурсы предков.|
|ролеассигнменткаунт|Int32      |Необязательный. Число назначений ролей для данного ресурса. Чтобы получить свойство, используйте `$select=roleAssignmentCount` експликтли в запросе.|
|роледефинитионкаунт|Int32      |Необязательный. Количество определений ролей для данного ресурса. Чтобы получить свойство, используйте `$select=roleDefinitionCount` експликтли в запросе.|
|permissions|[governancePermission](../resources/governancepermission.md)      |Необязательное свойство. Он представляет состояние доступа запрашивающего к ресурсу. Чтобы получить свойство, используйте `$select=permissions` експликтли в запросе.|

## <a name="relationships"></a>Связи
| Связь   | Тип                                         |Описание|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)|Коллекция назначений ролей для ресурса.|
|roleDefinitions |Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)|Коллекция ролей дефинтионс для ресурса.|
|ролеассигнментрекуестс |Коллекция [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Коллекция запросов назначений ролей для ресурса.|
|ролесеттингс |Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)|Коллекция параметров роли для ресурса.|
|верхнего          |[governanceResource](../resources/governanceresource.md)           |Только для чтения. Родительский ресурс. для `pimforazurerbac` сценария может представлять подписку, к которой относится ресурс.|

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
