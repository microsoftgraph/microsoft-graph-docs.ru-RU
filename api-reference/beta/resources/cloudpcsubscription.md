---
title: Тип ресурса cloudPcSubscription
description: Представляет подписку на облачный компьютер.
author: xhan2077
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 425ada12758e2602d8cf262e27c34087722bf84f
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366328"
---
# <a name="cloudpcsubscription-resource-type"></a>Тип ресурса cloudPcSubscription

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о подписке, которые можно использовать для хранения моментальных снимков или моментальных снимков облачного компьютера для проведения экспертного анализа.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|subscriptionId|String|Идентификатор подписки.|
|subscriptionName|String|Имя подписки.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "subscriptionId",
  "@odata.type": "microsoft.graph.cloudPcSubscription",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSubscription",
  "subscriptionId": "String",
  "subscriptionName": "String"
}
```
