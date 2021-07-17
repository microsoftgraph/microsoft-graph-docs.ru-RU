---
title: тип ресурса externalItemContent
description: Содержимое элемента, индексироваться с помощью Поиск (Майкрософт) подключения.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4dd853ca32c918988f2f99e1f1238d9ac937da02
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467454"
---
# <a name="externalitemcontent-resource-type"></a>тип ресурса externalItemContent

Пространство имен: microsoft.graph.externalConnectors

Содержимое [externalItem,](externalconnectors-externalitem.md) индексироваться с помощью Поиск (Майкрософт) [подключения](externalconnectors-externalconnection.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|type|microsoft.graph.externalConnectors.externalItemContentType|Тип контента в свойстве значения. Возможные значения: `text`, `html`, `unknownFutureValue`.|
|value|String|Содержимое для externalItem. Обязательный.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
}
-->
``` json
{
  "value": "String",
  "type": "String"
}
```

