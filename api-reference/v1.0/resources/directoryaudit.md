---
title: Тип ресурса directoryAudit
description: Представляет элементы аудита каталога и его коллекцию.
author: SarahBar
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 749fd5e525848cadece6b6ed5272057bc7c225eb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337448"
---
# <a name="directoryaudit-resource-type"></a>Тип ресурса directoryAudit

Пространство имен: microsoft.graph

Представляет элементы аудита каталога и его коллекцию.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |Перечисление элементов аудита каталога в коллекции и их свойства.|
|[Получение directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |Получение определенного элемента аудита каталога и его свойств.|

## <a name="properties"></a>Свойства

| Свойство            | Тип                                                | Описание                                                                                                                                                                                                                                                                        |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| activityDateTime    | DateTimeOffset                                      | Указывает дату и время выполнения действия. Тип Timestamp всегда представлен в формате времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.                                                                                          |
| activityDisplayName | String                                              | Указывает имя действия или имя операции (примеры: "Создание пользователя" и "Добавление участника в группу"). Полный список см. в [списке действий Azure AD](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list). |
| additionalDetails   | Коллекция [keyValue](keyvalue.md)                  | Указывает дополнительные сведения о действии.                                                                                                                                                                                                                                      |
| category            | String                                              | Указывает, для какой категории ресурса предназначено действие. (Пример: управление пользователями, управление группами и т. д.)                                                                                                                                                          |
| correlationId       | Guid                                                | Указывает уникальный идентификатор, помогающий соотносить действия, происходящие в различных службах. Можно использовать для отслеживания журналов в службах.                                                                                                                                                |
| id                  | String                                              | Указывает уникальный идентификатор для действия. Это идентификатор GUID.                                                                                                                                                                                                                          |
| initiatedBy         | [auditActivityInitiator](auditactivityinitiator.md) | Указывает сведения о пользователе или приложении, запустившем действие.                                                                                                                                                                                                                |
| loggedByService     | String                                              | Указывает сведения о том, какая служба инициировала действие (например: `Self-service Password Management`, , `Core Directory`, `Invited Users``B2C`, , `Microsoft Identity Manager`, `Privileged Identity Management`.                                                                      |
| result              | operationResult                                              | Указывает результат действия. Возможные значения: `success`, `failure`, `timeout`, `unknownFutureValue`.                                                                                                                                                                   |
| resultReason        | String                                              | Указывает причину сбоя, если **результат** или `failure` `timeout`.                                                                                                                                                                                                                                 |
| targetResources     | Коллекция [targetResource](targetresource.md)      | Указывает, какой ресурс был изменен в результате действия. Тип целевого ресурса может быть , , , , , `Role`или `Other``Group``Policy` . `App``Directory``Device``User`                                                                                                                   |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryAudit"
}-->

```json
{
  "activityDateTime": "String (timestamp)",
  "activityDisplayName": "String",
  "additionalDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "category": "String",
  "correlationId": "Guid",
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.auditActivityInitiator"},
  "loggedByService": "String",
  "result": "String",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryAudit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
