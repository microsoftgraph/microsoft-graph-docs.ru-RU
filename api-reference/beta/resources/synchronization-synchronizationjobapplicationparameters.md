---
title: Тип ресурса synchronizationJobApplicationParameters
description: Представляет объекты для подготовки и правила, выполняемые во время подготовки по запросу.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 08dc3f6494a2c7e641f6ebfc81eb223aa990eb69
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296453"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>Тип ресурса synchronizationJobApplicationParameters

Пространство имен: microsoft.graph

Представляет объекты, которые будут подготовлены, и выполняемые правила синхронизации. Ресурс в основном используется для подготовки по запросу. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleId|Строка|Идентификатор [применяемого synchronizationRule](synchronization-synchronizationrule.md) . Этот идентификатор правила определяется в схеме для [заданного задания синхронизации или шаблона](../api/synchronization-synchronizationschema-get.md). |
|Предметы|[Коллекция synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)|Идентификаторы одного или нескольких объектов, к которым будет применено задание синхронизации.|

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


