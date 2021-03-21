---
title: onPremisesAgent type
description: onPremisesAgent типа ресурса.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 74128ab48e023f066f259fea5f326d5e1642eb14
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956934"
---
# <a name="onpremisesagent-resource-type"></a>onPremisesAgent type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет локального агента. Агенты локального использования, установленные администратором клиента, могут быть настроены для доступа и обработки запросов к определенному [опубликованому ресурсу.](publishedresource.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список onPremisesAgents](../api/onpremisesagent-list.md) | [коллекция onPremisesAgent](onpremisesagent.md) | Получите **коллекцию объектов onPremisesAgents.** |
| [Get onPremisesAgent](../api/onpremisesagent-get.md) | [onPremisesAgent](onpremisesagent.md) | Ознакомьтесь с свойствами и отношениями **объекта onPremisesAgent.** |
| [Назначение onPremisesAgent onPremisesAgentGroup](../api/onpremisesagent-post-agentgroups.md) | Нет | Назначение **onPremisesAgent** для **onPremisesAgentGroup.**|
| [Удаление onpremisesAgent из onPremisesAgentGroup](../api/onpremisesagent-delete-agentgroups.md) | Нет | Удалите **onPremisesAgent** из **onPremisesAgentGroup.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|externalIp|Строка|Внешний IP-адрес, обнаруженный службой для машины агента. Только для чтения|
|id|Строка| ID объекта onPremisesAgent. Только для чтения.|
|machineName|Строка|Имя машины, на которую работает aggent. Только для чтения|
|status|agentStatus| Возможные значения: `active`, `inactive`.|
|publishingType|Строка| Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|agentGroups|[коллекция onPremisesAgentGroup](onpremisesagentgroup.md)| Список **onPremisesAgentGroups,** который назначен **onPremisesAgent.** Только для чтения. Допускается значение null.|

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



