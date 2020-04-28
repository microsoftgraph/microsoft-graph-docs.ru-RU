---
title: Тип ресурса Персонанниверсари
description: Тип ресурса Персонанниверсари
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c8ea4e9bf7db268c5ec6bffad1c7d43cbbdd2439
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227733"
---
# <a name="personanniversary-resource-type"></a>Тип ресурса Персонанниверсари

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о значимых датах, связанных с пользователем в [профиле](profile.md)пользователя.

Наследуется от [итемфацет](itemFacet.md).

## <a name="methods"></a>Методы

| Метод                                                   | Возвращаемый тип                               | Описание                                                              |
|:---------------------------------------------------------|:------------------------------------------|:-------------------------------------------------------------------------|
| [Получение Персонанниверсари](../api/personanniversary-get.md) | [персонанниверсари](personanniversary.md) | Чтение свойств и связей объекта **персонанниверсари** . |
| [обновление](../api/personanniversary-update.md).             | [персонанниверсари](personanniversary.md) | Обновление объекта **персонанниверсари** .                                   |
| [удаление](../api/personanniversary-delete.md);             | Нет                                      | Удаление объекта **персонанниверсари** .                                   |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|date          |Date         | Содержит дату, связанную с типом юбилея.          |
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
