---
title: тип ресурса subjectRightsRequestStageDetail
description: Представляет свойства этапов запроса на права субъекта
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f53bce724c6ff48eba65277585a45757eb060c13
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60454129"
---
# <a name="subjectrightsrequeststagedetail-resource-type"></a>тип ресурса subjectRightsRequestStageDetail

Пространство имен: microsoft.graph

Представляет свойства этапов запроса на права субъекта. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|error|[publicError](../resources/publicerror.md)|Описывает ошибку, если она есть, на текущем этапе.|
|этап|subjectRightsRequestStage|Этап запроса на права субъекта. Возможные значения: `contentRetrieval`, `contentReview`, `generateReport`, `contentDeletion`, `caseResolved`, `unknownFutureValue`.|
|status|subjectRightsRequestStageStatus|Состояние текущего этапа. Возможные значения: `notStarted`, `current`, `completed`, `failed`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestStageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestStageDetail",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "stage": "microsoft.graph.subjectRightsRequestStage",
  "status": "microsoft.graph.subjectRightsRequestStageStatus"
}
```

