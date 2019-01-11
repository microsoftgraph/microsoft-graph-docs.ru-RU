---
title: Тип ресурса profilePhoto
description: Фотографий профиля пользователя, группы или контакта Outlook доступ из Exchange Online или Azure Active Directory (AAD). Это не кодируются в-64 двоичных данных.
localization_priority: Normal
ms.openlocfilehash: 7754d70c4e59b13b1b0003022ddc0f185cc18ae2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837072"
---
# <a name="profilephoto-resource-type"></a>Тип ресурса profilePhoto

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
|id|строка|Только для чтения.|
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
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
