---
title: тип ресурса redundancyDetectionSettings
description: Параметры избыточности для дела об обнаружении электронных данных.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: ddd3d06e7d174509cae55fab0542a286fd4c1c70
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2021
ms.locfileid: "61403172"
---
# <a name="redundancydetectionsettings-resource-type"></a>тип ресурса redundancyDetectionSettings

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры избыточности (потоковой отправки электронной почты и обнаружения неподалеку от дубликата) для случая обнаружения электронных данных.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|Указывает, включена ли потоковая отправка электронной почты и обнаружение дубликата.|
|maxWords|Int32|Указывает максимальное количество слов, используемых для потоковой отправки электронной почты и обнаружения неподалеку от дубликата. Чтобы узнать больше, см. [в руб. Минимальное или максимальное количество слов.](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading)|
|minWords|Int32|Указывает минимальное количество слов, используемых для потоковой отправки электронной почты и обнаружения неподалеку от дубликата. Чтобы узнать больше, см. [в руб. Минимальное или максимальное количество слов.](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading)|
|similarityThreshold|Int32|Указывает уровень сходства для документов, которые будут помещаться в один и тот же рядом дубликат. Дополнительные дополнительные сообщения см. в [сообщении о пороге сходства документов и электронной почты.](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading)|

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
