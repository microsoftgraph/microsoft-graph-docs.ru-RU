---
title: тип ресурса securityVendorInformation
description: " subProvider=AppLocker)."
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ed666cb4948d658dc877567bbbf31a0e6d551778
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142511"
---
# <a name="securityvendorinformation-resource-type"></a>тип ресурса securityVendorInformation

Пространство имен: microsoft.graph

Содержит сведения о поставщике, поставщике, поставщике и подпрограмме безопасности (например, поставщик=Microsoft; provider=Защитник Windows ATP; subProvider=AppLocker).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|поставщик |String|Конкретный поставщик (продукт/служба — не компания-поставщик); например, WindowsDefenderATP.|
|providerVersion|String|Версия поставщика или подпрограммы, если она существует, которая вызвала оповещение. *Required*|
|subProvider|String|Определенный субпровиндер (под агрегированием поставщика); например, WindowsDefenderATP.SmartScreen.|
|поставщик |String|Имя поставщика оповещений (например, Microsoft, Dell, FireEye). *Required*|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

