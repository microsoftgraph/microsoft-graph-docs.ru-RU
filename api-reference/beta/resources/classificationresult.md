---
title: тип ресурса classificationResult
description: Представляет результат запроса классификации.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5ecc16197ef4671c6e83883bc69aed45b3ffa200
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941825"
---
# <a name="classificationresult-resource-type"></a>тип ресурса classificationResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет результат операции классификации из системы классификации Майкрософт. Классификация данных из служб Azure Information Protection, Office и других служб Майкрософт может возвращать четко определенный набор [типов классификации.](/office365/securitycompliance/what-the-sensitive-information-types-look-for) Эти типы могут быть предоставлены API [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) для разрешения конфиденциальной информации на метку Microsoft Information Protection. 

## <a name="properties"></a>Свойства

| Свойство        | Тип  | Описание                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| confidenceLevel | Int32 | Уровень доверия от 0 до 100 результатов.                         |
| count           | Int32 | Количество экземпляров определенного типа сведений в вводе. |
| sensitiveTypeId | GUID  | GUID обнаруженного типа конфиденциальной информации.                 |

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