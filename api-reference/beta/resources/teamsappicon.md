---
title: тип ресурса teamsAppIcon
description: Значок, связанный с приложением в Microsoft Teams.
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3e8a256dc0b9e92c414cd3d362bb36579708083f
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882713"
---
# <a name="teamsappicon-resource-type"></a>тип ресурса teamsAppIcon

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Значок, связанный с [teamsApp.](teamsapp.md)

## <a name="methods"></a>Методы

| Метод                                            | Возвращаемый тип                                       | Описание                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [Получить значок](../api/teamsappicon-get.md)     | [teamsAppIcon](teamsappicon.md)                   | Получите значок, связанный с определенной версией приложения Teams. |
| [Получить контент с хост-контентом](../api/teamworkhostedcontent-get.md) | [teamworkHostedContent](teamworkhostedcontent.md) | Получите у себя содержимое (и его bytes) для значка.                |

## <a name="properties"></a>Свойства

| Свойство      | Тип                        | Описание                                                                             |
| :------------ | :-------------------------- | :-------------------------------------------------------------------------------------- |
| id            | string                      | Уникальный ID значка приложения.                                                          |
| webUrl        | string                      | Веб-URL-адрес, который можно использовать для скачивания изображения.                                 |

## <a name="relationships"></a>Связи

| Связь  | Тип                                              | Описание                                                                         |
| :------------ | :------------------------------------------------ | :---------------------------------------------------------------------------------- |
| hostedContent | [teamworkHostedContent](teamworkhostedcontent.md) | Содержимое значка приложения, если значок находится в инфраструктуре Teams. |

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppIcon",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "webUrl": "string"
}
```

## <a name="see-also"></a>См. также

- [teamsApp](teamsapp.md)
- [teamsAppDefinition](teamsappdefinition.md)
