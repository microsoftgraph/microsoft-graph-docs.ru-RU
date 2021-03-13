---
title: Тип ресурса rbacApplication
description: Свойство навигации по управлению ролью
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: c3833d07e0fb9758cc8f4f5418f725889fd784dc
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760927"
---
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="706c1-103">Тип ресурса rbacApplication</span><span class="sxs-lookup"><span data-stu-id="706c1-103">rbacApplication resource type</span></span>

<span data-ttu-id="706c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="706c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="706c1-105">Контейнер управления ролью для унифицированных определений ролей и назначений ролей для поставщиков Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="706c1-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="706c1-106">В настоящее время "каталог" является единственным поддерживаемой приложением RBAC.</span><span class="sxs-lookup"><span data-stu-id="706c1-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="methods"></a><span data-ttu-id="706c1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="706c1-107">Methods</span></span>

| <span data-ttu-id="706c1-108">Метод</span><span class="sxs-lookup"><span data-stu-id="706c1-108">Method</span></span>       | <span data-ttu-id="706c1-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="706c1-109">Return Type</span></span> | <span data-ttu-id="706c1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="706c1-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="706c1-111">Создание unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="706c1-111">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="706c1-112">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="706c1-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="706c1-113">Создайте новую унифицированную функциюRoleAssignment, разместив в коллекции roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="706c1-113">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="706c1-114">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="706c1-114">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="706c1-115">[коллекция unifiedRoleAssignment](unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="706c1-115">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="706c1-116">Получите коллекцию объектов unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="706c1-116">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="706c1-117">Только определенные экземпляры можно запрашивать, фильтруя на roleDefitionId или principalId.</span><span class="sxs-lookup"><span data-stu-id="706c1-117">Only specific instances can be queried, by filtering on roleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="706c1-118">Создание unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="706c1-118">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="706c1-119">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="706c1-119">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="706c1-120">Создайте новое единоеRoleDefinition, разместив в коллекции roleDefinitions.</span><span class="sxs-lookup"><span data-stu-id="706c1-120">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="706c1-121">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="706c1-121">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="706c1-122">[коллекция unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="706c1-122">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="706c1-123">Получите коллекцию объектов unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="706c1-123">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="706c1-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="706c1-124">Properties</span></span>

<span data-ttu-id="706c1-125">Нет</span><span class="sxs-lookup"><span data-stu-id="706c1-125">None</span></span>

## <a name="relationships"></a><span data-ttu-id="706c1-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="706c1-126">Relationships</span></span>

<span data-ttu-id="706c1-127">Нет</span><span class="sxs-lookup"><span data-stu-id="706c1-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="706c1-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="706c1-128">JSON representation</span></span>

<span data-ttu-id="706c1-129">Нет</span><span class="sxs-lookup"><span data-stu-id="706c1-129">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


