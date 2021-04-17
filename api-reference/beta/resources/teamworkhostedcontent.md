---
title: тип ресурса teamworkHostedContent
description: Представляет богатый контент, который организован Microsoft Teams
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da0b157bab78867bd3309b4529afe8ef734f0144
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882315"
---
# <a name="teamworkhostedcontent-resource-type"></a>тип ресурса teamworkHostedContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет богатый контент, например изображения и фрагменты кода в Microsoft Teams. Для богатого [контента в сообщениях](chatMessage.md)каналов и чатов см. [в странице chatMessageHostedContent.](chatMessageHostedContent.md)

## <a name="methods"></a>Методы

| Метод                                            | Возвращаемый тип                                       | Описание                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [Получите иконки приложений](../api/teamsappicon-get.md)     | [teamworkHostedContent](teamworkhostedcontent.md)                   | Получите bytes of the hosted content backing a Teams app icon. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contentBytes|Двоичный|Только напишите. Bytes for the hosted content (such as images).|
|contentType|String|Только напишите. Тип контента, например изображение/png, изображение/jpg.|
|id|Строка|ID хост-контента.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkHostedContent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHostedContent",
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```

