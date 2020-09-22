---
title: Тип ресурса Самлсинглесигнонсеттингс
description: Представляет параметры единого входа SAML.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 6c07e9c0284ef111a3032ec729c3b741be65f920
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016032"
---
# <a name="samlsinglesignonsettings-resource-type"></a>Тип ресурса Самлсинглесигнонсеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контейнер для параметров, связанных с единым входом SAML.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|релайстате|String| Относительный URI, по которому поставщик услуг перенаправляется после завершения процесса единого входа. |


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
}-->

```json
{
    "relayState": "string",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "samlSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


