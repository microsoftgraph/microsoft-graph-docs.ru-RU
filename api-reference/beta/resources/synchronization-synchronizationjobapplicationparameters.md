---
title: Тип ресурса Синчронизатионжобаппликатионпараметерс
description: Представляет объекты, которые необходимо подготовить, и правила, выполняемые при подготовке по требованию.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0f0b7cae5a3ce9c49ea64b603390ea65831144b
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007214"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>Тип ресурса Синчронизатионжобаппликатионпараметерс

Пространство имен: microsoft.graph

Представляет объекты, которые будут подготовлены к работе, и выполняемые правила синхронизации. Ресурс в основном используется для подготовки по требованию. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleId|String|Идентификатор Синчронизатионруле, который требуется применить; необязательно для Синчронизатионжоб с одним Синчронизатионруле.|
|вопросов|Коллекция [синчронизатионжобсубжект](../resources/synchronization-synchronizationjobsubject.md)|Идентификаторы одного или нескольких объектов, к которым применяется Синчронизатионжоб.|

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
