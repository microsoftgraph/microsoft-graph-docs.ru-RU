---
title: Тип ресурса rbacApplicationMultiple
description: Свойство навигации по управлению ролью
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: df5c5cd1421d4601357ef2d48c00b693e6c5e324
ms.sourcegitcommit: 30903b12daf4cf2841524c57743889e23d11f85a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2021
ms.locfileid: "53533866"
---
# <a name="rbacapplicationmultiple-resource-type"></a>Тип ресурса rbacApplicationMultiple

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер управления ролью для унифицированных определений ролей и назначений ролей для Microsoft 365 поставщиков RBAC, которые поддерживают несколько принципов и несколько областей в одном назначении ролей. 

Это отличается от типа ресурса [rbacApplication.](rbacapplication.md) 

Облачные пк и Microsoft Intune являются примерами таких поставщиков RBAC. Назначение ролей в этих поставщиках может иметь массив принципов и массив групп областей.

Для определений ролей поставщик облачных ПК в настоящее время поддерживает [операцию](../api/rbacapplication-list-roledefinitions.md) списка, но не [создание](../api/rbacapplication-post-roledefinitions.md).

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Создайте новое единоеRoleDefinition, разместив в коллекции roleDefinitions. |
| [Перечисление объектов roleDefinition](../api/rbacapplication-list-roledefinitions.md) | [коллекция unifiedRoleDefinition](unifiedroledefinition.md) | Получите коллекцию объектов unifiedRoleDefinition. |
| [Создание unifiedRoleAssignmentMultiple](../api/rbacapplicationmultiple-post-roleassignments.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Создайте новый объединенныйRoleAssignmentMultiple, разместив в коллекции roleAssignments. |
| [Список объектов roleAssignment](../api/rbacapplicationmultiple-list-roleassignments.md) | [коллекция unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Получите коллекцию объектов unifiedRoleAssignmentMultiple. |

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Отношения

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


