---
title: Тип ресурса changeNotificationCollection
description: Представляет коллекцию уведомлений о подписке, отправленных абоненту.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 74af713c082cb8070b2329785647274c29c259bb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335397"
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
| validationTokens | Коллекция (string) | Содержит массив маркеров JWT, созданных корпорацией Майкрософт Graph для приложения для проверки происхождения уведомлений. Microsoft Graph создает один маркер для каждого отдельного приложения и пары клиента для элемента, если он существует в массиве значений. Имейте в виду, что уведомления могут содержать сочетание элементов для различных приложений и клиентов, которые подписывались с помощью одного и того же URL-адреса уведомлений. Только для [уведомлений об изменениях с данными ресурса Необязательный](/graph/webhooks-with-resource-data.md) . |
| значение | collection([changeNotification](changenotification.md)) | Набор уведомлений, отосланных на URL-адрес уведомления. Обязательный. |

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
``` json
{
  "@odata.type": "#microsoft.graph.changeNotificationCollection",
  "validationTokens": [
    "String"
  ],
  "value": [
    {
      "@odata.type": "microsoft.graph.changeNotification"
    }
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

