---
title: Тип ресурса Пассвордсинглесигнонсеттингс
description: Параметры, связанные с единым входом на основе паролей
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a1b2739ecbd5d09358e58203ab61d4e65c48716b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998175"
---
# <a name="passwordsinglesignonsettings-resource-type"></a>Тип ресурса Пассвордсинглесигнонсеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит коллекцию параметров единого входа на основе паролей.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|fields|Коллекция [пассвордсинглесигнонфиелд](passwordsinglesignonfield.md)||

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnSettings",
  "baseType": null
}-->

```json
{
  "fields": [{"@odata.type": "microsoft.graph.passwordSingleSignOnField"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

