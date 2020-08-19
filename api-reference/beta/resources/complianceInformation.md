---
title: " Тип ресурса Комплианцеинформатион"
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2c8bb3b2a016ec58da1ad58b01843a2691ad13b7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811142"
---
#  <a name="complianceinformation-resource-type"></a>Тип ресурса Комплианцеинформатион

Пространство имен: microsoft.graph

Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.

|Свойство |Тип |Описание |
|:--|:--|:--|
|цертификатионнаме | string | Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171). |
|цертификатионконтролс | Коллекция [цертификатионконтрол](certificationcontrol.md) | Коллекция элементов управления сертификацией, связанных с сертификацией |

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
