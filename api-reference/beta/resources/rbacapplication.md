---
title: Тип ресурса Рбакаппликатион
description: Свойство навигации по управлению ролями
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c1501eb32a16073990930ecf6004946b5026ea91
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462255"
---
# <a name="rbacapplication-resource-type"></a>Тип ресурса Рбакаппликатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер управления ролями для определения Объединенных ролей и назначений ролей для поставщиков Microsoft 365 RBAC. В настоящее время "каталог" является единственным поддерживаемым приложением RBAC.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание Унифиедролеассигнмент](../api/rbacapplication-post-roleassignments.md) | [унифиедролеассигнмент](unifiedroleassignment.md) | Создание нового Унифиедролеассигнмент путем отправки в коллекцию roleAssignments. |
| [Список объектов roleAssignment](../api/rbacapplication-list-roleassignments.md) | Коллекция [унифиедролеассигнмент](unifiedroleassignment.md) | Получение коллекции объектов Унифиедролеассигнмент. С помощью фильтрации на Унифиедроледефитионид или ПринЦипалид можно запрашивать только определенные экземпляры. |
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
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
