---
title: тип ресурса onlineMeetingInfo
description: Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f2a114ed51217e88cf981208b3b010f82a1524221724c8edf2479efc5758ec25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202170"
---
# <a name="onlinemeetinginfo-resource-type"></a>тип ресурса onlineMeetingInfo

Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|conferenceId|String| ID конференции.|
|joinUrl|String| Внешняя ссылка, которая запускает собрание в Интернете. Это URL-адрес, который клиенты запускают в браузер и перенаправляют пользователя, чтобы присоединиться к собранию.|
|phones|Коллекция [phone](phone.md)| Все телефонные номера, связанные с этой конференцией.|
|quickDial|String| Предварительно отформатированный quickdial для этого вызова.|
|tollFreeNumbers|Коллекция строк| Бесплатные номера, которые можно использовать, чтобы присоединиться к конференции.|
|tollNumber|String| Платный номер, который можно использовать для большого количества участников конференции.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onlineMeetingInfo"
}-->

```json
{
  "conferenceId": "String",
  "joinUrl": "String",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "quickDial": "String",
  "tollFreeNumbers": ["String"],
  "tollNumber": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

