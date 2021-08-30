---
title: Тип ресурса удостоверений
description: Представляет идентификатор, используемый для набора разрешений на внешний контент, добавленный в Microsoft Graph.
author: sacampbe-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 94733a3e9d6595341a515ff525cdf90050f41b4a
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697515"
---
# <a name="identity-resource-type"></a>Тип ресурса удостоверений

Пространство имен: microsoft.graph.externalConnectors

Представляет [идентификатор, используемый](externalconnectors-identity.md) для набора разрешений на внешний контент, добавленный в Microsoft Graph.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание удостоверений](../api/externalconnectors-externalgroup-post-members.md)|[identity](externalconnectors-identity.md)|Создание ресурса [удостоверений](../resources/externalconnectors-identity.md) для нового участника в [externalGroup.](../resources/externalconnectors-externalgroup.md)|
|[Удаление удостоверений](../api/externalconnectors-identity-delete.md)|Нет|Удалите [ресурс удостоверений,](../resources/externalconnectors-identity.md) чтобы удалить соответствующий член из [externalGroup.](../resources/externalconnectors-externalgroup.md)|

## <a name="properties"></a>Свойства

| Свойство       | Тип                    | Описание                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | String                  | Уникальный идентификатор удостоверения. Это будет свойство objectId в случае Azure Active Directory пользователей или групп Azure AD, а также свойство **id** **externalGroup** в случае внешних групп.                                    |
| type           | microsoft.graph.externalConnectors.identityType | Тип удостоверения. Возможные значения: `user` или `group` для удостоверений Azure AD и для групп во внешней `externalgroup` системе. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.identity",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "type": "String"
}
```
