---
title: тип ресурса provisioningObjectSummary
description: Представляет действие, выполняемые службой подготовка Azure AD и связанными с ней свойствами.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2bfe519d6a5cab816bdd35da451221be58105e37
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719404"
---
# <a name="provisioningobjectsummary-resource-type"></a>тип ресурса provisioningObjectSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, выполняемые службой подготовка Azure AD и связанными с ней свойствами. 

## <a name="methods"></a>Методы

| Метод  | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список provisioningObjectSummary](../api/provisioningobjectsummary-list.md) | [provisioningObjectSummary](provisioningobjectsummary.md) | Получите список всех событий, которые произошли в клиенте. |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|action|String|Указывает имя действия или имя операции (например, Создание пользователя, добавление участника в группу). Список действий, зарегистрированных в журнале, обратитесь к списку действий Azure AD.|
|activityDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|changeId|String|Уникальный ID этого изменения в этом цикле.|
|cycleId|String|Уникальный ID для итерации задания.|
|durationInMilliseconds|Int32|Указывает, сколько времени потребовалось для завершения этого действия по подготовкам. Измеряется в миллисекунд.|
|id|String| Указывает уникальный идентификатор для действия. Это GUID только для чтения.|
|initiatedBy|[initiator](initiator.md)|Сведения о том, кто инициировал это подготовка.|
|jobId|String|Уникальный ID для всего задания по подготовкам.|
|modifiedProperties|[измененная коллекцияProperty](modifiedproperty.md)|Сведения о каждом свойстве, которое было изменено в этом действии по обеспечению этого объекта.|
|provisioningSteps|[provisioningStep](provisioningstep.md) collection|Сведения о каждом шаге в области подготовка.|
|servicePrincipal|Коллекция [servicePrincipal](serviceprincipal.md)|Представляет принцип службы, используемый для обеспечения.|
|sourceIdentity|[provisionedIdentity](provisionedidentity.md)|Сведения о предварительном предоставлении объекта-источника.|
|sourceSystem|[provisioningSystemDetails](provisioningsystemdetails.md)|Сведения о исходных системах объекта, который был закамут.|
|statusInfo|[statusBase](statusbase.md)|Сведения о состоянии подготовка.|
|targetIdentity|[provisionedIdentity](provisionedidentity.md)|Сведения о предварительном предоставлении целевого объекта.|
|targetSystem|[provisioningSystemDetails](provisioningsystemdetails.md)|Сведения о целевой системе объекта.|
|tenantId|String|Уникальный ID клиента Azure AD.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "keyProperty": "id"
}-->

```json
{
  "action": "String",
  "activityDateTime": "String (timestamp)",
  "changeId": "String",
  "cycleId": "String",
  "durationInMilliseconds": 1024,
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.initiator"},
  "jobId": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}],
  "provisioningSteps": [{"@odata.type": "microsoft.graph.provisioningStep"}],
  "servicePrincipal": [{"@odata.type": "microsoft.graph.provisioningServicePrincipal"}],
  "sourceIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
  "statusInfo": {"@odata.type": "microsoft.graph.statusBase"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
  "tenantId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningObjectSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


