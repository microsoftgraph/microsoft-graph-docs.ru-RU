---
title: Тип ресурса Синчронизатионжобаппликатионпараметерс
description: Представляет объекты, которые необходимо подготовить, и правила, выполняемые при подготовке по требованию.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca91021ccb9fbc4cf8ec6c61b4edea979bb7c833
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523205"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>Тип ресурса Синчронизатионжобаппликатионпараметерс

Пространство имен: microsoft.graph

Представляет объекты, которые будут подготовлены к работе, и выполняемые правила синхронизации. Ресурс в основном используется для подготовки по требованию. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleId|String|Идентификатор Синчронизатионруле, который требуется применить.|
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


