---
title: тип ресурса subjectRightsRequestDetail
description: Представляет сведения о запросе на права субъекта, включая количество найденных элементов, количество рассмотренных элементов и т. д.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 9e332d53acdeea4eed7b970263547dd066974210
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457258"
---
# <a name="subjectrightsrequestdetail-resource-type"></a>тип ресурса subjectRightsRequestDetail

Пространство имен: microsoft.graph

Представляет сведения о запросе на права субъекта, включая количество найденных элементов, количество рассмотренных элементов и т. д.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|excludedItemCount|Int64|Количество элементов, исключенных из запроса.|
|insightCounts|Коллекция [keyValuePair](../resources/keyvaluepair.md)|Количество элементов на понимание.|
|itemCount|Int64|Количество найденных элементов.|
|itemNeedReview|Int64|Количество элементов, которые необходимо просмотреть.|
|productItemCounts|Коллекция [keyValuePair](../resources/keyvaluepair.md)|Количество элементов для каждого продукта, таких как Exchange, SharePoint, OneDrive и Teams.|
|signedOffItemCount|Int64|Количество элементов, подписанных администратором.|
|totalItemSize|Int64|Общий размер элемента в bytes.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestDetail",
      "itemCount": "Int64",
      "totalItemSize": "Int64",
      "itemNeedReview": "Int64",
      "signedOffItemCount": "Int64",
      "excludedItemCount": "Int64",
      "productItemCounts": [],
      "insightCounts": []
}
```

