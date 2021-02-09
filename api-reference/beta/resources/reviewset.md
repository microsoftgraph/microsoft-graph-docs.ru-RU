---
title: Тип ресурса reviewSet
description: Представляет статический набор хранимой в электронном виде информации, собираемой для использования в судебных, расследованиях или нормативных запросах.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: b6234fafbf0d6e36d5dcbb4143956447e26d3a0f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153510"
---
# <a name="reviewset-resource-type"></a>Тип ресурса reviewSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет статический набор хранимой в электронном виде информации, собираемой для использования в судебных, расследованиях или нормативных запросах.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список reviewSet](../api/reviewset-list.md) | [Коллекция reviewSet](reviewset.md) | Получите коллекцию наборов для проверки. |
| [Get reviewSet](../api/reviewset-get.md) | [reviewSet](reviewset.md) | Чтение свойств и связей объекта **reviewSet.** |
| [Создание reviewSet](../api/reviewset-post.md) | [reviewSet](reviewset.md) | Создайте новый набор для проверки. |
| [Список запросов](../api/reviewsetquery-list.md)|[Коллекция reviewSetQuery](../resources/reviewsetquery.md)|Получите ресурсы reviewSetQuery из свойства навигации запросов.|
| [Создание запросов](../api/reviewsetquery-post.md)|[reviewSetQuery](../resources/reviewsetquery.md)|Создание объекта reviewSetQuery.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy        | [identitySet](/graph/api/resources/identityset) | Пользователь, создавший набор для проверки. Только для чтения. |
|createdDateTime  |DateTimeOffset| Дата и время создания набора для проверки. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|displayName      |String| Имя набора для проверки. Имя уникально с максимальным ограничением в 64 символа. |
|id               |String| Уникальный идентификатор набора для проверки. Только для чтения. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
| Проверка запроса набора |[Коллекция reviewSetQuery](reviewsetquery.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSet",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSet",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
