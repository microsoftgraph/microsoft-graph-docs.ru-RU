---
title: тип ресурса onPremisesAgentGroup
description: на типе ресурсовPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 5751e01ab6e7645416a8a8fde5c30f09c38a3d22
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956920"
---
# <a name="onpremisesagentgroup-resource-type"></a>тип ресурса onPremisesAgentGroup

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет группу локального агента. Группы агентов позволяют администратору клиента назначать определенных [агентов](onpremisesagent.md) для обслуживания определенных опубликованных локально [ресурсов.](publishedresource.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список наPremisesAgentGroups](../api/onpremisesagentgroup-list.md) | коллекция onPremisesAgentGroups | Получите **коллекцию объектов onPremisesAgentGroup.** |
| [Get onPremisesAgentGroup](../api/onpremisesagentgroup-get.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | Ознакомьтесь с свойствами и отношениями объекта **onPremisesAgentGroup.** |
| [Создание onPremisesAgentGroup](../api/onpremisesagentgroup-post.md)  | [onPremisesAgentGroup](onpremisesagentgroup.md) | Создайте **новую onPremisesAgentGroup.** |
| [Обновление наPremisesAgentGroup](../api/onpremisesagentgroup-update.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | Обновление **объекта onPremisesAgentGroup.** |
| [Удаление наPremisesAgentGroup](../api/onpremisesagentgroup-delete.md) | Нет | Удаление **объекта onPremisesAgentGroup.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка|Отображение имени **onPremisesAgentGroup.**|
|id|Строка| ID объекта **onPremisesAgentGroup**. Только для чтения.|
|isDefault|Boolean|Указывает, является **ли onPremisesAgentGroup** группой агентов по умолчанию. Только одна группа агентов может быть по умолчанию **наPremisesAgentGroup** и задаваема системой.|
|publishingType|Строка| Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|агенты|[коллекция onPremisesAgent](onpremisesagent.md)| Список **onPremisesAgent,** которые назначены **onPremisesAgentGroup.** Только для чтения. Допускается значение null.|
|publishedResources|[коллекция publishedResource](publishedresource.md)| Список **опубликованныхРесурса,** которые назначены **onPremisesAgentGroup.** Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
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



