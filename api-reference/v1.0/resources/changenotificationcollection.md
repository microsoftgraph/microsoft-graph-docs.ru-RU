---
title: Тип ресурса changeNotificationCollection
description: Представляет коллекцию уведомлений о подписке, отправленных абоненту.
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: f4fd69bca39042c00630d21905e26d587b8d3ad8b0d014656eb2e9cf6a57d342
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189897"
---
# <a name="changenotificationcollection-resource-type"></a>Тип ресурса changeNotificationCollection

Пространство имен: microsoft.graph

Представляет коллекцию уведомлений об изменении ресурсов, отправленных абоненту.

Подробности см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| validationTokens | Коллекция (string) | Содержит массив маркеров JWT, созданных корпорацией Майкрософт Graph для приложения для проверки происхождения уведомлений. Microsoft Graph создает один маркер для каждого отдельного приложения и пары клиента для элемента, если он существует в массиве значений. Имейте в виду, что уведомления могут содержать сочетание элементов для различных приложений и клиентов, которые подписывались с помощью одного и того же URL-адреса уведомлений. Только для [уведомлений об изменениях с данными ресурса Необязательный.](/graph/webhooks-with-resource-data.md) |
| значение | [collection(changeNotification)](changenotification.md) | Набор уведомлений, отосланных на URL-адрес уведомления. Обязательный. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationCollection"
}-->

```json
{
  "value": [],
  "validationTokens": [
    "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
  ]
}
```

<!-- uuid: 8cc2599e-9740-4191-93fa-bc13c6f91564
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification collection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

