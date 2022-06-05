---
title: Тип ресурса ticketInfo
description: Представляет сведения о билетах, связанные с назначением ролей и запросами на участие в программе.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e2356ef6fdbf0d1832d79fc2b68ecbef69db1ede
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900466"
---
# <a name="ticketinfo-resource-type"></a>Тип ресурса ticketInfo

Пространство имен: microsoft.graph

Представляет сведения о билетах, связанные с назначением ролей и запросами на участие в программе. Используйте этот объект для определения параметров билета для назначения роли или запроса на приемлемость, инициированного другим запросом, выполненным во внешней системе.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ticketNumber|Строка|Номер билета.|
|ticketSystem|Строка|Описание системы запросов.|

## <a name="relationships"></a>Отношения
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

