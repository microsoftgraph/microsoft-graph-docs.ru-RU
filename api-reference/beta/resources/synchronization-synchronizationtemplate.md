---
title: Тип ресурса Синчронизатионтемплате
description: " любой пользователь может получить шаблон для просмотра параметров по умолчанию, в том числе схемы синхронизации."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 125b8fe81aedc285da33380c3043827c7c534ab8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620649"
---
# <a name="synchronizationtemplate-resource-type"></a>Тип ресурса Синчронизатионтемплате

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет предварительно настроенные параметры синхронизации для определенного приложения. Эти параметры будут использоваться по умолчанию для всех [заданий синхронизации](synchronization-synchronizationjob.md) , основанных на шаблоне. Разработчик приложения определяет шаблон; любой пользователь может получить шаблон для просмотра параметров по умолчанию, в том числе [схемы синхронизации](synchronization-synchronizationschema.md).

Вы можете предоставить несколько шаблонов для приложения и назначить шаблон по умолчанию. Если для интересующего вас приложения доступно несколько шаблонов, попросите рекомендаций для конкретного приложения, чтобы определить, какой из них наилучшим образом соответствует вашим потребностям.

## <a name="methods"></a>Методы

| Метод        | Возвращаемый тип               | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |Коллекция [синчронизатионтемплате](synchronization-synchronizationtemplate.md)  |Список шаблонов, доступных для приложения или экземпляра приложения (субъекта-службы).|
|[получение](../api/synchronization-synchronizationtemplate-get.md);      |[Синчронизатионтемплате](synchronization-synchronizationtemplate.md)   |Чтение свойств и связей объекта **синчронизатионтемплате** .|
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
|обнаружения   |String                     |`true`Если этот шаблон должен отображаться в коллекции шаблонов, доступных для экземпляра приложения (субъекта-службы).|
|Факторитаг     |String                     |Один из известных тегов фабрики, поддерживаемых обработчиком синхронизации. **Факторитаг** сообщает обработчику синхронизации, какую реализацию следует использовать при обработке заданий на основе этого шаблона.|
|метаданных       |Коллекция Метадатаентри   |Дополнительные свойства расширения. Если явно не указано иное, значения метаданных не должны изменяться.|

## <a name="relationships"></a>Отношения
| Отношение      | Тип      |Описание|
|:------------------|:----------|:----------|
|схемы             |[Синчронизатионсчема](synchronization-synchronizationschema.md)     |Схема синхронизации по умолчанию для заданий, основанных на этом шаблоне.|

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
