---
title: тип ресурса meetingRegistrantBase
description: Представляет регистратор базового собрания, который зарегистрировался на собрании в Интернете.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c17ccf2cb3b34b9b139726b727cd84148b6bc9a8
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565236"
---
# <a name="meetingregistrantbase-resource-type"></a>тип ресурса meetingRegistrantBase

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет регистратор базового собрания, который зарегистрировался на собрании в Интернете.

Базовый тип [meetingRegistrant](meetingregistrant.md) и [externalMeetingRegistrant](externalmeetingregistrant.md).

> [!TIP]
> Это абстрактный тип, который нельзя использовать напрямую. Вместо этого используйте производный [тип meetingRegistrant](meetingregistrant.md) или [externalMeetingRegistrant.](externalmeetingregistrant.md)

## <a name="properties"></a>Свойства

| Свойство   | Тип   | Описание                                                         |
|:-----------|:-------|:--------------------------------------------------------------------|
| id         | Строка | Уникальный идентификатор регистратора. Только для чтения.                 |
| joinWebUrl | Строка | Уникальный веб-URL-адрес для регистратора, который должен присоединиться к собранию. Только для чтения. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.meetingRegistrantBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.meetingRegistrantBase",
  "id": "String (identifier)",
  "joinWebUrl": "String"
}
```
