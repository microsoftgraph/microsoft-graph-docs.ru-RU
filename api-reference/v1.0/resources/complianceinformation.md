---
title: Тип ресурса complianceInformation
description: Этот ресурс содержит данные о соответствии, связанные с управлением оценкой безопасности.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: dc7f50753723d5ae0566803b3ad3b1937ec08f1f
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971527"
---
#  <a name="complianceinformation-resource-type"></a>Тип ресурса complianceInformation

Пространство имен: microsoft.graph

Содержит данные о соответствии, связанные с управлением оценкой безопасности.

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|certificationName|Строка| Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171) |
|certificationControls|[Коллекция certificationControl](certificationcontrol.md)|Коллекция элементов управления сертификацией, связанных с сертификацией|

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
  "certificationControls": [{"@odata.type": "microsoft.graph.certificationControl"}]
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

