---
title: Тип ресурса eventQuery
description: Представляет рабочую нагрузку (SharePoint Online, OneDrive для бизнеса, Exchange Online) и идентификационные данные, связанные с событием хранения.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: bfdb65f2609947b6cc820c5c4937925c5b340115
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447857"
---
# <a name="eventquery-resource-type"></a>Тип ресурса eventQuery

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет рабочую нагрузку (SharePoint Online, OneDrive для бизнеса, Exchange Online) и идентификационные данные, связанные с событием хранения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|queryType|microsoft.graph.security.queryType|Представляет тип запроса, связанного с событием. "files" для SPO и ODB, а также "messages" для EXO. Возможные значения: `files`, , `messages``unknownFutureValue`.|
|Запрос|String|Представляет уникальную идентификацию запроса. "Идентификатор ресурса" для SharePoint Online и OneDrive для бизнеса, "ключевые слова" для Exchange Online.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.eventQueries"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.eventQuery",
  "queryType": "String",
  "query": "String"
}
```


