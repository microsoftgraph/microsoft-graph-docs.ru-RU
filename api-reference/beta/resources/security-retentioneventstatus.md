---
title: Тип ресурса retentionEventStatus
description: Для хранения на основе событий предоставляет состояние распространения события в указанные расположения после создания события.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: d21fabd92f19ac1be107568426e0c3e116e6a7ea
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447814"
---
# <a name="retentioneventstatus-resource-type"></a>Тип ресурса retentionEventStatus

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для хранения на основе событий этот атрибут предоставляет состояние свойства события целевым расположениям после создания события.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|error|[microsoft.graph.publicError](../resources/publicerror.md)|Ошибка, если состояние не выполнено успешно.|
|status|microsoft.graph.security.eventStatusType|Состояние распределения. Допустимые значения: `pending`, `error`, `success`, `notAvaliable`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.retentionEventStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionEventStatus",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "status": "String"
}
```

