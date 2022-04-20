---
title: Тип ресурса contentSharingSession
description: Представляет сеанс общего доступа к содержимому в вызове.
author: satyakonmsft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5d642350b3fe5e6b1edf5e35dbc3cb5a1f677aea
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917968"
---
# <a name="contentsharingsession-resource-type"></a>Тип ресурса contentSharingSession

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сеанс общего доступа к содержимому в вызове.

## <a name="methods"></a>Методы

| Метод                                                             | Возвращаемый тип                                                 | Описание                                                                     |
|:-------------------------------------------------------------------|:------------------------------------------------------------|:--------------------------------------------------------------------------------|
| [Получение contentSharingSession](../api/contentsharingsession-get.md )                                     | [contentSharingSession](contentsharingsession.md)                                             | Получение свойств объекта **contentSharingSession** .                                         |
| [Перечисление contentSharingSessions](../api/call-list-contentsharingsessions.md )              | [Коллекция contentSharingSession](contentsharingsession.md)                    | Получение списка объектов **contentSharingSession** в вызове.                                            |

## <a name="properties"></a>Свойства

|Свойство                 |Тип                      |Описание                                                                        |
|:---                     |:---                      |:---                                                                               |
| id                      | String                   | Уникальный идентификатор сеанса общего доступа к содержимому. Только для чтения. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.contentSharingSession"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contentSharingSession",
  "id": "String(identifier)"
}
```
