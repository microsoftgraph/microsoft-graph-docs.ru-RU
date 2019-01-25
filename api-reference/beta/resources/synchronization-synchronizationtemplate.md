---
title: Тип ресурса synchronizationTemplate
description: " всем пользователям можно извлечь шаблон, чтобы увидеть параметры по умолчанию, включая схемы синхронизации."
localization_priority: Normal
ms.openlocfilehash: 75df13d55cfb58aafe8a751279e103424aa29367
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516555"
---
# <a name="synchronizationtemplate-resource-type"></a>Тип ресурса synchronizationTemplate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет параметры предварительно настроенным синхронизации для конкретного приложения. Эти параметры будет использоваться по умолчанию для каждого [задания синхронизации](synchronization-synchronizationjob.md) , основанный на шаблоне. Разработчик приложений задает шаблон; всем пользователям можно извлечь шаблон, чтобы увидеть параметры по умолчанию, включая [схемы синхронизации](synchronization-synchronizationschema.md).

Предоставление нескольких шаблонов для приложения и назначить шаблон по умолчанию. Если приложение, которое вы хотите несколько шаблонов, seek инструкции для определения, какой из них лучше всего соответствует потребностям приложения.

## <a name="methods"></a>Методы

| Метод        | Возвращаемый тип               | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |[synchronizationTemplate](synchronization-synchronizationtemplate.md) коллекции  |Список шаблонов, доступных для приложения или экземпляра приложения (участников-служб).|
|[Get](../api/synchronization-synchronizationtemplate-get.md)      |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Чтение свойства и связи объекта **synchronizationTemplate** .|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>Свойства

| Свойство      | Тип                      | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |String                     |Шаблон уникальный идентификатор.|
|applicationId  |String                     |Идентификатор приложения, к которому принадлежит этот шаблон.|
|по умолчанию        |Логическое                    |`true`Если этот шаблон рекомендуется по умолчанию для приложения.|
|description    |String                     |Описание шаблона.|
|обнаруживаемые   |String                     |`true`Если этот шаблон должен отображаться в коллекцию шаблонов, доступных для экземпляра приложения (участников-служб).|
|factoryTag     |String                     |Один из известных фабрики тегов, поддерживаемые обработчиком синхронизации. **FactoryTag** сообщает о том, обработчик синхронизации реализация для использования при обработке задания на основе этого шаблона.|
|Метаданные       |metadataEntry коллекции   |Расширение дополнительные свойства. Если не указан явно, значения метаданных не должно изменяться.|

## <a name="relationships"></a>Отношения
| Связь      | Тип      |Описание|
|:------------------|:----------|:----------|
|схема             |[synchronizationSchema](synchronization-synchronizationschema.md)     |Схема синхронизации по умолчанию для заданий на основе этого шаблона.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
