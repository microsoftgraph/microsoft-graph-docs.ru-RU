---
title: Тип ресурса Персонанниверсари
description: Тип ресурса Персонанниверсари
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7dad5536eb78b2d7119ace63eb0f7ce16880e85f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521927"
---
# <a name="personanniversary-resource-type"></a>Тип ресурса Персонанниверсари

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о значимых датах, связанных с пользователем в [профиле](profile.md)пользователя.

Наследуется от [итемфацет](itemFacet.md).

## <a name="methods"></a>Методы

| Метод                                                   | Возвращаемый тип                               | Описание                                                    |
|:---------------------------------------------------------|:------------------------------------------|:---------------------------------------------------------------|
| [Получение Персонанниверсари](../api/personanniversary-get.md) | [персонанниверсари](personanniversary.md) | Чтение свойств и связей объекта **персонанниверсари** . |
| [обновление](../api/personanniversary-update.md).             | [персонанниверсари](personanniversary.md) | Обновление объекта **персонанниверсари** .                               |
| [удаление](../api/personanniversary-delete.md);             | Нет                                      | Удаление объекта **персонанниверсари** .                               |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|date          |Date         | Содержит дату, связанную с типом юбилея.         |
|type          |string       | Возможные значения: `birthday`, `wedding`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON. 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personAnniversary",
  "baseType": ""
}-->

```json
{
  "date": "String (timestamp)",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personAnniversary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
