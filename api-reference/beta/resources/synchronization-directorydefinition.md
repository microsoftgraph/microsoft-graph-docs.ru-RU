---
title: тип ресурса directoryDefinition
description: Предоставляет сведения о каталоге и его объектах в движке синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 8e3adb4679233fa35a53574b6f8d0c2b806be110
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956801"
---
# <a name="directorydefinition-resource-type"></a>тип ресурса directoryDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о каталоге и его объектах в движке синхронизации. Этот ресурс сообщает механизму синхронизации, например, что в каталоге есть объекты с именем **пользователя** и **группы,** атрибуты которых поддерживаются для этих объектов, и типы для этих атрибутов. Чтобы объект и атрибут участвовали [](synchronization-synchronizationrule.md) в правилах синхронизации и сопоставлениях [объектов,](synchronization-objectmapping.md)их необходимо определить как часть определения каталога.

Как правило, [](synchronization-synchronizationschema.md) схема синхронизации по умолчанию, [](synchronization-synchronizationtemplate.md) предоставляемая в рамках шаблона синхронизации, будет определять наиболее часто используемые объекты и атрибуты для этого каталога. Однако если каталог поддерживает добавление настраиваемого атрибута, может потребоваться расширить определение по умолчанию с помощью собственных настраиваемых объектов или атрибутов. Дополнительные сведения см. в [рублях Настройка](synchronization-configure-with-custom-target-attributes.md) синхронизации с пользовательскими атрибутами и настройка синхронизации с атрибутами [расширения каталогов.](synchronization-configure-with-directory-extension-attributes.md)

Определения каталогов обновляются в рамках схемы [синхронизации.](synchronization-synchronizationschema.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Обнаружение directoryDefinition](../api/directorydefinition-discover.md) | [directoryDefinition](synchronization-directorydefinition.md) |Откройте схему и поддерживаемые свойства каталога.|

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|id           |Строка     |Идентификатор Directory. Значение null не допускается.|
|метаданные       |коллекция metadataEntry    |Дополнительные свойства расширения. Если не упомянуть явно, значения метаданных не следует менять.|
|name           |String     |Имя каталога. Должна быть уникальной в [схеме синхронизации.](synchronization-synchronizationschema.md) Значение null не допускается.|
|объекты        |[коллекция objectDefinition](synchronization-objectdefinition.md)    |Коллекция объектов, поддерживаемых каталогом.|
|version|String|Чтение только значения, которое указывает обнаруженную версию. `null` если обнаружение еще не произошло.|
|discoveryDateTime|DateTimeOffset| Представляет дату и время обнаружения с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|discoverabilities|directoryDefinitionDiscoverabilities| Прочитайте только значение, указывающее тип обнаружения, поддерживаемого приложением. Возможные значения: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.| 

## <a name="json-representation"></a>Представление JSON

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


