---
title: Тип ресурса synchronizationJobSubject
description: Представляет объекты, которые будут быть представлены во время предоставления по требованию.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c9e6d83ed7024556954740e89edcc18f7b56ba04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132001"
---
# <a name="synchronizationjobsubject-resource-type"></a>Тип ресурса synchronizationJobSubject

Пространство имен: microsoft.graph

Представляет объекты, которые будут быть представлены во время предоставления по требованию.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|objectId|String|Идентификатор объекта, к которому применяется synchronizationJob.|
|objectTypeName|Строка|Тип объекта, к которому применяется synchronizationJob.|

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


