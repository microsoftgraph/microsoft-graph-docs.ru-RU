---
title: Тип ресурса outOfOfficeSettings
description: Представляет сведения о доступе по телефону для собрания по сети.
author: elvinyang-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4e3e179ec752cfffc4ae4711d9fd0bc541f1506d
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796783"
---
# <a name="outofofficesettings-resource-type"></a>Тип ресурса outOfOfficeSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры "Нет на месте", связанные с [присутствием](presence.md) пользователя.

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| message           | String  | Сообщение об простое, настроенное пользователем в клиенте Outlook (автоматические ответы (нет на офисе) или клиенте Teams (запланировать выход из офиса). |
| isOutOfOffice      | Логический  | True, если один из них:</br><ul><li>В настоящее время он находится в периоде простоя, настроенного в клиенте Outlook или Teams.</li><li>В настоящее время в календаре пользователя есть событие, помеченное как "Показать как нет на офисе"</li></ul></br>В противном случае false. |

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
