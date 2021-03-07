---
title: тип ресурса printerBase
description: Представляет базовый тип для обмена принтерами и принтерами
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 515c14bb4de7352a8c17cffdacbd7a4c9091fc70
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517332"
---
# <a name="printerbase-resource-type"></a>тип ресурса printerBase

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет базовый тип для [типов сущности](printer.md) [принтера и принтераShare.](printerShare.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|capabilities|[printerCapabilities](printercapabilities.md)|Возможности принтера и принтераShare.|
|defaults|[printerDefaults](printerdefaults.md)|Параметры печати принтера и принтера По умолчанию.|
|displayName|Строка|Имя принтера/принтераShare.|
|id|Строка|Идентификатор.|
|isAcceptingJobs|Логический|Принимает ли принтер или принтер в настоящее время новые задания печати.|
|location|[printerLocation](printerlocation.md)|Физическое и/или организационное расположение принтера/принтераShare.|
|manufacturer|String|Производитель принтера и принтераShare.|
|model|String|Имя модели принтера/принтераShare.|
|status|[printerStatus](printerstatus.md)|Состояние обработки принтера и принтераShare, включая ошибки.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|jobs|[коллекция printJob](printjob.md)|Список заданий, которые стоят в очереди для печати принтером или принтеромShare.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerBase",
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  }
}
```

