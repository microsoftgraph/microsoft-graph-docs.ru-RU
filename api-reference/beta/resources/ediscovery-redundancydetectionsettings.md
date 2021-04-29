---
title: тип ресурса redundancyDetectionSettings
description: Параметры избыточности для дела об обнаружении электронных данных
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: fd1ca1ea3faf03e2639896c79acd0629931c71c9
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080890"
---
# <a name="redundancydetectionsettings-resource-type"></a>тип ресурса redundancyDetectionSettings

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры избыточности (потоковой отправки электронной почты и обнаружения неподалеку от дубликата) для случая обнаружения электронных данных.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|Указывает, включена ли потоковая отправка электронной почты и обнаружение дубликата.|
|maxWords|Int32|Узнайте [больше о минимальном](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) или максимальном количестве слов.|
|minWords|Int32|Узнайте [больше о минимальном](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) или максимальном количестве слов.|
|similarityThreshold|Int32|Подробнее [см. в сообщении о пороге сходства](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) документов и электронной почты.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.redundancyDetectionSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.redundancyDetectionSettings",
  "isEnabled": "Boolean",
  "similarityThreshold": "Integer",
  "minWords": "Integer",
  "maxWords": "Integer"
}
```
