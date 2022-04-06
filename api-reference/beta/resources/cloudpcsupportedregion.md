---
title: тип ресурса cloudPcSupportedRegion
description: Представляет поддерживаемый регион для создания сетевого подключения Azure для облачных компьютеров.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d13bfb6709d856119dcfaa700d819b9ed6f55258
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588570"
---
# <a name="cloudpcsupportedregion-resource-type"></a>тип ресурса cloudPcSupportedRegion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поддерживаемый регион для создания сетевого подключения Azure для облачных компьютеров.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список cloudPcSupportedRegions](../api/virtualendpoint-list-supportedregions.md)|[коллекция cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md)|Список поддерживаемых регионов, доступных для создания подключений к облачным ПК.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для поддерживаемого региона. Только для чтения.|
|displayName|Строка|Имя поддерживаемой области. Только для чтения.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcSupportedRegion",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSupportedRegion",
  "id": "String (identifier)",
  "displayName": "String"
}
```
