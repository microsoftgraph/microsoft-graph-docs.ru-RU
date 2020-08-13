---
title: Тип ресурса Пассвордсинглесигнонсеттингс
description: Параметры, связанные с единым входом на основе паролей
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4da86cb39a1b16c9312ebe8de35c7fc87a09fdb
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658189"
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