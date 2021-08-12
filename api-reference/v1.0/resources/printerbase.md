---
title: тип ресурса printerBase
description: Представляет базовый тип для обмена принтерами и принтерами
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 12b611e73fab82d0ac1eafbdc19b26069ccfd94fa3806e4286da0f0c6516202b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235375"
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
|displayName|String|Имя принтера/принтераShare.|
|id|String|Идентификатор.|
|isAcceptingJobs|Логическое|Принимает ли принтер или принтер в настоящее время новые задания печати.|
|расположение|[printerLocation](printerlocation.md)|Физическое и/или организационное расположение принтера/принтераShare.|
|manufacturer|String|Производитель принтера и принтераShare.|
|model|String|Имя модели принтера/принтераShare.|
|status|[printerStatus](printerstatus.md)|Состояние обработки принтера и принтераShare, включая ошибки.|

## <a name="relationships"></a>Связи
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

