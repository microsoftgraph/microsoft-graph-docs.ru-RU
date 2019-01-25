---
title: Тип ресурса profilePhoto
description: Фотографий профиля пользователя, группы или контакта Outlook доступ из Exchange Online или Azure Active Directory (AAD). Это не кодируются в-64 двоичных данных.
localization_priority: Normal
ms.openlocfilehash: 2a831abd098fb9a0dfa95f6d6dd3a9cd5de128cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513657"
---
# <a name="profilephoto-resource-type"></a>Тип ресурса profilePhoto

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Фотографий профиля пользователя, группы или контакта Outlook доступ из Exchange Online или Azure Active Directory (AAD). Это не кодируются в-64 двоичных данных.

Поддерживаемые размеры фотографий в формате HD для Exchange Online: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 и 648x648. На AAD фотографии может быть любой измерения.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение объекта profilePhoto](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) |Получите указанный **profilePhoto** или метаданных (**profilePhoto** свойства). |
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
  "suppressions": [
    "Error: /api-reference/beta/resources/profilephoto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
