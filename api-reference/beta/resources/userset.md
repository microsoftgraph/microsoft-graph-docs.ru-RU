---
title: сложный тип User
description: Абстрактный базовый тип для типов, используемых в параметрах просмотра запроса, утверждения и назначения для политики назначения пакетов Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aabd0716990f67d0b73b4bb300b6953caa0bfe07
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057810"
---
# <a name="userset-complex-type"></a>сложный тип User

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах просмотра запроса, утверждения и назначения для [политики назначения пакетов Access](accesspackageassignmentpolicy.md). Абстрактный базовый тип для типов [SingleUser.](singleuser.md),[граупмемберс](groupmembers.md), [коннектедорганизатионмемберс](connectedorganizationmembers.md), [рекуесторманажер](requestormanager.md), [интерналспонсорс](internalsponsors.md)и [екстерналспонсорс](externalsponsors.md) .

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| Создание резервной копии | Boolean | Для пользователя на этапе утверждения данное свойство указывает, является ли пользователь утверждающим резервной копии. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено представление объекта User в формате JSON.  Обратите внимание, что пользовательский набор является абстрактным базовым классом, и поэтому не может быть отправлен или получен.  Вместо этого используется один из `@odata.type` " `#microsoft.graph.singleUser` ", " `#microsoft.graph.groupMembers` ", " `#microsoft.graph.connectedOrganizationMembers` ", " `#microsoft.graph.requestorManager` ", " `#microsoft.graph.internalSponsors` " или " `#microsoft.graph.externalSponsors` ".

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSet",
  "baseType": ""
}-->

```json
{
       "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSet complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


