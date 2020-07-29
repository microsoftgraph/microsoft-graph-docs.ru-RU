---
title: Тип ресурса Коннектедорганизатион
description: В управлении службой управления правами Azure AD подключенная организация является ссылкой на каталог или домен другой организации, чьи пользователи могут запрашивать доступ.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cb82ac88f1f81bf7d2f3238657818d0782ed6b60
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510364"
---
# <a name="connectedorganization-resource-type"></a>Тип ресурса Коннектедорганизатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)подключенная организация является ссылкой на каталог или домен другой организации, чьи пользователи могут запрашивать доступ.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Коннектедорганизатионс](../api/connectedorganization-list.md) | Коллекция [коннектедорганизатион](connectedorganization.md) | Получение списка объектов Коннектедорганизатион. |
|[Создание Коннектедорганизатион](../api/connectedorganization-post.md) | [коннектедорганизатион](connectedorganization.md) | Создание нового объекта Коннектедорганизатион. |
|[Получение Коннектедорганизатион](../api/connectedorganization-get.md) | [коннектедорганизатион](connectedorganization.md) | Чтение свойств и связей объекта Коннектедорганизатион. |
|[Обновление Коннектедорганизатион](../api/connectedorganization-update.md) | | Обновление Коннектедорганизатион. |
|[Удаление Коннектедорганизатион](../api/connectedorganization-delete.md) |Нет | Удаление объекта Коннектедорганизатион. |

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|Строка|Имя участника-пользователя, создавшего этот ресурс. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|description|String|Описание подключенной Организации.|
|displayName|Строка|Отображаемое имя подключенной Организации.|
|id|String| Только для чтения.|
|модифиедби|Строка|Имя участника-пользователя, который последним изменил этот ресурс. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|

## <a name="relationships"></a>Отношения

|Связь|Тип|Описание|
|:---|:---|:---|
|идентитисаурцес|Коллекция [идентитисаурце](identitySource.md)| Источники удостоверений в этой подключенной Организации, один из [азуреактиведиректоритенант](azureactivedirectorytenant.md), [домаинидентитисаурце](domainidentitysource.md) или [екстерналдомаинфедератион](externaldomainfederation.md). Только для чтения. Допускается значение null.|
|интерналспонсорс| Коллекция [directoryObject](directoryobject.md)| Допускается значение null.|
|екстерналспонсорс| Коллекция [directoryObject](directoryobject.md)| Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectedOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "identitySources": [
    {
      "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
      "tenantId": "String (identifier)",
      "displayName": "String"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
