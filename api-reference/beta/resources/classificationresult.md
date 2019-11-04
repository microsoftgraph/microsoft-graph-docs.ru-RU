---
title: Тип ресурса Классификатионресулт
description: Представляет результат запроса классификации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 51b03cf4a579ccab642fe9bdce2e71becebba4be
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938767"
---
# <a name="classificationresult-resource-type"></a>Тип ресурса Классификатионресулт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет результат операции классификации из модуля классификации Майкрософт. Результаты классификации данных в Azure Information Protection, Office и других службах Майкрософт могут возвращать [строго определенный набор типов классификации](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for). Эти типы можно предоставлять в API [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) для разрешения конфиденциальной информации в метку Microsoft Information Protection. 

## <a name="properties"></a>Свойства

| Свойство        | Тип  | Описание                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| confidenceLevel | Int32 | Степень вероятности результата — от 0 до 100.                         |
| count           | Int32 | Число экземпляров определенного типа данных во входных данных. |
| сенситиветипеид | GUID  | GUID обнаруженного типа конфиденциальной информации.                 |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.classificationResult",
  "baseType": null
}-->

```json
{
  "confidenceLevel": 1024,
  "count": 1024,
  "sensitiveTypeId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "classificationResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
