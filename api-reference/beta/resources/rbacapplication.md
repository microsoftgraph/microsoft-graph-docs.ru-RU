---
title: Тип ресурса rbacApplication
description: Свойство навигации по управлению ролью
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9636f113222bbbe6a754c2977e08273d140a6086
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317198"
---
# <a name="rbacapplication-resource-type"></a>Тип ресурса rbacApplication

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер управления ролью для унифицированных определений ролей и назначений ролей для Microsoft 365 поставщиков RBAC. В настоящее время каталог и управление правами — это единственные поддерживаемые приложения RBAC.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Создайте новую унифицированную функциюRoleAssignment, разместив в коллекции roleAssignments. |
| [Список объектов roleAssignment](../api/rbacapplication-list-roleassignments.md) | [коллекция unifiedRoleAssignment](unifiedroleassignment.md) | Получите коллекцию объектов unifiedRoleAssignment. Только определенные экземпляры можно запрашивать, фильтруя на roleDefitionId или principalId. |
| [Создание unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Создайте новое единоеRoleDefinition, разместив в коллекции roleDefinitions. |
| [Перечисление объектов roleDefinition](../api/rbacapplication-list-roledefinitions.md) | [коллекция unifiedRoleDefinition](unifiedroledefinition.md) | Получите коллекцию объектов unifiedRoleDefinition. |

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Нет.

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


