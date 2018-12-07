---
title: Тип ресурса governanceRoleAssignment
description: Представляет назначения пользователя или группы на роль.
ms.openlocfilehash: 3b0520f4641c961358b2db990914fbdf8de254f8
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191139"
---
# <a name="governanceroleassignment-resource-type"></a>Тип ресурса governanceRoleAssignment
> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет назначения пользователя или группы на роль.

Управление правами Identity (PIM) поддерживает два типа назначения.

1. Активное назначение — предоставляет доступ/активирован непосредственно к ресурсам.
2. Допустимость назначения — представляет промежуточного этапа привилегированный доступ к ресурсам между нет доступа и прямой доступ. Администраторы могут назначать пользователей и групп для `eligible assignment` заранее, а каждый раз, когда требуется доступ, `activation` на `eligible assignment` необходим для получения быстрого доступа к ресурсу для нескольких часов. После активации `active assignment` будут создаваться заинтересованных пользователей и групп для указания состояния активации.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:------------|:--------|:--------|
|[Получение](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |Чтение свойства и связи объекта назначения ролей.|
|[List](../api/governanceroleassignment-list.md) | [governanceRoleAssignment](../resources/governanceroleassignment.md) коллекции|Список коллекции назначения ролей для ресурса. |
|[Экспорт](../api/governanceroleassignment-export.md) | потока октетов |Загрузите набор из назначения ролей для ресурса и сохранить как `.csv` файла.|

Не `POST`, `PUT`, `PATCH`, или `DELETE` поддерживается на `roleAssignments` набора сущностей. Любой создание, обновление и удаление операций на `governanceRoleAssignment` выполнить по `governanceRoleAssignmentRequest`.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |Строка     |Идентификатор назначения ролей. Это в формате GUID.|
|resourceId |Строка     |Обязательный. Идентификатор ресурса, назначения ролей, связанный с. |
|roleDefinitionId|Строка|Обязательный. Идентификатор определения роли, назначения ролей, связанный с. |
|subjectId|Строка       |Обязательный. Идентификатор субъекта, назначения ролей, связанный с. |
|linkedEligibleRoleAssignmentId|Строка|Если это `active assignment` и создано из-за активации на `eligible assignment`, представляющий идентификатор, который `eligible assignment`; В противном случае — значение `null`. |
|externalId   |String     |Внешний идентификатор ресурса, используемый для идентификации назначения роли в поставщик.|
|startDateTime|DateTimeOffset|Время начала назначения ролей. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|endDateTime|DateTimeOffset|Назначение ролей не постоянная — это время, когда срока действия назначения ролей. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|assignmentState|Строка  |Состояние назначения. Значение может быть <ul><li> `Eligible`для подходящими назначения</li><li> `Active`-Если она назначена непосредственно `Active` администраторами, или активируемого на допустимость назначения для пользователей.</li></ul>|
|memberType|Строка      |Тип элемента. Значение может быть: <ul><li>`Inherited`-Назначение ролей наследуется от родительской области ресурсов</li><li>`Group`-назначения ролей не наследуется, но, поступающие из членства Назначение группы</li><li>`User`-не наследуется назначения ролей, ни из Назначение группы.</li></ul>|


## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Ресурс, связанный с назначения ролей. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, связанные с назначения ролей. |
|subject|[governanceSubject](../resources/governancesubject.md)|Только для чтения. Тема, связанная с назначения ролей. |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Только для чтения. Если это `active assignment` и создано из-за активации на `eligible assignment`, представляющий объект, который `eligible assignment`; В противном случае — значение `null`. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
