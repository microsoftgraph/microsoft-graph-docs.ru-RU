---
title: Тип ресурса Провисионингобжектсуммари
description: Представляет действие, выполненное службой подготовки Azure AD и связанными с ним свойствами.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9eabbb0c0cd1cd692ad6ebc5a346c46473161b1
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394605"
---
# <a name="provisioningobjectsummary-resource-type"></a>Тип ресурса Провисионингобжектсуммари

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, выполненное службой подготовки Azure AD и связанными с ним свойствами. 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Провисионингобжектсуммари](../api/provisioningobjectsummary-list.md) | [провисионингобжектсуммари](provisioningobjectsummary.md) | Получение списка всех событий подготовки, произошедших в клиенте. |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|action|String|Указывает имя действия или имя операции (например, создание пользователя, Добавление участника в группу). Список действий, регистрируемых в журнале, можно найти в списке действий Azure AD.|
|activityDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|чанжеид|String|Уникальный идентификатор этого изменения в этом цикле.|
|циклеид|String|Уникальный идентификатор для итерации задания.|
|дуратионинмиллисекондс|Int32|Указывает время завершения этого действия подготовки. Измеряется в миллисекундах.|
|id|String| Указывает уникальный идентификатор для действия. Это GUID, предназначенный только для чтения.|
|initiatedBy|[initiator](initiator.md)|Сведения о том, кто инициировал эту подготовку.|
|jobId|String|Уникальный идентификатор для полного задания подготовки.|
|modifiedProperties|Коллекция [модифиедпроперти](modifiedproperty.md)|Сведения о каждом свойстве, которое было изменено в этом действии подготовки для данного объекта.|
|провисионингстепс|Коллекция [провисионингстеп](provisioningstep.md)|Сведения о каждом этапе подготовки.|
|servicePrincipal|Коллекция [servicePrincipal](serviceprincipal.md)|Представляет участника службы, используемого для подготовки.|
|саурцеидентити|[provisionedIdentity](provisionedidentity.md)|Сведения о подготовленном исходном объекте.|
|саурцесистем|[провисионингсистемдетаилс](provisioningsystemdetails.md)|Сведения об исходной системе подготовленного объекта.|
|статусинфо|[statusBase](statusbase.md)|Сведения о состоянии подготовки.|
|таржетидентити|[provisionedIdentity](provisionedidentity.md)|Сведения о подготовленном целевом объекте.|
|таржетсистем|[провисионингсистемдетаилс](provisioningsystemdetails.md)|Сведения о целевой системе объекта, подготавливается к работе.|
|tenantId|String|Уникальный идентификатор клиента Azure AD.|

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
