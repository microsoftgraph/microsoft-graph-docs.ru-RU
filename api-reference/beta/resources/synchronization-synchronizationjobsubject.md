---
title: тип ресурса синхронизацииJobSubject
description: Представляет объекты, которые будут представлены во время предварительной провизии по запросу.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c7dea31898cb0bfb521367042401be7c583c60c2868d4805682c9d0e707fc898
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226114"
---
# <a name="synchronizationjobsubject-resource-type"></a>тип ресурса синхронизацииJobSubject

Пространство имен: microsoft.graph

Представляет объекты, которые будут представлены во время предварительной провизии по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|objectId|String|Идентификатор объекта, к которому должна применяться синхронизацияJob.|
|objectTypeName|Строка|Тип объекта, к которому должна применяться синхронизацияJob.|

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


