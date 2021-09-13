---
title: тип ресурса onlineMeetingInfo
description: Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.
ms.localizationpriority: medium
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3ff85e6e14f7af23d383d9d19f929deefddeadc7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072003"
---
# <a name="onlinemeetinginfo-resource-type"></a>тип ресурса onlineMeetingInfo

Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|conferenceId|Строка| ID конференции.|
|joinUrl|Строка| Внешняя ссылка, которая запускает собрание в Интернете. Это URL-адрес, который клиенты запускают в браузер и перенаправляют пользователя, чтобы присоединиться к собранию.|
|phones|Коллекция [phone](phone.md)| Все телефонные номера, связанные с этой конференцией.|
|quickDial|String| Предварительно отформатированный quickdial для этого вызова.|
|tollFreeNumbers|Коллекция String| Бесплатные номера, которые можно использовать, чтобы присоединиться к конференции.|
|tollNumber|String| Платный номер, который можно использовать для большого количества участников конференции.|

## <a name="json-representation"></a>Представление в формате JSON

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

