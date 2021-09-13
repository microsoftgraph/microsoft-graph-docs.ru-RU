---
title: тип ресурса provisionedIdentity
description: Описывает удостоверение, связанное с сводным событием объекта подготовка.
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 63374ee02bf178f429f5f3afa998d0c0bb3c61d9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019183"
---
# <a name="provisionedidentity-resource-type"></a>тип ресурса provisionedIdentity

Пространство имен: microsoft.graph


Описывает удостоверение, связанное с сводным событием объекта подготовка. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|details|[detailsInfo](detailsinfo.md)|Сведения о удостоверении.|
|displayName|Строка|Отображение имени удостоверения. |
|id|String|Уникально идентифицирует удостоверение.|
|identityType|String|Тип предварительного удостоверения, например "пользователь" или "группа".|

## <a name="json-representation"></a>Представление JSON

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


