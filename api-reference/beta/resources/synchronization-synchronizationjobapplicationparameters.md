---
title: Тип ресурса Синчронизатионжобаппликатионпараметерс
description: Представляет объекты, которые необходимо подготовить, и правила, выполняемые при подготовке по требованию.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: eaa569faa7705baf95ef5843ad0ae1e66a0bf1ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026112"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>Тип ресурса Синчронизатионжобаппликатионпараметерс

Пространство имен: microsoft.graph

Представляет объекты, которые будут подготовлены к работе, и выполняемые правила синхронизации. Ресурс в основном используется для подготовки по требованию. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleId|String|Идентификатор Синчронизатионруле, который требуется применить; необязательно для Синчронизатионжоб с одним Синчронизатионруле.|
|вопросов|Коллекция [синчронизатионжобсубжект](../resources/synchronization-synchronizationjobsubject.md)|Идентификаторы одного или нескольких объектов, к которым применяется Синчронизатионжоб.|

## <a name="relationships"></a>Отношения
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


