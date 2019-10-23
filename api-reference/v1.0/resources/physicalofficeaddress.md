---
title: Тип ресурса Фисикалоффицеаддресс
description: Представляет рабочий адрес ресурса, например контакт или событие.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7d79479136390627eeb82a269e79b286cebf9a2e
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622693"
---
# <a name="physicalofficeaddress-resource-type"></a>Тип ресурса Фисикалоффицеаддресс

Представляет рабочий адрес ресурса, например контакта в Организации.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|city|String|Город.|
|countryOrRegion|String|Страна или регион. Это строковое значение в произвольном формате, например "США".|
|officeLocation  | String | Местоположение Office, например здание и номер офиса для контакта в Организации.  |
|postalCode|String|Почтовый индекс.|
|state|String|Штат.|
|street|String|Улица.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
