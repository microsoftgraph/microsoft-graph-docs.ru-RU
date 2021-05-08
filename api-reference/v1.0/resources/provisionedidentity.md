---
title: тип ресурса provisionedIdentity
description: Описывает удостоверение, связанное с сводным событием объекта подготовка.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 083609787920d840d8576d1c2a7cd5e39945768c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241580"
---
# <a name="provisionedidentity-resource-type"></a>тип ресурса provisionedIdentity

Пространство имен: microsoft.graph


Описывает удостоверение, связанное с сводным событием объекта подготовка. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|подробности|[detailsInfo](detailsinfo.md)|Сведения о удостоверении.|
|displayName|Строка|Отображение имени удостоверения. |
|id|Строка|Уникально идентифицирует удостоверение.|
|identityType|Строка|Тип предварительного удостоверения, например "пользователь" или "группа".|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedIdentity",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String",
  "identityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


