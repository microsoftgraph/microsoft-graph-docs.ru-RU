---
title: тип ресурса externalItemContent
description: Содержимое элемента, индексироваться с помощью Поиск (Майкрософт) подключения.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 35a410a12608ad43f75196b41b3d747e56b10d59
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/17/2022
ms.locfileid: "63560028"
---
# <a name="externalitemcontent-resource-type"></a>тип ресурса externalItemContent

Пространство имен: microsoft.graph.externalConnectors

Содержимое [externalItem,](externalconnectors-externalitem.md) индексироваться с помощью Поиск (Майкрософт) [подключения](externalconnectors-externalconnection.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|type|microsoft.graph.externalConnectors.externalItemContentType|Тип контента в свойстве значения. Возможные значения: `text`, `html`, `unknownFutureValue`. Это типы контента, поддерживаемые индексером, а не разрешенные типы расширения файлов.|
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

