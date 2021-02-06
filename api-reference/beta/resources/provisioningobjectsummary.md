---
title: Тип ресурса provisioningObjectSummary
description: Представляет действие, выполняемые службой предоставления Azure AD, и связанные с ней свойства.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e51a3a5e184fae0c5c35e01b5a0b23494f63edc7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135375"
---
# <a name="provisioningobjectsummary-resource-type"></a>Тип ресурса provisioningObjectSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, выполняемые службой предоставления Azure AD, и связанные с ней свойства. 

## <a name="methods"></a>Методы

| Метод  | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список provisioningObjectSummary](../api/provisioningobjectsummary-list.md) | [provisioningObjectSummary](provisioningobjectsummary.md) | Получите список всех событий предоставления, произошедших в клиенте. |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|action|Строка|Указывает имя действия или имя операции (например, "Создать пользователя", "Добавить участника в группу"). Список зарегистрированных действий можно найти в списке действий Azure AD.|
|activityDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|changeId|Строка|Уникальный ИД этого изменения в этом цикле.|
|cycleId|Строка|Уникальный ИД для итерации задания.|
|durationInMilliseconds|Int32|Указывает, сколько времени потребовалось для завершения этого действия. Измеряется в миллисекунах.|
|id|String| Указывает уникальный идентификатор для действия. Это GUID только для чтения.|
|initiatedBy|[initiator](initiator.md)|Сведения о том, кто инициировал эту подготовка.|
|jobId|Строка|Уникальный ИД для всего задания по обеспечению.|
|modifiedProperties|[Коллекция modifiedProperty](modifiedproperty.md)|Сведения о каждом свойстве, которое было изменено в этом действии по обеспечению этого объекта.|
|provisioningSteps|[Коллекция provisioningStep](provisioningstep.md)|Подробные сведения о каждом шаге в предоставлении.|
|servicePrincipal|Коллекция [servicePrincipal](serviceprincipal.md)|Представляет основной сервис, используемый для предоставления.|
|sourceIdentity|[provisionedIdentity](provisionedidentity.md)|Сведения о объекте-источнике, который необходимо подготовка.|
|sourceSystem|[provisioningSystemDetails](provisioningsystemdetails.md)|Сведения об источнике системы для объекта, который необходимо подготовка.|
|statusInfo|[statusBase](statusbase.md)|Сведения о состоянии предоставления.|
|targetIdentity|[provisionedIdentity](provisionedidentity.md)|Сведения о подготовках целевого объекта.|
|targetSystem|[provisioningSystemDetails](provisioningsystemdetails.md)|Сведения о целевой системе для объекта, который необходимо подготовка.|
|tenantId|String|Уникальный ИД клиента Azure AD.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "baseType": "",
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


