---
title: тип ресурса onlineMeetingInfo
description: Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a12c194f37f119211ccbe45c337cf8256d6110155382951c49b563b8d71b450d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226128"
---
# <a name="onlinemeetinginfo-resource-type"></a>тип ресурса onlineMeetingInfo

Пространство имен: microsoft.graph

Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|conferenceId|Строка| ID конференции.|
|joinUrl|Строка| Внешняя ссылка, которая запускает собрание в Интернете. Это URL-адрес, который клиенты запускают в браузер и перенаправляют пользователя, чтобы присоединиться к собранию.|
|phones|Коллекция [phone](phone.md)| Все телефонные номера, связанные с этой конференцией.|
|quickDial|Строка| Предварительно отформатированный quickdial для этого вызова.|
|tollFreeNumbers|Коллекция String| Бесплатные номера, которые можно использовать, чтобы присоединиться к конференции.|
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
}-->s


