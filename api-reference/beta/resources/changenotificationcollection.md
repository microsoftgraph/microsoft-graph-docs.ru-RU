---
title: Тип ресурса Чанженотификатионколлектион
description: Представляет коллекцию уведомлений о подписке, отправляемых подписчику.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 583a6444fb7f0f1be65c68a4eb772089ddb768bd
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/30/2020
ms.locfileid: "44430612"
---
# <a name="changenotificationcollection-resource-type"></a>Тип ресурса Чанженотификатионколлектион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию уведомлений о подписке, отправляемых подписчику.

Дополнительные сведения см. [в статье Использование API Microsoft Graph для получения уведомлений об изменениях](webhooks.md).

## <a name="methods"></a>Методы

Отсутствуют.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| валидатионтокенс | Коллекция (string) | Содержит массив маркеров JWT, созданных приложением Microsoft Graph для проверки источника уведомлений. Microsoft Graph создает один маркер для каждой отдельной пары приложения и клиента, для которой существует элемент в массиве value. Имейте в виду, что уведомления могут содержать набор элементов для различных приложений и клиентов, подписанных с использованием того же URL-адреса уведомления. Предоставляется только для [уведомлений об изменениях с данными ресурсов](/graph/webhooks-with-resource-data.md) . |
| значение | Коллекция ([чанженотификатион](changenotification.md)) | Набор уведомлений, отправляемых на URL-адрес уведомлений. Обязательный элемент. |

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
