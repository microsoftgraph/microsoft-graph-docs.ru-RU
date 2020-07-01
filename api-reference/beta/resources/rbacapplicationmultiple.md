---
title: Тип ресурса Рбакаппликатионмултипле
description: Свойство навигации по управлению ролями
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e7f44133050a616cac190aee5c7eeac9904f8715
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990278"
---
# <a name="rbacapplicationmultiple-resource-type"></a>Тип ресурса Рбакаппликатионмултипле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер управления ролями для универсальных определений ролей и назначений ролей для поставщиков Microsoft 365 RBAC, поддерживающих несколько субъектов и несколько областей в рамках одного назначения роли. Это отличается от типа ресурса [рбакаппликатион](rbacapplication.md) . Microsoft Intune это пример такого поставщика RBAC. Назначение роли в Intune может иметь массив субъектов и массив групп областей.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [унифиедролеассигнментмултипле](unifiedroleassignmentmultiple.md) | Создание нового Унифиедролеассигнментмултипле путем отправки в коллекцию roleAssignments. |
| [Список Ролеассигнментсмултипле](../api/unifiedroleassignmentmultiple-list.md) | Коллекция [унифиедролеассигнментмултипле](unifiedroleassignmentmultiple.md) | Получение коллекции объектов Унифиедролеассигнментмултипле. |
| [Создание Унифиедроледефинитион](../api/rbacapplication-post-roledefinitions.md) | [унифиедроледефинитион](unifiedroledefinition.md) | Создание нового Унифиедроледефинитион путем отправки в коллекцию перечисление roledefinition. |
| [Перечисление объектов roleDefinition](../api/rbacapplication-list-roledefinitions.md) | Коллекция [унифиедроледефинитион](unifiedroledefinition.md) | Получение коллекции объектов Унифиедроледефинитион. |

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
