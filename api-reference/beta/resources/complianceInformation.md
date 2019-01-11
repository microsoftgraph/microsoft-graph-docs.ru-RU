---
title: " Тип ресурса complianceInformation"
description: Этот ресурс содержит соответствия данные, связанные с безопасного элемента управления показателя.
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820603"
---
#  <a name="complianceinformation-resource-type"></a>Тип ресурса complianceInformation

Соответствие требованиям содержит данные, связанные с безопасного элемента управления показателя.

|Свойство |Тип |Описание |
|:--|:--|:--|
|certificationName | string | Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800 171) |
|certificationControls | [certificationControl](certificationcontrol.md) коллекции | Коллекция элементов управления сертификации, связанные с сертификации |

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
