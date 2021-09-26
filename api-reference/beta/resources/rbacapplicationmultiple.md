---
title: Тип ресурса rbacApplicationMultiple
description: Свойство навигации по управлению ролью
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a989896dbf3ae71daade9e4feee07f3ea2bcd94b
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766350"
---
# <a name="rbacapplicationmultiple-resource-type"></a>Тип ресурса rbacApplicationMultiple

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер управления ролью для унифицированных определений ролей и назначений ролей для Microsoft 365 поставщиков RBAC, которые поддерживают несколько принципов и несколько областей в одном назначении ролей. 

Это отличается от типа ресурса [rbacApplication.](rbacapplication.md) 

Облачные пк и Microsoft Intune являются примерами таких поставщиков RBAC. Назначение ролей в этих поставщиках может иметь массив принципов и массив групп областей.

Для определений ролей поставщик облачных ПК в настоящее время поддерживает [операцию](../api/rbacapplication-list-roledefinitions.md) списка, но не [создание](../api/rbacapplication-post-roledefinitions.md).


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

Нет

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


