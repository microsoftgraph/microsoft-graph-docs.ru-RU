---
title: Тип ресурса synchronizationTemplate
description: " всем пользователям можно извлечь шаблон, чтобы увидеть параметры по умолчанию, включая схемы синхронизации."
localization_priority: Normal
ms.openlocfilehash: e98d3fa16d0a80ac9353aaa75200d8cb24d3e904
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833077"
---
# <a name="synchronizationtemplate-resource-type"></a>Тип ресурса synchronizationTemplate

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Предоставляет параметры предварительно настроенным синхронизации для конкретного приложения. Эти параметры будет использоваться по умолчанию для каждого [задания синхронизации](synchronization-synchronizationjob.md) , основанный на шаблоне. Разработчик приложений задает шаблон; всем пользователям можно извлечь шаблон, чтобы увидеть параметры по умолчанию, включая [схемы синхронизации](synchronization-synchronizationschema.md).

Предоставление нескольких шаблонов для приложения и назначить шаблон по умолчанию. Если приложение, которое вы хотите несколько шаблонов, seek инструкции для определения, какой из них лучше всего соответствует потребностям приложения.

## <a name="methods"></a>Методы

| Метод        | Возвращаемый тип               | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |[synchronizationTemplate](synchronization-synchronizationtemplate.md) коллекции  |Список шаблонов, доступных для приложения или экземпляра приложения (участников-служб).|
|[получение](../api/synchronization-synchronizationtemplate-get.md);      |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Чтение свойства и связи объекта **synchronizationTemplate** .|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>Свойства

| Свойство      | Тип                      | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |Строка                     |Шаблон уникальный идентификатор.|
|applicationId  |String                     |Идентификатор приложения, к которому принадлежит этот шаблон.|
|по умолчанию        |Логический                    |`true`Если этот шаблон рекомендуется по умолчанию для приложения.|
|описание    |String                     |Описание шаблона.|
|обнаруживаемые   |Строка                     |`true`Если этот шаблон должен отображаться в коллекцию шаблонов, доступных для экземпляра приложения (участников-служб).|
|factoryTag     |Строка                     |Один из известных фабрики тегов, поддерживаемые обработчиком синхронизации. **FactoryTag** сообщает о том, обработчик синхронизации реализация для использования при обработке задания на основе этого шаблона.|
|метаданные       |metadataEntry коллекции   |Расширение дополнительные свойства. Если не указан явно, значения метаданных не должно изменяться.|

## <a name="relationships"></a>Связи
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
