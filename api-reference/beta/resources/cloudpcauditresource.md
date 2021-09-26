---
title: тип ресурса cloudPcAuditResource
description: Представляет ресурс аудита.Это показывает объект целевого редактирования ресурсов с несколькими измененными свойствами.
author: ecmadao
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c168fa404d00f855659a38a096673f0524938f56
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767150"
---
# <a name="cloudpcauditresource-resource-type"></a>тип ресурса cloudPcAuditResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурс аудита.Это показывает объект целевого редактирования ресурсов с несколькими измененными свойствами.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображает имя объекта ресурса.|
|modifiedProperties|[коллекция cloudPcAuditProperty](../resources/cloudpcauditproperty.md)|Список измененных свойств.|
|type|Строка|Тип ресурса аудита.|
|resourceId|String|ID ресурса аудита.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditResource"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```
