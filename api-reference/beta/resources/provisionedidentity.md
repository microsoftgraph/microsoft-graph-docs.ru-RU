---
title: Тип ресурса Провисионедидентити
description: Описывает удостоверение, связанное со сводным событием объекта наполнения.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb535bbba827f93b597c5e41efb128f2ad610ef2
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349435"
---
# <a name="provisionedidentity-resource-type"></a>Тип ресурса Провисионедидентити

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает удостоверение, связанное со сводным событием объекта наполнения. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|details|[Детаилсинфо](detailsinfo.md)|Сведения об удостоверении.|
|displayName|Строка|Отображаемое имя удостоверения. |
|id|String|Уникально идентифицирует удостоверение.|
|Идентититипе|String|Тип удостоверения, которое было подготовлено, например "пользователь" или "Группа".|

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
