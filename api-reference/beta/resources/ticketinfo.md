---
title: тип ресурса ticketInfo
description: Объект, который представляет сведения о билетах, связанные с запросами на назначение ролей
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e75cd3f594a515e83abb59d0b476e4d130771875
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694906"
---
# <a name="ticketinfo-resource-type"></a>тип ресурса ticketInfo

Пространство имен: microsoft.graph

Объект, который представляет сведения о билетах, связанные с запросами на назначение ролей

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ticketNumber|String|Метаданные номеров билетов|
|ticketSystem|String|Метаданные системы билетов|

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

