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
# <a name="rbacapplicationmultiple-resource-type"></a><span data-ttu-id="b608c-103">Тип ресурса Рбакаппликатионмултипле</span><span class="sxs-lookup"><span data-stu-id="b608c-103">rbacApplicationMultiple resource type</span></span>

<span data-ttu-id="b608c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b608c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b608c-105">Контейнер управления ролями для универсальных определений ролей и назначений ролей для поставщиков Microsoft 365 RBAC, поддерживающих несколько субъектов и несколько областей в рамках одного назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b608c-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="b608c-106">Это отличается от типа ресурса [рбакаппликатион](rbacapplication.md) .</span><span class="sxs-lookup"><span data-stu-id="b608c-106">This is different from [rbacApplication](rbacapplication.md) resource type.</span></span> <span data-ttu-id="b608c-107">Microsoft Intune это пример такого поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="b608c-107">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="b608c-108">Назначение роли в Intune может иметь массив субъектов и массив групп областей.</span><span class="sxs-lookup"><span data-stu-id="b608c-108">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span>

## <a name="methods"></a><span data-ttu-id="b608c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="b608c-109">Methods</span></span>

| <span data-ttu-id="b608c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="b608c-110">Method</span></span>       | <span data-ttu-id="b608c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b608c-111">Return Type</span></span> | <span data-ttu-id="b608c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b608c-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b608c-113">Создание Унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="b608c-113">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="b608c-114">унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="b608c-114">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="b608c-115">Создание нового Унифиедролеассигнментмултипле путем отправки в коллекцию roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="b608c-115">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="b608c-116">Список Ролеассигнментсмултипле</span><span class="sxs-lookup"><span data-stu-id="b608c-116">List roleAssignmentsMultiple</span></span>](../api/unifiedroleassignmentmultiple-list.md) | <span data-ttu-id="b608c-117">Коллекция [унифиедролеассигнментмултипле](unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="b608c-117">[unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) collection</span></span> | <span data-ttu-id="b608c-118">Получение коллекции объектов Унифиедролеассигнментмултипле.</span><span class="sxs-lookup"><span data-stu-id="b608c-118">Get unifiedRoleAssignmentMultiple object collection.</span></span> <span data-ttu-id="b608c-119">С помощью фильтрации на Унифиедроледефитионид или ПринЦипалид можно запрашивать только определенные экземпляры.</span><span class="sxs-lookup"><span data-stu-id="b608c-119">Only specific instances can be queried, by filtering on unifiedRoleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="b608c-120">Создание Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="b608c-120">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="b608c-121">унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="b608c-121">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="b608c-122">Создание нового Унифиедроледефинитион путем отправки в коллекцию перечисление roledefinition.</span><span class="sxs-lookup"><span data-stu-id="b608c-122">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="b608c-123">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b608c-123">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="b608c-124">Коллекция [унифиедроледефинитион](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b608c-124">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="b608c-125">Получение коллекции объектов Унифиедроледефинитион.</span><span class="sxs-lookup"><span data-stu-id="b608c-125">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="b608c-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="b608c-126">Properties</span></span>

<span data-ttu-id="b608c-127">Нет</span><span class="sxs-lookup"><span data-stu-id="b608c-127">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b608c-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="b608c-128">Relationships</span></span>

<span data-ttu-id="b608c-129">Нет</span><span class="sxs-lookup"><span data-stu-id="b608c-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b608c-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b608c-130">JSON representation</span></span>

<span data-ttu-id="b608c-131">Нет</span><span class="sxs-lookup"><span data-stu-id="b608c-131">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplicationMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->