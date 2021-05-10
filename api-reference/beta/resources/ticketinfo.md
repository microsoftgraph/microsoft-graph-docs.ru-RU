---
title: тип ресурса ticketInfo
description: Объект, который представляет сведения о билетах, связанные с запросами на назначение ролей
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 584600bf017a75efb141539b6f1397920717fb76
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299761"
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

