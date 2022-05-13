---
title: Тип ресурса ticketInfo
description: Объект, представляющий сведения о билетах, связанные с запросами на назначение ролей
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d64bd63615ec156548942d14deb5833eb5dd990a
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399455"
---
# <a name="ticketinfo-resource-type"></a>Тип ресурса ticketInfo

Пространство имен: microsoft.graph

Объект, представляющий сведения о билетах, связанные с запросами на назначение ролей

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ticketNumber|String|Метаданные номера билета|
|ticketSystem|String|Метаданные системы запросов|

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

