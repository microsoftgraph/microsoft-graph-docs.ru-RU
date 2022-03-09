---
title: Тип ресурса rbacApplication
description: Контейнер для определений ролей и назначений ролей для Microsoft 365 для поставщиков управления доступом на основе ролей (RBAC)
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 294bf357465002a180549e5654fbfd7f2baabac6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393475"
---
# <a name="rbacapplication-resource-type"></a>Тип ресурса rbacApplication

Пространство имен: microsoft.graph

Контейнер управления ролью для унифицированных определений ролей и назначений ролей для Microsoft 365 для поставщиков управления доступом на основе ролей (RBAC). Назначения ролей поддерживают только одну главу и одну область. В **настоящее время** каталог **и entitlementManagement** — это два поддерживаемых поставщика RBAC.

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|roleAssignments|[коллекция unifiedRoleAssignment](../resources/unifiedroleassignment.md)| Ресурс для предоставления доступа пользователям или группам. |
|roleDefinitions|[коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Ресурс, представляющий роли, разрешенные поставщиками RBAC, и разрешения, присвоенные ролям. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rbacApplication",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rbacApplication"
}
```
