---
title: Тип ресурса Синчронизатионжобсубжект
description: Представляет объекты, которые будут подготовлены при подготовке по запросу.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54f8271d3b11cce55cc3e7042ffcba84a330d798
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007208"
---
# <a name="synchronizationjobsubject-resource-type"></a>Тип ресурса Синчронизатионжобсубжект

Пространство имен: microsoft.graph

Представляет объекты, которые будут подготовлены при подготовке по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|objectId|String|Идентификатор объекта, к которому применяется Синчронизатионжоб.|
|обжекттипенаме|String|Тип объекта, к которому применяется Синчронизатионжоб.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobSubject",
  "objectId": "String",
  "objectTypeName": "String"
}
```
