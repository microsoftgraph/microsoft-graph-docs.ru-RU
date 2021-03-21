---
title: тип ресурса outOfOfficeSettings
description: Представляет сведения о доступе к телефону для собрания в Интернете.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 018852150ef833d8cb114892790f911b4aad8fe0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960384"
---
# <a name="outofofficesettings-resource-type"></a>тип ресурса outOfOfficeSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры из офиса, связанные с [присутствием](presence.md) пользователя.

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| message           | String  | Сообщение из офиса, настроенное пользователем в клиенте Outlook (Автоматические ответы (вне Office)) или клиенте Teams (Расписание вне офиса). |
| isOutOfOffice      | Boolean  | True, если либо:</br><ul><li>В настоящее время он находится в окне вне офиса, настроенном на клиент Outlook или Teams.</li><li>В настоящее время в календаре пользователя имеется событие, помеченное как Show as Out of Office</li></ul></br>В противном случае, false. |

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
