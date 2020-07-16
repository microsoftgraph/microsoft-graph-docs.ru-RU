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
# <a name="rbacapplicationmultiple-resource-type"></a><span data-ttu-id="3e9d7-103">Тип ресурса Рбакаппликатионмултипле</span><span class="sxs-lookup"><span data-stu-id="3e9d7-103">rbacApplicationMultiple resource type</span></span>

<span data-ttu-id="3e9d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e9d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e9d7-105">Контейнер управления ролями для универсальных определений ролей и назначений ролей для поставщиков Microsoft 365 RBAC, поддерживающих несколько субъектов и несколько областей в рамках одного назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3e9d7-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="3e9d7-106">Это отличается от типа ресурса [рбакаппликатион](rbacapplication.md) .</span><span class="sxs-lookup"><span data-stu-id="3e9d7-106">This is different from [rbacApplication](rbacapplication.md) resource type.</span></span> <span data-ttu-id="3e9d7-107">Microsoft Intune это пример такого поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="3e9d7-107">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="3e9d7-108">Назначение роли в Intune может иметь массив субъектов и массив групп областей.</span><span class="sxs-lookup"><span data-stu-id="3e9d7-108">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span>

## <a name="methods"></a><span data-ttu-id="3e9d7-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3e9d7-109">Methods</span></span>

| <span data-ttu-id="3e9d7-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3e9d7-110">Method</span></span>       | <span data-ttu-id="3e9d7-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3e9d7-111">Return Type</span></span> | <span data-ttu-id="3e9d7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3e9d7-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3e9d7-113">Создание unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3e9d7-113">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="3e9d7-114">унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="3e9d7-114">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="3e9d7-115">Создание нового Унифиедролеассигнментмултипле путем отправки в коллекцию roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="3e9d7-115">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="3e9d7-116">Список Ролеассигнментсмултипле</span><span class="sxs-lookup"><span data-stu-id="3e9d7-116">List roleAssignmentsMultiple</span></span>](../api/unifiedroleassignmentmultiple-list.md) | <span data-ttu-id="3e9d7-117">Коллекция [унифиедролеассигнментмултипле](unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="3e9d7-117">[unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) collection</span></span> | <span data-ttu-id="3e9d7-118">Получение коллекции объектов Унифиедролеассигнментмултипле.</span><span class="sxs-lookup"><span data-stu-id="3e9d7-118">Get unifiedRoleAssignmentMultiple object collection.</span></span> |
| [<span data-ttu-id="3e9d7-119">Создание Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="3e9d7-119">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="3e9d7-120">унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="3e9d7-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="3e9d7-121">Создание нового Унифиедроледефинитион путем отправки в коллекцию перечисление roledefinition.</span><span class="sxs-lookup"><span data-stu-id="3e9d7-121">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="3e9d7-122">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3e9d7-122">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="3e9d7-123">Коллекция [унифиедроледефинитион](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3e9d7-123">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="3e9d7-124">Получение коллекции объектов Унифиедроледефинитион.</span><span class="sxs-lookup"><span data-stu-id="3e9d7-124">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="3e9d7-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e9d7-125">Properties</span></span>

<span data-ttu-id="3e9d7-126">Нет</span><span class="sxs-lookup"><span data-stu-id="3e9d7-126">None</span></span>

## <a name="relationships"></a><span data-ttu-id="3e9d7-127">Связи</span><span class="sxs-lookup"><span data-stu-id="3e9d7-127">Relationships</span></span>

<span data-ttu-id="3e9d7-128">Нет</span><span class="sxs-lookup"><span data-stu-id="3e9d7-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e9d7-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e9d7-129">JSON representation</span></span>

<span data-ttu-id="3e9d7-130">Нет</span><span class="sxs-lookup"><span data-stu-id="3e9d7-130">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplicationMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
