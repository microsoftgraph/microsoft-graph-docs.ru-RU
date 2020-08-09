---
title: Тип ресурса resourceData
description: Представляет данные ресурсов, вложенные в уведомление об изменении, отправляемое подписчику.
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: c9da2041a6d982556ec909375ff46b3a9b3e2e2d
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598405"
---
# <a name="resourcedata-resource-type"></a>Тип ресурса resourceData

Пространство имен: microsoft.graph

Представляет данные ресурсов, вложенные в уведомление об изменении, отправляемое подписчику.

Дополнительные сведения см. [в статье Использование API Microsoft Graph для получения уведомлений об изменениях](webhooks.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Для ресурсов Outlook **resourceData** содержит следующие поля:

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| @odata.type | строка | @odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект. |
| @odata.id | строка | @odata.id — идентификатор OData для объекта. |
| @odata.etag | строка | @odata.etag — HTTP-тег сущности, представляющий версию объекта. |
| id | строка | Идентификатор объекта. |

> **Примечание:** `id`Значение, указанное в **resourceData** , является допустимым во время создания уведомления об изменении. Некоторые действия, например перемещение сообщения в другую папку, могут привести к `id` недействительности при обработке уведомления об изменении.

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceData"
}-->

```json
{
  "id": "1565293727947",
  "@odata.type": "#Microsoft.Graph.ChatMessage",
  "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
}
```

<!-- uuid: eb6c98ec-8257-4826-910e-5c603265257f
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource data resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
