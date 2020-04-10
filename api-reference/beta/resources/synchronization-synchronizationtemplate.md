---
title: Тип ресурса Синчронизатионтемплате
description: Предоставляет предварительно настроенные параметры синхронизации для определенного приложения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5067df26f0b1c1e6b77d1c3d87d4c73bb9e45208
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217005"
---
# <a name="synchronizationtemplate-resource-type"></a>Тип ресурса Синчронизатионтемплате

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет предварительно настроенные параметры синхронизации для определенного приложения. Эти параметры будут использоваться по умолчанию для всех [заданий синхронизации](synchronization-synchronizationjob.md) , основанных на шаблоне. Разработчик приложения определяет шаблон; любой пользователь может получить шаблон для просмотра параметров по умолчанию, в том числе [схемы синхронизации](synchronization-synchronizationschema.md).

Вы можете предоставить несколько шаблонов для приложения и назначить шаблон по умолчанию. Если для интересующего вас приложения доступно несколько шаблонов, попросите рекомендаций для конкретного приложения, чтобы определить, какой из них наилучшим образом соответствует вашим потребностям.

## <a name="methods"></a>Методы

| Метод        | Возвращаемый тип               | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |Коллекция [синчронизатионтемплате](synchronization-synchronizationtemplate.md)  |Список шаблонов, доступных для приложения или экземпляра приложения (субъекта-службы).|
|[получение](../api/synchronization-synchronizationtemplate-get.md);      |[синчронизатионтемплате](synchronization-synchronizationtemplate.md)   |Чтение свойств и связей объекта **синчронизатионтемплате** .|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>Свойства

| Свойство      | Тип                      | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |Строка                     |Уникальный идентификатор шаблона.|
|applicationId  |String                     |Идентификатор приложения, к которому принадлежит этот шаблон.|
|умолчани        |Boolean                    |`true`Если этот шаблон рекомендуется использовать по умолчанию для приложения.|
|description    |String                     |Описание шаблона.|
|обнаружения   |Строка                     |`true`Если этот шаблон должен отображаться в коллекции шаблонов, доступных для экземпляра приложения (субъекта-службы).|
|факторитаг     |Строка                     |Один из известных тегов фабрики, поддерживаемых обработчиком синхронизации. **Факторитаг** сообщает обработчику синхронизации, какую реализацию следует использовать при обработке заданий на основе этого шаблона.|
|метаданных       |Коллекция Метадатаентри   |Дополнительные свойства расширения. Если явно не указано иное, значения метаданных не должны изменяться.|

## <a name="relationships"></a>Отношения
| Связь      | Тип      |Описание|
|:------------------|:----------|:----------|
|схемы             |[синчронизатионсчема](synchronization-synchronizationschema.md)     |Схема синхронизации по умолчанию для заданий, основанных на этом шаблоне.|

## <a name="json-representation"></a>Представление JSON

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
