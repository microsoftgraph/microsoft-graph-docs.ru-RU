---
title: тип ресурса provisionedIdentity
description: Описывает удостоверение, связанное с сводным событием объекта подготовка.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 89ba5791235810529e7cc3b2b3c4e1d817920148790f7f9934edb20432420215
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251838"
---
# <a name="provisionedidentity-resource-type"></a>тип ресурса provisionedIdentity

Пространство имен: microsoft.graph


Описывает удостоверение, связанное с сводным событием объекта подготовка. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|подробности|[detailsInfo](detailsinfo.md)|Сведения о удостоверении.|
|displayName|String|Отображение имени удостоверения. |
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


