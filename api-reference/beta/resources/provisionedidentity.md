---
title: Тип ресурса Провисионедидентити
description: Описывает удостоверение, связанное со сводным событием объекта наполнения.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 03270c0b5e6ea373ad87355612ddfb85b428d61c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993142"
---
# <a name="provisionedidentity-resource-type"></a>Тип ресурса Провисионедидентити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает удостоверение, связанное со сводным событием объекта наполнения. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|details|[detailsInfo](detailsinfo.md)|Сведения об удостоверении.|
|displayName|String|Отображаемое имя удостоверения. |
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


