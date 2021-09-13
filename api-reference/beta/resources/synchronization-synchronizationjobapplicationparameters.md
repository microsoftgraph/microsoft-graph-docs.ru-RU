---
title: тип ресурса синхронизацииJobApplicationParameters
description: Представляет объекты, которые должны быть предварительно оформлены, и правила, выполненные во время подготовка по запросу.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: aeaae3419307787c019402d5b8ddf8268f1f9605
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59090961"
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


