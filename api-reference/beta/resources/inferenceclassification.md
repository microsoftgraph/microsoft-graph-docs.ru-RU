---
title: Тип ресурса inferenceClassification
description: 'Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ebd2a76a58e23fce51afcec5ffec8891859172aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496217"
---
# <a name="inferenceclassification-resource-type"></a>Тип ресурса inferenceClassification

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassification"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
