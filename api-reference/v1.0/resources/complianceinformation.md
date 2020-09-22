---
title: Тип ресурса Комплианцеинформатион
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 00447f134b2c54bdda92857c6c84c05e8c52b3cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018937"
---
#  <a name="complianceinformation-resource-type"></a>Тип ресурса Комплианцеинформатион

Пространство имен: microsoft.graph

Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|цертификатионнаме|String| Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171). |
|цертификатионконтролс|Коллекция [цертификатионконтрол](certificationcontrol.md)|Коллекция элементов управления сертификацией, связанных с сертификацией|

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

