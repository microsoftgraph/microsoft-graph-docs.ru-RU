---
title: тип ресурса complianceInformation
description: Этот ресурс содержит данные о соответствии требованиям, связанные с безопасным управлением счетами.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 427660aa0f7227a4536a01cedcc7df818e8a499348c7be3f5be764f0764cad24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180875"
---
#  <a name="complianceinformation-resource-type"></a>тип ресурса complianceInformation

Пространство имен: microsoft.graph

Содержит данные о соответствии требованиям, связанные с безопасным управлением счетами.

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|certificationName|String| Имя сертификации соответствия требованиям (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171) |
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

