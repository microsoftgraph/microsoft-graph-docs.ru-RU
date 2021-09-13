---
title: тип ресурса complianceInformation
description: Этот ресурс содержит данные о соответствии требованиям, связанные с безопасным управлением счетами.
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 05ba1b7900f50474e2eaaac64326f02eeadfd913
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109264"
---
#  <a name="complianceinformation-resource-type"></a>тип ресурса complianceInformation

Пространство имен: microsoft.graph

Содержит данные о соответствии требованиям, связанные с безопасным управлением счетами.

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|certificationName|Строка| Имя сертификации соответствия требованиям (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171) |
|certificationControls|[коллекция certificationControl](certificationcontrol.md)|Коллекция элементов управления сертификацией, связанных с сертификацией|

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

