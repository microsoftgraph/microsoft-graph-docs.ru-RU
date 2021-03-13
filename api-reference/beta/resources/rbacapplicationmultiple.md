---
title: Тип ресурса rbacApplicationMultiple
description: Свойство навигации по управлению ролью
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ba6c4973dd79f328c1d04ea26803a6b2aec39c7f
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760920"
---
# <a name="rbacapplicationmultiple-resource-type"></a><span data-ttu-id="bac0d-103">Тип ресурса rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="bac0d-103">rbacApplicationMultiple resource type</span></span>

<span data-ttu-id="bac0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bac0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bac0d-105">Контейнер управления ролью для унифицированных определений ролей и назначений ролей для поставщиков Microsoft 365 RBAC, которые поддерживают несколько принципов и несколько областей в одном назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="bac0d-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="bac0d-106">Это отличается от типа ресурса [rbacApplication.](rbacapplication.md)</span><span class="sxs-lookup"><span data-stu-id="bac0d-106">This is different from [rbacApplication](rbacapplication.md) resource type.</span></span> <span data-ttu-id="bac0d-107">Microsoft Intune является примером такого поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="bac0d-107">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="bac0d-108">Назначение ролей в Intune может иметь массив принципалов и массив групп областей.</span><span class="sxs-lookup"><span data-stu-id="bac0d-108">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span>

## <a name="methods"></a><span data-ttu-id="bac0d-109">Методы</span><span class="sxs-lookup"><span data-stu-id="bac0d-109">Methods</span></span>

| <span data-ttu-id="bac0d-110">Метод</span><span class="sxs-lookup"><span data-stu-id="bac0d-110">Method</span></span>       | <span data-ttu-id="bac0d-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bac0d-111">Return Type</span></span> | <span data-ttu-id="bac0d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bac0d-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bac0d-113">Создание unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="bac0d-113">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="bac0d-114">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="bac0d-114">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="bac0d-115">Создайте новый объединенныйRoleAssignmentMultiple, разместив в коллекции roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="bac0d-115">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="bac0d-116">List roleAssignmentsMultiple</span><span class="sxs-lookup"><span data-stu-id="bac0d-116">List roleAssignmentsMultiple</span></span>](../api/unifiedroleassignmentmultiple-list.md) | <span data-ttu-id="bac0d-117">[коллекция unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="bac0d-117">[unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) collection</span></span> | <span data-ttu-id="bac0d-118">Получите коллекцию объектов unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="bac0d-118">Get unifiedRoleAssignmentMultiple object collection.</span></span> |
| [<span data-ttu-id="bac0d-119">Создание unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bac0d-119">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="bac0d-120">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bac0d-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="bac0d-121">Создайте новое единоеRoleDefinition, разместив в коллекции roleDefinitions.</span><span class="sxs-lookup"><span data-stu-id="bac0d-121">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="bac0d-122">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="bac0d-122">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="bac0d-123">[коллекция unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bac0d-123">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="bac0d-124">Получите коллекцию объектов unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="bac0d-124">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="bac0d-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="bac0d-125">Properties</span></span>

<span data-ttu-id="bac0d-126">Нет</span><span class="sxs-lookup"><span data-stu-id="bac0d-126">None</span></span>

## <a name="relationships"></a><span data-ttu-id="bac0d-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="bac0d-127">Relationships</span></span>

<span data-ttu-id="bac0d-128">Нет</span><span class="sxs-lookup"><span data-stu-id="bac0d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bac0d-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bac0d-129">JSON representation</span></span>

<span data-ttu-id="bac0d-130">Нет</span><span class="sxs-lookup"><span data-stu-id="bac0d-130">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplicationMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


