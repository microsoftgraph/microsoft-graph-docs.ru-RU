---
title: Тип ресурса Онпремисесажент
description: Тип ресурса Онпремисесажент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff30f427c2aac754ba3cfda4082d590e95f5edd3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522244"
---
# <a name="onpremisesagent-resource-type"></a>Тип ресурса Онпремисесажент

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет локальный агент. Локальные агенты, установленные администратором клиента, можно настроить для доступа к определенному [опубликованному ресурсу](publishedresource.md)или обработки запросов.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Онпремисесажентс](../api/onpremisesagent-list.md) | Коллекция [онпремисесажент](onpremisesagent.md) | Получение коллекции объектов **онпремисесажентс** . |
| [Получение Онпремисесажент](../api/onpremisesagent-get.md) | [онпремисесажент](onpremisesagent.md) | Чтение свойств и связей объекта **онпремисесажент** . |
| [Назначение Онпремисесажент для Онпремисесажентграуп](../api/onpremisesagent-post-agentgroups.md) | Нет | Назначение **онпремисесажент** для **онпремисесажентграуп**.|
| [Удаление Онпремисесажент из Онпремисесажентграуп](../api/onpremisesagent-delete-agentgroups.md) | Нет | Удаление **онпремисесажент** из **онпремисесажентграуп**. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|екстерналип|String|Внешний IP-адрес, обнаруженный службой для компьютера агента. Только для чтения|
|id|Строка| Идентификатор объекта Онпремисесажент. Только для чтения.|
|ИмяКомпьютера|String|Имя компьютера, на котором выполняется агжент. Только для чтения|
|status|string| Возможные значения: `active`, `inactive`.|
|публишингтипе|строка| Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|ажентграупс|Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)| Список **онпремисесажентграупс** , которым назначено **онпремисесажент** . Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "baseType": "",
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
