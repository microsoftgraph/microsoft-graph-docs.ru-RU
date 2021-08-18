---
title: тип ресурса синхронизацииJobApplicationParameters
description: Представляет объекты, которые должны быть предварительно оформлены, и правила, выполненные во время подготовка по запросу.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 5d8ac5a51842d76f5c72eb2bba1d03fe1479eb30f57c498a1dcdb326f4c1ff51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224252"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>тип ресурса синхронизацииJobApplicationParameters

Пространство имен: microsoft.graph

Представляет объекты, которые будут оформлены, и правила синхронизации выполнены. Этот ресурс используется в основном для обеспечения по требованию. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleId|String|Идентификатор применяемой синхронизацииRule.|
|субъекты|[коллекция синхронизацииJobSubject](../resources/synchronization-synchronizationjobsubject.md)|Идентификаторы одного или более объектов, к которым должна применяться синхронизацияJob.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobApplicationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobApplicationParameters",
  "ruleId": "String",
  "subjects": [
    {
      "@odata.type": "microsoft.graph.synchronizationJobSubject"
    }
  ]
}
```


