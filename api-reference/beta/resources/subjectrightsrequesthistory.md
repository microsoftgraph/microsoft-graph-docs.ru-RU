---
title: тип ресурса subjectRightsRequestHistory
description: Представляет историю запроса на права субъекта.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 0e452083ba9c75692452a24316b8450571fb560c
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60454219"
---
# <a name="subjectrightsrequesthistory-resource-type"></a>тип ресурса subjectRightsRequestHistory

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет историю запроса на права субъекта.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|changedBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, измениввшего запрос на права субъекта.|
|eventDateTime|DateTimeOffset|Данные и время изменения объекта.|
|этап|subjectRightsRequestStage|Этап, на который был изменен объект. Возможные значения: `contentRetrieval`, `contentReview`, `generateReport`, `contentDeletion`, `caseResolved`, `unknownFutureValue`.|
|stageStatus|subjectRightsRequestStageStatus|Состояние стадии, когда объект был изменен. Возможные значения: `notStarted`, `current`, `completed`, `failed`, `unknownFutureValue`.|
|type|String|Тип истории.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestHistory",
    "type": "String",
    "stage": "String",
    "stageStatus": "String",
    "eventDateTime": "String (timeStamp)",
    "changedBy": {
        "user": {
            "id": "String",
            "displayName": "String"
        }
    }
}
```

