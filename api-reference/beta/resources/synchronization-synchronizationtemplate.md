---
title: Тип ресурса synchronizationTemplate
description: Предоставляет предварительно настроенные параметры синхронизации для конкретного приложения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c08f5c3eee6225a1149ff993415f83b2e5916583
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132309"
---
# <a name="synchronizationtemplate-resource-type"></a>Тип ресурса synchronizationTemplate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет предварительно настроенные параметры синхронизации для конкретного приложения. Эти параметры будут использоваться по умолчанию для [любого](synchronization-synchronizationjob.md) задания синхронизации, основанного на шаблоне. Разработчик приложения определяет шаблон; Любой может получить шаблон, чтобы увидеть параметры по умолчанию, включая схему [синхронизации.](synchronization-synchronizationschema.md)

Для приложения можно предоставить несколько шаблонов и назначить шаблон по умолчанию. Если для интересуемого приложения доступно несколько шаблонов, обратитесь к конкретным приложениям, чтобы определить, какой из них лучше всего соответствует вашим потребностям.

## <a name="methods"></a>Методы

| Метод        | Возвращаемый тип               | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|[Список](../api/synchronization-synchronizationtemplate-list.md)    |[Коллекция synchronizationTemplate](synchronization-synchronizationtemplate.md)  |Список шаблонов, доступных для экземпляра приложения или приложения (участников-служб).|
|[Get](../api/synchronization-synchronizationtemplate-get.md)      |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Чтение свойств и связей объекта **synchronizationTemplate.**|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>Свойства

| Свойство      | Тип                      | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |Строка                     |Уникальный идентификатор шаблона.|
|applicationId  |String                     |Идентификатор приложения, к которой принадлежит этот шаблон.|
|default        |Boolean                    |`true` если этот шаблон рекомендуется использовать по умолчанию для приложения.|
|description    |Строка                     |Описание шаблона.|
|обнаруживаемый   |Строка                     |`true` если этот шаблон должен отображаться в коллекции шаблонов, доступных для экземпляра приложения (основного приложения-службы).|
|factoryTag     |Строка                     |Один из известных заводских тегов, поддерживаемых механизмом синхронизации. FactoryTag **сообщает** механизму синхронизации, какую реализацию использовать при обработке заданий на основе этого шаблона.|
|метаданные       |Коллекция metadataEntry   |Дополнительные свойства расширения. Если не было явно упомянуто, значения метаданных не следует менять.|

## <a name="relationships"></a>Связи
| Связь      | Тип      |Описание|
|:------------------|:----------|:----------|
|схема             |[synchronizationSchema](synchronization-synchronizationschema.md)     |Схема синхронизации по умолчанию для заданий, основанных на этом шаблоне.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}-->

```json
{
  "applicationId": "String (identifier)",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "id": "String (identifier)",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "schema": {"@odata.type": "microsoft.graph.synchronizationSchema"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


