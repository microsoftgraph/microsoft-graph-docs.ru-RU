---
title: Тип ресурса Акцесспаккажеассигнментрекуест
description: Запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7d7fcf663abf15478b0c2745e9c60e1021d1ee7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508550"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>Тип ресурса Акцесспаккажеассигнментрекуест

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access. Если запрос выполнен успешно, при наличии необходимых утверждений пользователь получает назначение пакета Access и является темой этого назначенного пакета доступа.  Кроме того, Azure AD автоматически создает запросы на отправку для отслеживания удаления.


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Акцесспаккажеассигнментрекуестс](../api/accesspackageassignmentrequest-list.md) | Коллекция [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md) | Получение списка объектов акцесспаккажеассигнментрекуест. |
| [Создание Акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md) | [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md) | Создание нового Акцесспаккажеассигнментрекуест. |
| [Получение Акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-get.md) | [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md) | Чтение свойств и связей объекта Акцесспаккажеассигнментрекуест. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|комплетеддате|DateTimeOffset|Дата завершения обработки (успешное или неудачное) запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|id|String| Только для чтения.|
|исвалидатиононли|Логический|Имеет значение true, если запрос не обрабатывается для назначения.|
|текста|String|Выставляемое по запросу обоснование.|
|рекуестстате|String|Один из `Denied`, `Delivered` `PartiallyDelivered`, `Submitted` или `Scheduled`. Только для чтения.|
|рекуестстатус|String|Дополнительные сведения о состоянии обработки запроса. Только для чтения.|
|requestType|String|Один из `UserAdd`, `UserRemove` `AdminAdd`, `AdminRemove` или `SystemRemove`. Только для чтения.|
|акцесспаккажеассигнмент|[акцесспаккажеассигнмент](accesspackageassignment.md)| Требуется создать назначение пакета Access.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|опросчика|[акцесспаккажесубжект](accesspackagesubject.md)| Тема, которая запросила или, если назначено прямое назначение, было назначено. Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "2020-02-12T22:06:58.303Z",
  "completedDate": "2020-02-12T22:14:28.19Z",
  "id": "1244d439-5baa-4b9a-be5f-e8fdef5a998b",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "justification": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
