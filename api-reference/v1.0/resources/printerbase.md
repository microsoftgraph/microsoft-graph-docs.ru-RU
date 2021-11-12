---
title: тип ресурса printerBase
description: Представляет базовый тип для обмена принтерами и принтерами
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9e770cd0dfdd29da549114ca5a688718e679855c
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944986"
---
# <a name="printerbase-resource-type"></a>тип ресурса printerBase

Пространство имен: microsoft.graph

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

