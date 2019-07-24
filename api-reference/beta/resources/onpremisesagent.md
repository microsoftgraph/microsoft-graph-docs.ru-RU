---
title: Тип ресурса Онпремисесажент
description: Тип ресурса Онпремисесажент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1bcff659cf30b946654f14190b2cf5f693d27bc4
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841264"
---
# <a name="onpremisesagent-resource-type"></a>Тип ресурса Онпремисесажент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет локальный агент. Локальные агенты, установленные администратором клиента, можно настроить для доступа к определенному опубликованному ресурсу или [](publishedresource.md)обработки запросов.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Онпремисесажентс](../api/onpremisesagent-list.md) | Коллекция [онпремисесажент](onpremisesagent.md) | Получение коллекции объектов **онпремисесажентс** . |
| [Получение Онпремисесажент](../api/onpremisesagent-get.md) | [Онпремисесажент](onpremisesagent.md) | Чтение свойств и связей объекта **онпремисесажент** . |
| [Назначение Онпремисесажент для Онпремисесажентграуп](../api/onpremisesagent-post-agentgroups.md) | Нет | Назначение **онпремисесажент** для **онпремисесажентграуп**.|
| [Удаление Онпремисесажент из Онпремисесажентграуп](../api/onpremisesagent-delete-agentgroups.md) | Нет | Удаление **онпремисесажент** из **онпремисесажентграуп**. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|Екстерналип|String|Внешний IP-адрес, обнаруженный службой для компьютера агента. Только для чтения|
|id|Строка| Идентификатор объекта Онпремисесажент. Только для чтения.|
|ИмяКомпьютера|String|Имя компьютера, на котором выполняется агжент. Только для чтения|
|status|string| Возможные значения: `active`, `inactive`.|
|Публишингтипе|string| Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|

## <a name="relationships"></a>Отношения

| Отношение | Тип        | Описание |
|:-------------|:------------|:------------|
|Ажентграупс|Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)| Список **онпремисесажентграупс** , которым назначено **онпремисесажент** . Только для чтения. Допускается значение null.|

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
