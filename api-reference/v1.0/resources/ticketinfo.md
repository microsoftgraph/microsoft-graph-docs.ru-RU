---
title: Тип ресурса ticketInfo
description: Представляет сведения о билетах, связанные с назначением ролей и запросами на участие в программе.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e2356ef6fdbf0d1832d79fc2b68ecbef69db1ede
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134381"
---
# <a name="ticketinfo-resource-type"></a>Тип ресурса ticketInfo

Пространство имен: microsoft.graph

Представляет сведения о билетах, связанные с назначением ролей и запросами на участие в программе. Используйте этот объект для определения параметров билета для назначения роли или запроса на приемлемость, инициированного другим запросом, выполненным во внешней системе.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ticketNumber|String|Номер билета.|
|ticketSystem|String|Описание системы запросов.|

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

