---
title: тип ресурса physicalOfficeAddress
description: Представляет бизнес-адрес такого ресурса, как контакт или событие.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9f632fab8d5859a72eff551bba35184face6e3869255687ad9758decf3b131d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243315"
---
# <a name="physicalofficeaddress-resource-type"></a>тип ресурса physicalOfficeAddress

Пространство имен: microsoft.graph

Представляет бизнес-адрес такого ресурса, как организационный контакт.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|city|String|Город.|
|countryOrRegion|String|Страна или регион. Это строковое значение в произвольном формате, например "США".|
|officeLocation  | String | Office, например здание и номер офиса для организационного контакта.  |
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

