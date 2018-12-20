---
title: " Тип ресурса complianceInformation"
description: Этот ресурс содержит соответствия данные, связанные с безопасного элемента управления показателя.
ms.openlocfilehash: a32670c6d11d391834358b769ae938a67b3d8aad
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380961"
---
#  <a name="complianceinformation-resource-type"></a>Тип ресурса complianceInformation

Соответствие требованиям содержит данные, связанные с безопасного элемента управления показателя.

|Свойство |Тип |Описание |
|:--|:--|:--|
|certificationName | строка | Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800 171) |
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
