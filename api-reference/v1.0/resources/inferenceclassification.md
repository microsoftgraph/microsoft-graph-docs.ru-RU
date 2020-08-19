---
title: Тип ресурса inferenceClassification
description: 'Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях. '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 67b115001bed8e95093598bc5bb9f1969fbb3493
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808937"
---
# <a name="inferenceclassification-resource-type"></a>Тип ресурса inferenceClassification

Пространство имен: microsoft.graph

Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях.

Дополнительные сведения см. в статье [Управление сортировкой почты](manage-focused-inbox.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание объекта inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) |[inferenceClassificationOverride](inferenceclassificationoverride.md)| Создание переопределения для отправителя, указанному по SMTP-адресу. Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.|
|[Список переопределений](../api/inferenceclassification-list-overrides.md) |Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)| Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string| Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|overrides|Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)| Набор переопределений пользователя, классифицирующих сообщения от определенных отправителей указанными способами: `focused` или `other`. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
