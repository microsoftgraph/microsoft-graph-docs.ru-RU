---
title: Тип ресурса Комплианцеинформатион
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 85fef478a8dcc0f3196355d89f0a20ef0cd7a5b4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629308"
---
#  <a name="complianceinformation-resource-type"></a>Тип ресурса Комплианцеинформатион

Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|Цертификатионнаме|String| Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171). |
|Цертификатионконтролс|Коллекция [цертификатионконтрол](certificationcontrol.md)|Коллекция элементов управления сертификацией, связанных с сертификацией|

## <a name="json-representation"></a>Представление в формате JSON

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
