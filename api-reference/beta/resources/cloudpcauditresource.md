---
title: тип ресурса cloudPcAuditResource
description: Представляет ресурс аудита.Это показывает объект целевого редактирования ресурсов с несколькими измененными свойствами.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ebd61a14680c5e5f2917e273456bcce60672149e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211404"
---
# <a name="cloudpcauditresource-resource-type"></a>тип ресурса cloudPcAuditResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурс аудита.Это показывает объект целевого редактирования ресурсов с несколькими измененными свойствами.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображает имя объекта ресурса.|
|modifiedProperties|[коллекция cloudPcAuditProperty](../resources/cloudpcauditproperty.md)|Список измененных свойств.|
|type|String|Тип ресурса аудита.|
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
