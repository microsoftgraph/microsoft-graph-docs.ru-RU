---
title: " Тип ресурса Комплианцеинформатион"
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b93e01bf6274591282fd5e486bebb878672d8cc3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973232"
---
#  <a name="complianceinformation-resource-type"></a>Тип ресурса Комплианцеинформатион

Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.

|Свойство |Тип |Описание |
|:--|:--|:--|
|Цертификатионнаме | string | Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171). |
|Цертификатионконтролс | Коллекция [цертификатионконтрол](certificationcontrol.md) | Коллекция элементов управления сертификацией, связанных с сертификацией |

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
