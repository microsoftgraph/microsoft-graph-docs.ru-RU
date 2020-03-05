---
title: Тип ресурса Классификатионресулт
description: Представляет результат запроса классификации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5281156752ceb290772daf841530b4ddb80350d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507665"
---
# <a name="classificationresult-resource-type"></a>Тип ресурса Классификатионресулт

Пространство имен: Microsoft. Graph

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
