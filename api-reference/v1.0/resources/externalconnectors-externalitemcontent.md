---
title: тип ресурса externalItemContent
description: Содержимое элемента, индексироваться с помощью Поиск (Майкрософт) подключения.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: eade917bcee86acbc44917d8809fb26a1776bf42
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123428"
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

