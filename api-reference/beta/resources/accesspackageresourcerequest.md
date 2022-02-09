---
title: тип ресурса accessPackageResourceRequest
description: Запрос ресурса пакета доступа — это запрос на добавление ресурса в каталог, чтобы роли ресурса можно было использовать в одном или более пакетах доступа каталога.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9f6557a4256b692005c82ca18bc93041f003b886
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468300"
---
# <a name="accesspackageresourcerequest-resource-type"></a>тип ресурса accessPackageResourceRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-overview.md) запрос ресурсов пакета доступа — это запрос на добавление ресурса [](accesspackageresource.md) в каталог, чтобы роли ресурса можно было использовать в одном или несколько пакетах доступа каталога, или удалить ресурс из каталога, который больше не нужен пакетам доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список accessPackageResourceRequests](../api/entitlementmanagement-list-accesspackageresourcerequests.md) | [коллекция accessPackageResourceRequest](accesspackageresourcerequest.md) | Извлечение списка **объектов accessPackageResourceRequest** . |
| [Создание accessPackageResourceRequest](../api/entitlementmanagement-post-accesspackageresourcerequests.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Создание нового **объекта accessPackageResourceRequest** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|catalogId|Строка|Уникальный ID каталога пакетов доступа.|
|expirationDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|id|String| Только для чтения.|
|isValidationOnly|Логическое|Если установлено, ресурс не добавляется.|
|обоснование|Строка|Обоснование запроса для добавления или удаления ресурса.|
|requestState|Строка| Результат того, удалось ли службе добавить ресурс в каталог.  Значение, если `Delivered` ресурс был добавлен или удален. Только для чтения.|
|requestStatus|String|Только для чтения.|
|requestType|String|Используйте `AdminAdd` для добавления ресурса, если вызываемая является администратором или владельцем ресурса, `AdminRemove` или для удаления ресурса. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageResource|[accessPackageResource](accesspackageresource.md)| Допускается значение null.|
|запросчик|[accessPackageSubject](accesspackagesubject.md)| Только для чтения. Допускается значение null. Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
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


