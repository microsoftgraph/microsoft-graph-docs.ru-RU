---
title: тип ресурса audioConferencing
description: Представляет сведения о доступе к телефону для собрания в Интернете.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 98daa0db87c86625581c30e558f851d7cfa075f8
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220425"
---
# <a name="audioconferencing-resource-type"></a>тип ресурса audioConferencing

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о доступе к телефону для [onlineMeeting.](onlinemeeting.md)

## <a name="properties"></a>Свойства

| Свойство                    | Тип              | Описание                                                                    |
| :-------------------------- | :---------------- | :----------------------------------------------------------------------------- |
| dialinUrl                   | Строка            | URL-адрес веб-страницы, доступной извне, который содержит сведения о диалоговом номере. |
| conferenceId                | String            | ID конференции собрания в Интернете.                                       |
| tollFreeNumbers             | Коллекция строк | Список бесплатных номеров, отображаемого в приглашении на собрание.            |
| tollNumbers                 | Коллекция строк | Список номеров платных номеров, отображаемого в приглашении на собрание.                 |
| tollFreeNumber (обесценилось) | Строка            | Бесплатный номер, подключенный к поставщику аудиоконференции.           |
| tollNumber (износ)     | String            | Платный номер, который подключается к поставщику аудиоконференции.                |

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
  "tollFreeNumbers": [ "String" ],
  "tollNumbers": [ "String" ]
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


