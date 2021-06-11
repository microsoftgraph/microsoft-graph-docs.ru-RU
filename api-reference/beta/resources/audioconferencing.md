---
title: тип ресурса audioConferencing
description: Представляет сведения о доступе к телефону для собрания в Интернете.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5f0c9338aefa592ed030585a6b0342d03e7717d0
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896699"
---
# <a name="audioconferencing-resource-type"></a>тип ресурса audioConferencing

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о доступе к телефону для [onlineMeeting.](onlinemeeting.md)

## <a name="properties"></a>Свойства

| Свойство                    | Тип              | Описание                                                                    |
| :-------------------------- | :---------------- | :----------------------------------------------------------------------------- |
| dialinUrl                   | String            | URL-адрес веб-страницы, доступной извне, который содержит сведения о диалоговом номере. |
| conferenceId                | String            | ID конференции собрания в Интернете.                                       |
| tollFreeNumber (обесценилось) | String            | Бесплатный номер, подключенный к поставщику аудиоконференции.           |
| tollFreeNumbers             | Коллекция String | Список бесплатных номеров, отображаемого в приглашении на собрание.            |
| tollNumber (износ)     | String            | Платный номер, который подключается к поставщику аудиоконференции.                |
| tollNumbers                 | Коллекция String | Список номеров платных номеров, отображаемого в приглашении на собрание.                 |

> [!CAUTION]
>
>- Свойства **tollFreeNumber** и **tollNumber** обесценяются. Вместо этого **используйте свойства tollFreeNumbers** **и tollNumbers.**
>- Для обратной совместимости исходный **tollFreeNumber** добавляется в новую коллекцию **tollFreeNumbers,** а исходный **tollNumber** добавляется в новую коллекцию **tollNumbers.**

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "conferenceId": "String",
  "tollFreeNumbers": ["String"],
  "tollNumbers": ["String"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


