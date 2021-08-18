---
title: " тип ресурса complianceInformation"
description: Этот ресурс содержит данные о соответствии требованиям, связанные с безопасным управлением счетами.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 0b9b7385ae06b01747c0fc1c9c9001add515f43b472c3f7d419374f6e015a8a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253763"
---
#  <a name="complianceinformation-resource-type"></a>тип ресурса complianceInformation

Пространство имен: microsoft.graph

Содержит данные о соответствии требованиям, связанные с безопасным управлением счетами.

|Свойство |Тип |Описание |
|:--|:--|:--|
|certificationName | string | Имя сертификации соответствия требованиям (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171) |
|certificationControls | [коллекция certificationControl](certificationcontrol.md) | Коллекция элементов управления сертификацией, связанных с сертификацией |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": "Collection(microsoft.graph.complianceInformation)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


