---
title: Тип ресурса rbacApplicationMultiple
description: Свойство навигации по управлению ролью
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f25bf0db69ab9e414b99ff8f4d6f8351dc6cdfc1
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335425"
---
# <a name="rbacapplicationmultiple-resource-type"></a>Тип ресурса rbacApplicationMultiple

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер управления ролью для унифицированных определений ролей и назначений ролей для Microsoft 365 поставщиков RBAC, которые поддерживают несколько принципов и несколько областей в одном назначении ролей. Это отличается от типа [ресурса rbacApplication](rbacapplication.md) .

Облачный компьютер и Microsoft Intune являются примерами таких поставщиков RBAC. Назначение ролей в этих поставщиках может иметь массив принципов и массив групп областей.

Для определений ролей поставщик облачных ПК в настоящее время [поддерживает операцию списка](../api/rbacapplication-list-roledefinitions.md) , но не [создание](../api/rbacapplication-post-roledefinitions.md).

Наследуется [от сущности](entity.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Создайте новое единоеRoleDefinition, разместив в коллекции roleDefinitions. |
| [Перечисление объектов roleDefinition](../api/rbacapplication-list-roledefinitions.md) | [коллекция unifiedRoleDefinition](unifiedroledefinition.md) | Получите коллекцию объектов unifiedRoleDefinition. |
| [Создание unifiedRoleAssignmentMultiple](../api/rbacapplicationmultiple-post-roleassignments.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Создайте новый объединенныйRoleAssignmentMultiple, разместив в коллекции roleAssignments. |
| [Список объектов roleAssignment](../api/rbacapplicationmultiple-list-roleassignments.md) | [коллекция unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Получите коллекцию объектов unifiedRoleAssignmentMultiple. |

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|resourceNamespaces|[коллекция unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md)|Ресурс, представляючий коллекцию связанных действий.|
|roleAssignments|[коллекция unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)| Ресурс для предоставления доступа пользователям или группам. |
|roleDefinitions|[коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Ресурс, представляющий роли, разрешенные поставщиками RBAC, и разрешения, присвоенные ролям. |

## <a name="json-representation"></a>Представление JSON

Нет

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplicationMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


