---
title: Тип ресурса eventPropagationResult
description: Представляет состояние успешности созданного события и дополнительные сведения о расположениях с заданной областью.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f8822b44020b2e76a41372b93f8bb71ee5f8bafe
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447862"
---
# <a name="eventpropagationresult-resource-type"></a>Тип ресурса eventPropagationResult

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние запроса на создание события хранения и дополнительные сведения о расположениях с заданной областью.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|status|microsoft.graph.security.eventPropagationStatus|Указывает состояние запроса на создание события. Допустимые значения: `none`, `inProcessing`, `failed`, `success`.|
|statusInformation|String|Дополнительные сведения о состоянии запроса на создание события.|
|serviceName|String|Имя рабочей нагрузки, связанной с событием.|
|расположение;|String|Имя конкретного расположения в рабочей нагрузке, связанной с событием.|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.eventPropagationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.eventPropagationResult",
  "workload": "String",
  "location": "String",
  "status": "String",
  "statusInformation": "String"
}
```


