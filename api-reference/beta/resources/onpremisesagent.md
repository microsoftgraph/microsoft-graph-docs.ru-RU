---
title: Тип ресурса onPremisesAgent
description: Тип ресурса onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 59ee11bb952c85695b8c20daa1e040c8899740b9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158354"
---
# <a name="onpremisesagent-resource-type"></a>Тип ресурса onPremisesAgent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет локального агента. Для локального агента, установленного администратором клиента, можно настроить доступ и обработку запросов к определенному [опубликованного ресурса.](publishedresource.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список onPremisesAgents](../api/onpremisesagent-list.md) | [Коллекция onPremisesAgent](onpremisesagent.md) | Получите **коллекцию объектов onPremisesAgents.** |
| [Get onPremisesAgent](../api/onpremisesagent-get.md) | [onPremisesAgent](onpremisesagent.md) | Чтение свойств и связей объекта **onPremisesAgent.** |
| [Назначение onPremisesAgent onPremisesAgentGroup](../api/onpremisesagent-post-agentgroups.md) | Нет | **Назначьте onPremisesAgent** для **onPremisesAgentGroup.**|
| [Удаление onpremisesAgent из onPremisesAgentGroup](../api/onpremisesagent-delete-agentgroups.md) | Нет | Удалите **onPremisesAgent** из **onPremisesAgentGroup.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|externalIp|String|Внешний IP-адрес, обнаруженный службой для компьютера агента. Только для чтения|
|id|String| ИД объекта onPremisesAgent. Только для чтения.|
|machineName|String|Имя компьютера, на которого работает aggent. Только для чтения|
|status|string| Возможные значения: `active`, `inactive`.|
|publishingType|string| Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|agentGroups|[Коллекция onPremisesAgentGroup](onpremisesagentgroup.md)| Список **onPremisesAgentGroups,** которые **назначены onPremisesAgent.** Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "keyProperty": "id"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string",
  "supportedPublishingTypes": ["string"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



