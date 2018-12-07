---
title: Тип ресурса governanceResource
description: Представляет ресурсы, которые может осуществляться по управления правами Identity (PIM). Azure ресурсах может быть подписки, группы ресурсов и ресурсов, таких как виртуальную машину, базы данных SQL, и т.д.
ms.openlocfilehash: 6a048680c3b9bb614287e764d547a20bd09b5d25
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191132"
---
# <a name="governanceresource-resource-type"></a>Тип ресурса governanceResource

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет ресурсы, которые может осуществляться по управления правами Identity (PIM). Azure ресурсах может быть подписки, группы ресурсов и ресурсов, таких как виртуальную машину, базы данных SQL, и т.д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | [governanceResource](../resources/governanceresource.md) коллекции|Список коллекцию ресурсов, которыми запрашивающего доступ к.|
|[получение](../api/governanceresource-get.md); | [governanceResource](../resources/governanceresource.md) |Чтение свойства и связи с указанным идентификатором сущности ресурсов.|
|[Регистрация](../api/governanceresource-register.md) | |Зарегистрируйте неуправляемые Azure подписки или управление группу для службы управления персональными данными. |

Не `POST`, `PUT`, `PATCH`, `DELETE` поддерживаются в `roleDefinitions` набора сущностей в данный момент.

## <a name="properties"></a>Свойства
| Свойство          |Тип         |Описание|
|:------------------|:----------|:----------|
|id                 |Строка     |Идентификатор ресурса. Это в формате GUID.|
|externalId           |String   |Внешний идентификатор ресурса, представляющее его исходный идентификатор во внешней системе. Например ресурсов подписки внешний идентификатор может быть «/ подписок/c14ae696-5e0c-4e5d-88cc-bef6637737ac». |
|type               |Строка     |Обязательный. Тип ресурса. Например для Azure ресурсы тип может быть «Подписки», «Группа ресурсов», «Microsoft.Sql/server», и т.д.|
|displayName        |Строка     |Отображаемое имя ресурса.|
|status             |Строка     |Состояние указанного ресурса. Например, он может представлять ли ресурс заблокирован или нет (значения: `Active` / `Locked`). Примечание: Это свойство может быть расширен в будущем для поддержки дополнительных сценариев.|
|registeredDateTime|DateTimeOffset      |Представляет при регистрации ресурса в PIM даты и времени.|
|registeredRoot|Строка      |ExternalId область корневой ресурсов, зарегистрированные в PIM. Область корневой может быть родительский элемент или выше ресурсы предков.|
|roleAssignmentCount|Int32      |Необязательный атрибут. Число назначений ролей для указанного ресурса. Чтобы получить свойство, рекомендуется использовать явным образом `$select=roleAssignmentCount` в запросе.|
|roleDefinitionCount|Int32      |Необязательный атрибут. Количество определений ролей для указанного ресурса. Чтобы получить свойство, рекомендуется использовать явным образом `$select=roleDefinitionCount` в запросе.|
|permissions|[governancePermission](../resources/governancepermission.md)      |Необязательный атрибут. Он представляет состояние запрашивающего доступ к ресурсу. Чтобы получить свойство, рекомендуется использовать явным образом `$select=permissions` в запросе.|

## <a name="relationships"></a>Связи
| Связь   | Тип                                         |Описание|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md) коллекции|Коллекция назначения ролей для ресурса.|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md) коллекции|Коллекция файлов определения ролей для ресурса.|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) коллекции|Коллекция запросы назначения ролей для ресурса.|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md) коллекции|Коллекция параметров роли для ресурса.|
|родительский          |[governanceResource](../resources/governanceresource.md)           |Только для чтения. Родительский ресурс. для `pimforazurerbac` сценарий, он может представлять подписки, принадлежит ресурс.|

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
