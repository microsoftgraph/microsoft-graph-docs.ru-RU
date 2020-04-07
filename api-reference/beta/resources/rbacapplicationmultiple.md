---
title: Тип ресурса Рбакаппликатионмултипле
description: Свойство навигации по управлению ролями
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c89b9e12121fc5c3183629b6349d04d5dd434cab
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160384"
---
# <a name="rbacapplicationmultiple-resource-type"></a>Тип ресурса Рбакаппликатионмултипле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер управления ролями для универсальных определений ролей и назначений ролей для поставщиков Microsoft 365 RBAC, поддерживающих несколько субъектов и несколько областей в рамках одного назначения роли. Это отличается от типа ресурса [рбакаппликатион](rbacapplication.md) . Microsoft Intune это пример такого поставщика RBAC. Назначение роли в Intune может иметь массив субъектов и массив групп областей.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание Унифиедролеассигнментмултипле](../api/unifiedroleassignmentmultiple-post.md) | [унифиедролеассигнментмултипле](unifiedroleassignmentmultiple.md) | Создание нового Унифиедролеассигнментмултипле путем отправки в коллекцию roleAssignments. |
| [Список Ролеассигнментсмултипле](../api/unifiedroleassignmentmultiple-list.md) | Коллекция [унифиедролеассигнментмултипле](unifiedroleassignmentmultiple.md) | Получение коллекции объектов Унифиедролеассигнментмултипле. С помощью фильтрации на Унифиедроледефитионид или ПринЦипалид можно запрашивать только определенные экземпляры. |
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