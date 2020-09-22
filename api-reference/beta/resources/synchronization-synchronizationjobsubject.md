---
title: Тип ресурса Синчронизатионжобсубжект
description: Представляет объекты, которые будут подготовлены при подготовке по запросу.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f1f7421e00fbf3f974039878e9250f07a2bcbd0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023837"
---
# <a name="synchronizationjobsubject-resource-type"></a>Тип ресурса Синчронизатионжобсубжект

Пространство имен: microsoft.graph

Представляет объекты, которые будут подготовлены при подготовке по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|objectId|String|Идентификатор объекта, к которому применяется Синчронизатионжоб.|
|обжекттипенаме|String|Тип объекта, к которому применяется Синчронизатионжоб.|

## <a name="relationships"></a>Отношения
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


