---
title: Тип ресурса Акцесспаккажересаурцерекуест
description: Запрос ресурса пакета Access — это запрос на Добавление ресурса в каталог, чтобы роли ресурса можно было использовать в одном или нескольких пакетах доступа каталога.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 74cc7815d4df22c1914f525ed0451b778c7777d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508522"
---
# <a name="accesspackageresourcerequest-resource-type"></a>Тип ресурса Акцесспаккажересаурцерекуест

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)запрос ресурса пакета Access является запросом на Добавление ресурса к каталогу, чтобы роли ресурса можно было использовать в одном или нескольких пакетах доступа каталога.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Акцесспаккажересаурцерекуестс](../api/accesspackageresourcerequest-list.md) | Коллекция [акцесспаккажересаурцерекуест](accesspackageresourcerequest.md) | Получение списка объектов **акцесспаккажересаурцерекуест** . |
| [Создание Акцесспаккажересаурцерекуест](../api/accesspackageresourcerequest-post.md) | [акцесспаккажекаталог](accesspackageresourcerequest.md) | Создание нового объекта **акцесспаккажересаурцерекуест** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|каталогид|String|Уникальный идентификатор каталога пакетов Access.|
|expirationDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения.|
|исвалидатиононли|Логический|Если этот параметр установлен, ресурс не добавляется.|
|текста|String|Обоснование запрашивающей стороны для добавления ресурса.|
|рекуестстате|String| Результат того, удалось ли службе добавить ресурс в каталог.  Значение, `Delivered` если ресурс был добавлен. Только для чтения.|
|рекуестстатус|String|Только для чтения.|
|requestType|String|Используйте `AdminAdd` для добавления ресурса, если вызывающий абонент является администратором или владельцем ресурса. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|акцесспаккажересаурце|[акцесспаккажересаурце](accesspackageresource.md)| Допускается значение null.|
|опросчика|[акцесспаккажесубжект](accesspackagesubject.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "expirationDateTime": "String (timestamp)",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "String",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
