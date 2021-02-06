---
title: Тип ресурса synchronizationJobApplicationParameters
description: Представляет объекты, которые необходимо получить, и правила, которые выполняются во время предоставления по требованию.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 2c17d67f766a398f94ab4962850a762fc62f6e53
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133926"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>Тип ресурса synchronizationJobApplicationParameters

Пространство имен: microsoft.graph

Представляет объекты, которые будут быть выполнены с выполнением правил синхронизации. Ресурс в основном используется для предоставления по требованию. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleId|Строка|Идентификатор применяемого synchronizationRule.|
|subjects|[Коллекция synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)|Идентификаторы одного или более объектов, к которым необходимо применить synchronizationJob.|

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


