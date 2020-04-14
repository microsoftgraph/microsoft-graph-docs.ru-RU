---
title: Тип ресурса Провисионедидентити
description: Описывает удостоверение, связанное со сводным событием объекта наполнения.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5fde45d8e9baf28fddfe9935d71689d24059dfa3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43371397"
---
# <a name="provisionedidentity-resource-type"></a>Тип ресурса Провисионедидентити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает удостоверение, связанное со сводным событием объекта наполнения. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|details|[detailsInfo](detailsinfo.md)|Сведения об удостоверении.|
|displayName|Строка|Отображаемое имя удостоверения. |
|id|String|Уникально идентифицирует удостоверение.|
|идентититипе|String|Тип удостоверения, которое было подготовлено, например "пользователь" или "Группа".|

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
