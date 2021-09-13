---
title: тип ресурса resourceData
description: Представляет данные resouce, присоединенные к уведомлению об изменении, отправленным абоненту.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 4fef5e2564cbad29a3b998d11b2f4870663e7a7e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094088"
---
# <a name="resourcedata-resource-type"></a>тип ресурса resourceData

Пространство имен: microsoft.graph

Представляет данные resouce, присоединенные к уведомлению об изменении, отправленным абоненту.

Подробности см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Для Outlook **ресурсов resourceData содержит** следующие поля:

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| @odata.type | строка | @odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект. |
| @odata.id | строка | @odata.id — идентификатор OData для объекта. |
| @odata.etag | строка | @odata.etag — HTTP-тег сущности, представляющий версию объекта. |
| id | строка | Идентификатор объекта. |

> **Примечание:** Значение, `id` предоставляемого **в resourceData,** допустимо на момент сгенерировании уведомления об изменении. Некоторые действия, например перенос сообщения в другую папку, могут привести к неодержительным действиям при обработке `id` уведомления об изменении.

## <a name="relationships"></a>Отношения

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

