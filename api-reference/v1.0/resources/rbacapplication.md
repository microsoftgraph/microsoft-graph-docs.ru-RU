---
title: Тип ресурса rbacApplication
description: Контейнер для определений ролей и назначений ролей для Microsoft 365 для поставщиков управления доступом на основе ролей (RBAC)
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: eeb36364691fb31f30bde2313598b62ab06f950f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148536"
---
# <a name="rbacapplication-resource-type"></a>Тип ресурса rbacApplication

Пространство имен: microsoft.graph

Контейнер управления ролями для унифицированных определений ролей и назначений ролей для Microsoft 365 для поставщиков управления доступом на основе ролей (RBAC). Назначения ролей поддерживают только одну главу и одну область. В **настоящее время каталог** — единственный поддерживаемый поставщик RBAC.

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|roleAssignments|[коллекция unifiedRoleAssignment](../resources/unifiedroleassignment.md)| Ресурс для предоставления доступа пользователям или группам. |
|roleDefinitions|[коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Ресурс, представляющий роли, разрешенные поставщиками RBAC, и разрешения, присвоенные ролям. |

## <a name="json-representation"></a>Представление JSON

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
