---
title: Тип ресурса directoryAudit
description: Описывает ресурс Директоряудит (Entity) API Microsoft Graph (REST), который помогает выполнять аудит действий с каталогом (клиентом) (бета-версия).
author: SarahBar
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 82093afe35ec5c89158d72c2d3ce80d82770419b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217286"
---
# <a name="directoryaudit-resource-type"></a>Тип ресурса directoryAudit

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элементы аудита каталога и его коллекцию.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |Перечисление элементов аудита каталога в коллекции и их свойства.|
|[Получение directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |Получение определенного элемента аудита каталога и его свойств.|


## <a name="properties"></a>Свойства
| Свойство            | Тип                                                | Описание                                                                                                                                                                                                                                                            |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| activityDateTime    | DateTimeOffset                                      | Указывает дату и время выполнения действия. Тип Timestamp всегда представлен в формате времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.                                                                              |
| activityDisplayName | String                                              | Указывает имя действия или операции (например, "Создание пользователя", "Добавление участника в группу"). Список действий, регистрируемых в журнале, можно найти в [списке действий Azure AD](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list). |
| additionalDetails   | Коллекция [keyValue](keyvalue.md)                  | Указывает дополнительные сведения о действии.                                                                                                                                                                                                                          |
| category            | String                                              | Указывает, для какой категории ресурса предназначено действие. (Пример: управление пользователями, управление группами и т. д.)                                                                                                                                              |
| correlationId       | GUID                                                | Указывает уникальный идентификатор, помогающий соотносить действия, происходящие в различных службах. Можно использовать для отслеживания журналов в службах.                                                                                                                                    |
| id                  | String                                              | Указывает уникальный идентификатор для действия. Это идентификатор GUID.                                                                                                                                                                                                              |
| initiatedBy         | [auditActivityInitiator](auditactivityinitiator.md) | Указывает сведения о пользователе или приложении, запустившем действие.                                                                                                                                                                                                    |
| loggedByService     | String                                              | Указывает, в какой службе запущено действие (например: самостоятельное управление паролями, основной каталог, B2C, приглашенные пользователи, Microsoft Identity Manager, Privileged Identity Management).                                                          |
| result              | string                                              | Указывает результат действия. Возможные значения: `success`, `failure`, `timeout`, `unknownFutureValue`.                                                                                                                                                       |
| resultReason        | String                                              | Указывает причину сбоя, если результатом является Failure (Сбой) или timeout (время ожидания).                                                                                                                                                                                              |
| targetResources     | Коллекция [targetResource](targetresource.md)      | Указывает, какой ресурс был изменен в результате действия. Возможные типы целевых ресурсов: User, Device, Directory, App, Role, Group, Policy или Other.                                                                                                       |

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
  "result": "string",
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


