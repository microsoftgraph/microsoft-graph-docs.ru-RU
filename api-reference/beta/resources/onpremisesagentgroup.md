---
title: Тип ресурса Онпремисесажентграуп
description: Тип ресурса Онпремисесажентграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 84f0236c2c2e52742a84f19eae8eb7693f1b559b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052609"
---
# <a name="onpremisesagentgroup-resource-type"></a>Тип ресурса Онпремисесажентграуп

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет локальную группу агентов. Группы агентов позволяют администратору клиента назначать определенные [агенты](onpremisesagent.md) для обслуживания определенных [опубликованных локальных ресурсов](publishedresource.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Онпремисесажентграупс](../api/onpremisesagentgroup-list.md) | Коллекция Онпремисесажентграупс | Получение коллекции объектов **онпремисесажентграуп** . |
| [Получение Онпремисесажентграуп](../api/onpremisesagentgroup-get.md) | [онпремисесажентграуп](onpremisesagentgroup.md) | Чтение свойств и связей объекта **онпремисесажентграуп** . |
| [Создание Онпремисесажентграуп](../api/onpremisesagentgroup-post.md)  | [онпремисесажентграуп](onpremisesagentgroup.md) | Создание нового **онпремисесажентграуп**. |
| [Обновление Онпремисесажентграуп](../api/onpremisesagentgroup-update.md) | [онпремисесажентграуп](onpremisesagentgroup.md) | Обновление объекта **онпремисесажентграуп** . |
| [Удаление Онпремисесажентграуп](../api/onpremisesagentgroup-delete.md) | Нет | Удаление объекта **онпремисесажентграуп** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String|Отображаемое имя **онпремисесажентграуп**.|
|id|String| Идентификатор объекта **онпремисесажентграуп**. Только для чтения.|
|isDefault|Boolean|Указывает, является ли **онпремисесажентграуп** группой агентов по умолчанию. Только одна группа агентов может быть **онпремисесажентграуп** по умолчанию и задается системой.|
|публишингтипе|string| Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|агенты|Коллекция [онпремисесажент](onpremisesagent.md)| Список **онпремисесажент** , назначенных для **онпремисесажентграуп**. Только для чтения. Допускается значение null.|
|публишедресаурцес|Коллекция [публишедресаурце](publishedresource.md)| Список **публишедресаурце** , назначенных для **онпремисесажентграуп**. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "publishingType": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgentGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


