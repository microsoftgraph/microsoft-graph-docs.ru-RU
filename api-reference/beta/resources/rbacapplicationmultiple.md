---
title: Тип ресурса Рбакаппликатионмултипле
description: Свойство навигации по управлению ролями
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5caf422293a0e06fa9ba524af2a4809b49709140
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026392"
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


