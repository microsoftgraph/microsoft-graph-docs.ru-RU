---
title: тип ресурса outOfOfficeSettings
description: Представляет сведения о доступе к телефону для собрания в Интернете.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 13f826babea1e6f9448d1ecb9b8100baaf962b20
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896636"
---
# <a name="outofofficesettings-resource-type"></a>тип ресурса outOfOfficeSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры из офиса, связанные с [присутствием](presence.md) пользователя.

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| message           | String  | Неявное сообщение, настроенное пользователем на Outlook клиенте (Автоматические ответы (вне Office)) или клиенте Teams (Расписание вне офиса). |
| isOutOfOffice      | Boolean  | True, если либо:</br><ul><li>В настоящее время он находится в неявном окне времени, настроенном на Outlook или Teams клиенте.</li><li>В настоящее время в календаре пользователя имеется событие, помеченное как Show as Out of Office</li></ul></br>В противном случае, false. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.outOfOfficeSettings"
}-->
```json
{
  "message": "String",
  "isOutOfOffice": "Boolean"
}
```
