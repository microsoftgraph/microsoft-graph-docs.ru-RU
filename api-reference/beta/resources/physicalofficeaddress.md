---
title: тип ресурса physicalOfficeAddress
description: Представляет бизнес-адрес такого ресурса, как контакт или событие.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: ba9210df47c81f3714ea0fa11a9c3d2d9c1a359e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091183"
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


