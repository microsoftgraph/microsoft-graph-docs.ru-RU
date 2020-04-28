---
title: " Тип ресурса Комплианцеинформатион"
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 65eda1c24fee112ef18fc6682b537f92f924dcf8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507578"
---
#  <a name="complianceinformation-resource-type"></a>Тип ресурса Комплианцеинформатион

Пространство имен: microsoft.graph

Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.

|Свойство |Тип |Описание |
|:--|:--|:--|
|цертификатионнаме | string | Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171). |
|цертификатионконтролс | Коллекция [цертификатионконтрол](certificationcontrol.md) | Коллекция элементов управления сертификацией, связанных с сертификацией |

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
