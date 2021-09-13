---
title: тип ресурса синхронизацииJobSubject
description: Представляет объекты, которые будут представлены во время предварительной провизии по запросу.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 1f4de7d4c3d518b795d739a80403903842d16a16
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59090965"
---
# <a name="synchronizationjobsubject-resource-type"></a>тип ресурса синхронизацииJobSubject

Пространство имен: microsoft.graph

Представляет объекты, которые будут представлены во время предварительной провизии по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|objectId|String|Идентификатор объекта, к которому должна применяться синхронизацияJob.|
|objectTypeName|String|Тип объекта, к которому должна применяться синхронизацияJob.|

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


