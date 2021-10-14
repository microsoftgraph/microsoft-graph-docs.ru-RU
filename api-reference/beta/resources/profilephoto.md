---
title: Тип ресурса profilePhoto
description: Фотография профиля пользователя, группы или Outlook, доступ к Exchange Online или Azure Active Directory (AAD). Это двоичные данные, не представленные в кодировке base-64.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: people
author: kevinbellinger
ms.openlocfilehash: f64f87c18bd6e5752671a6dbb28b8464f07cfa3a
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2021
ms.locfileid: "60355549"
---
# <a name="profilephoto-resource-type"></a>Тип ресурса profilePhoto

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Фотография профиля пользователя, группы или Outlook, доступ к Exchange Online или Azure Active Directory (AAD). Это двоичные данные, не представленные в кодировке base-64.

Поддерживаемые размеры фотографий в формате HD для Exchange Online: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 и 648x648. На AAD фотографии могут быть любого измерения.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение объекта profilePhoto](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) |Получение указанного объекта **profilePhoto** или его метаданных (свойств **profilePhoto**). |
|[Обновление](../api/profilephoto-update.md) | [profilePhoto](profilephoto.md)  |Назначение фотографии указанному пользователю, группе или контакту. Фотография должна быть представлена в двоичном формате. Она заменяет текущую фотографию (если она существует). |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Только для чтения.|
|height|int32|Высота фотографии. Только для чтения.|
|width|int32|Ширина фотографии. Только для чтения.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


