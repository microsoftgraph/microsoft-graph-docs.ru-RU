---
title: Тип ресурса Усерпурпосе
description: Представляет получателя или тип почтового ящика пользователя в Exchange Online.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 83abf3bd19434867bbd162b6260ed5f4445d8ffd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057845"
---
# <a name="userpurpose-resource-type"></a>Тип ресурса Усерпурпосе

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Назначение почтового ящика. Используется для различения почтового ящика одного пользователя из общего почтового ящика и почтового ящика оборудования в Exchange Online.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|значение|[маилбоксреЦипиенттипе](#mailboxrecipienttype-values)|Представляет получателя или тип почтового ящика пользователя в Exchange Online. Возможные значения: `unknown` ,, `user` , `linked` , `shared` `room` , `equipment` и `others` . Более подробную информацию можно найти в следующем разделе.|

### <a name="mailboxrecipienttype-values"></a>значения МаилбоксреЦипиенттипе
|Member|Описание|
|:---------------|:--------|
|unknown|Сведения о почтовом ящике не найдены.|
|user|Учетная запись пользователя с почтовым ящиком в локальном лесе.|
|вязывает|Почтовый ящик, связанный с учетной записью пользователя в другом лесе.|
|общие|Почтовые ящики, используемые двумя или более учетными записями пользователей.|
|отеле|Почтовый ящик, представляющий комнату переговоров.|
|перифери|Почтовый ящик, представляющий компонент оборудования.|
|владельцев|Найден почтовый ящик, но цель пользователя отличается от указанных выше.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userPurpose"
}-->

```json
{
    "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userPurpose resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


