---
title: " Тип ресурса complianceInformation"
description: Этот ресурс содержит данные о соответствии, связанные с управлением оценкой безопасности.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 9d65043ca09ce945bbc87b83bfe2ec84d7f512bb
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944929"
---
#  <a name="complianceinformation-resource-type"></a>Тип ресурса complianceInformation

Пространство имен: microsoft.graph

Содержит данные о соответствии, связанные с управлением оценкой безопасности.

|Свойство |Тип |Описание |
|:--|:--|:--|
|certificationName | string | Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171) |
|certificationControls | [Коллекция certificationControl](certificationcontrol.md) | Коллекция элементов управления сертификацией, связанных с сертификацией |

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


