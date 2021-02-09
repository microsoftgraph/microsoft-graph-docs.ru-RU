---
title: Тип ресурса accessPackageResourceRequest
description: Запрос на доступ к пакету доступа — это запрос на добавление ресурса в каталог, чтобы роли ресурса можно было использовать в одном или более пакетах доступа каталога.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 16198df73c51b1b5f7cb7f8c7748da4816800890
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158585"
---
# <a name="accesspackageresourcerequest-resource-type"></a>Тип ресурса accessPackageResourceRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами [Azure AD](entitlementmanagement-root.md)запрос на доступ к пакету доступа — это запрос на добавление ресурса в каталог, чтобы роли ресурса можно было использовать в одном или более пакетах доступа каталога, или удалить ресурс из каталога, который больше не нужен пакетам доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md) | [Коллекция accessPackageResourceRequest](accesspackageresourcerequest.md) | Получить список объектов **accessPackageResourceRequest.** |
| [Создание accessPackageResourceRequest](../api/accesspackageresourcerequest-post.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Создание объекта **accessPackageResourceRequest.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|catalogId|String|Уникальный ИД каталога пакетов доступа.|
|expirationDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения.|
|isValidationOnly|Boolean|Если этот набор за установлен, ресурс не добавляется.|
|обоснование|String|Обоснование запросителя для добавления или удаления ресурса.|
|requestState|String| Результат того, удалось ли службе добавить ресурс в каталог.  Значением является `Delivered` то, был ли добавлен или удален ресурс. Только для чтения.|
|requestStatus|String|Только для чтения.|
|requestType|String|Используется для добавления ресурса, если вызываемая является администратором или владельцем ресурса, или `AdminAdd` `AdminRemove` для удаления ресурса. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageResource|[accessPackageResource](accesspackageresource.md)| Допускается значение null.|
|requestor|[accessPackageSubject](accesspackagesubject.md)| Только для чтения. Допускается значение null.|

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


