---
title: Тип ресурса onPremisesAgentGroup
description: Тип ресурса onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: da089ba198b5056bdecdceba96be572366618a23
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158347"
---
# <a name="onpremisesagentgroup-resource-type"></a>Тип ресурса onPremisesAgentGroup

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет группу локального агента. Группы агентов позволяют администратору клиента назначать определенных [агентов](onpremisesagent.md) для обслуживания определенных [опубликованных локального ресурса.](publishedresource.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список onPremisesAgentGroups](../api/onpremisesagentgroup-list.md) | Коллекция onPremisesAgentGroups | Получите **коллекцию объектов onPremisesAgentGroup.** |
| [Get onPremisesAgentGroup](../api/onpremisesagentgroup-get.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | Чтение свойств и связей объекта **onPremisesAgentGroup.** |
| [Создание onPremisesAgentGroup](../api/onpremisesagentgroup-post.md)  | [onPremisesAgentGroup](onpremisesagentgroup.md) | Создайте **новую группу onPremisesAgentGroup.** |
| [Обновление onPremisesAgentGroup](../api/onpremisesagentgroup-update.md) | [onPremisesAgentGroup](onpremisesagentgroup.md) | Обновление объекта **onPremisesAgentGroup.** |
| [Удаление onPremisesAgentGroup](../api/onpremisesagentgroup-delete.md) | Нет | Удаление объекта **onPremisesAgentGroup.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String|Отображаемого имени **onPremisesAgentGroup.**|
|id|String| ИД объекта **onPremisesAgentGroup.** Только для чтения.|
|isDefault|Boolean|Указывает, является ли **onPremisesAgentGroup** группой агентов по умолчанию. По умолчанию **onPremisesAgentGroup** может быть только одна группа агентов, которая устанавливается системой.|
|publishingType|string| Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|агенты|[Коллекция onPremisesAgent](onpremisesagent.md)| Список **onPremisesAgent,** которые назначены **onPremisesAgentGroup.** Только для чтения. Допускается значение null.|
|publishedResources|[Коллекция publishedResource](publishedresource.md)| Список **publishedResource,** которые назначены **onPremisesAgentGroup.** Только для чтения. Допускается значение null.|

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



