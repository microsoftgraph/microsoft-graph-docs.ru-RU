---
title: Тип ресурса directoryDefinition
description: Предоставляет механизм синхронизации сведения о каталоге и его объектах.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 77af192ff09cf557eec3e73c1973c4c71dc39a96
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134052"
---
# <a name="directorydefinition-resource-type"></a>Тип ресурса directoryDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет механизм синхронизации сведения о каталоге и его объектах. Этот ресурс сообщает механизму синхронизации, например, что каталог имеет объекты с именем **user** и **group,** какие атрибуты поддерживаются для этих объектов, а также типы этих атрибутов. Чтобы объект и атрибут участвовали [](synchronization-synchronizationrule.md) в правилах синхронизации и сопоставлениях [объектов,](synchronization-objectmapping.md)их необходимо определить как часть определения каталога.

Как правило, [](synchronization-synchronizationschema.md) схема синхронизации по умолчанию, [](synchronization-synchronizationtemplate.md) предоставляемая в рамках шаблона синхронизации, определяет наиболее часто используемые объекты и атрибуты для этого каталога. Однако если каталог поддерживает добавление настраиваемого атрибута, может потребоваться расширить определение по умолчанию с помощью собственных настраиваемые объекты или атрибуты. Дополнительные сведения см. в подстройке ["Настройка](synchronization-configure-with-custom-target-attributes.md) синхронизации с настраиваемой атрибутами" и "Настройка синхронизации с атрибутами [расширения каталога".](synchronization-configure-with-directory-extension-attributes.md)

Определения каталогов обновляются в рамках схемы [синхронизации.](synchronization-synchronizationschema.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Обнаружение directoryDefinition](../api/directorydefinition-discover.md) | [directoryDefinition](synchronization-directorydefinition.md) |Обнаружение схемы и поддерживаемых свойств каталога.|

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|id           |Строка     |Идентификатор каталога. Значение null не допускается.|
|метаданные       |Коллекция metadataEntry    |Дополнительные свойства расширения. Если не было явно упомянуто, значения метаданных не следует менять.|
|name           |String     |Имя каталога. Должен быть уникальным в [схеме синхронизации.](synchronization-synchronizationschema.md) Значение null не допускается.|
|objects        |[Коллекция objectDefinition](synchronization-objectdefinition.md)    |Коллекция объектов, поддерживаемых каталогом.|
|version|String|Только для чтения значения, которое указывает обнаруженную версию. NULL, если обнаружение еще не произошло.|
|discoveryDateTime|DateTimeOffset| Представляет дату и время обнаружения в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|discoverabilities|string| Только для чтения, указывающее тип обнаружения, поддерживаемого приложением. Возможные значения: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.| 

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "discoverabilities": "String",
  "discoveryDateTime": "DateTimeOffset",
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}],
  "version": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


