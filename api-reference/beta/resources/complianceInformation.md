---
title: " тип ресурса complianceInformation"
description: Этот ресурс содержит данные о соответствии требованиям, связанные с безопасным управлением счетами.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d5d59735dd8dc3dac96607bfc012f127283ca966
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023754"
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


