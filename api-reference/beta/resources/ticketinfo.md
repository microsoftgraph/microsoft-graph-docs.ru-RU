---
title: тип ресурса ticketInfo
description: Объект, который представляет сведения о билетах, связанные с запросами на назначение ролей
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 410b978184efdc098dfa05c08717d7ca471ffe9c
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64508470"
---
# <a name="ticketinfo-resource-type"></a>тип ресурса ticketInfo

Пространство имен: microsoft.graph

Объект, который представляет сведения о билетах, связанные с запросами на назначение ролей

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ticketNumber|Строка|Метаданные номеров билетов|
|ticketSystem|Строка|Метаданные системы билетов|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ticketInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ticketInfo",
  "ticketNumber": "String",
  "ticketSystem": "String"
}
```

