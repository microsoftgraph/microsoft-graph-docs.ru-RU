---
title: тип ресурса audioConferencing
description: Представляет сведения о доступе к телефону для собрания в Интернете.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9462971d1c2694b3443c9b3a4e799a24362eee80
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515641"
---
# <a name="audioconferencing-resource-type"></a>тип ресурса audioConferencing

Пространство имен: microsoft.graph

Представляет сведения о доступе к телефону для [onlineMeeting.](onlinemeeting.md)

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | Строка  | URL-адрес веб-страницы, доступной извне, который содержит сведения о диалоговом номере. |
| conferenceId        | Строка  | ID конференции собрания в Интернете.      |
| tollFreeNumber      | Строка  | Бесплатный номер, подключенный к поставщику аудиоконференции.              |
| tollNumber          | Строка  | Платный номер, который подключается к поставщику аудиоконференции.                   |

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
  "tollFreeNumber": "String",
  "tollNumber": "String"
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

