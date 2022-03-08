---
title: тип ресурса resourceData
description: Представляет данные resouce, присоединенные к уведомлению об изменении, отправленным абоненту.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 87fcd715bce5a58d3503ef48e43eebcca088cc9d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336755"
---
# <a name="resourcedata-resource-type"></a>тип ресурса resourceData

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные resouce, присоединенные к уведомлению об изменении, отправленным абоненту. Этот ресурс является открытым типом и позволяет передавать другие свойства.

Подробности см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет, кроме Outlook ресурсов, в которых **resourceData** содержит следующие поля:

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| @odata.type | Строка | @odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект. |
| @odata.id | Строка | @odata.id — идентификатор OData для объекта. |
| @odata.etag | Строка | @odata.etag — HTTP-тег сущности, представляющий версию объекта. |
| id | Строка | Идентификатор объекта. |

> **Примечание:** Значение **id** , предоставляемого **в resourceData** , допустимо на момент сгенерировании уведомления об изменении. Некоторые действия, например перенос сообщения в другую папку, `id` могут привести к неодержительным действиям при обработке уведомления об изменении.

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "@odata.type",
    "@odata.id",
    "@odata.etag",
    "id"
  ],
  "@odata.type": "microsoft.graph.resourceData"
}-->

```json
{
  "@odata.type": "#microsoft.graph.resourceData"
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


