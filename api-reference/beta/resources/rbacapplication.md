---
title: Тип ресурса Рбакаппликатион
description: Свойство навигации по управлению ролями
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5a5860cce6625257dfdecf145786a2e9bd2f2465
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "44989795"
---
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="2f26d-103">Тип ресурса Рбакаппликатион</span><span class="sxs-lookup"><span data-stu-id="2f26d-103">rbacApplication resource type</span></span>

<span data-ttu-id="2f26d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f26d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f26d-105">Контейнер управления ролями для определения Объединенных ролей и назначений ролей для поставщиков Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="2f26d-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="2f26d-106">В настоящее время "каталог" является единственным поддерживаемым приложением RBAC.</span><span class="sxs-lookup"><span data-stu-id="2f26d-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="methods"></a><span data-ttu-id="2f26d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2f26d-107">Methods</span></span>

| <span data-ttu-id="2f26d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2f26d-108">Method</span></span>       | <span data-ttu-id="2f26d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2f26d-109">Return Type</span></span> | <span data-ttu-id="2f26d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2f26d-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2f26d-111">Создание Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="2f26d-111">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="2f26d-112">унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="2f26d-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="2f26d-113">Создание нового Унифиедролеассигнмент путем отправки в коллекцию roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="2f26d-113">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="2f26d-114">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2f26d-114">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="2f26d-115">Коллекция [унифиедролеассигнмент](unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2f26d-115">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="2f26d-116">Получение коллекции объектов Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="2f26d-116">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="2f26d-117">С помощью фильтрации на Роледефитионид или ПринЦипалид можно запрашивать только определенные экземпляры.</span><span class="sxs-lookup"><span data-stu-id="2f26d-117">Only specific instances can be queried, by filtering on roleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="2f26d-118">Создание Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="2f26d-118">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="2f26d-119">унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="2f26d-119">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="2f26d-120">Создание нового Унифиедроледефинитион путем отправки в коллекцию перечисление roledefinition.</span><span class="sxs-lookup"><span data-stu-id="2f26d-120">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="2f26d-121">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2f26d-121">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="2f26d-122">Коллекция [унифиедроледефинитион](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2f26d-122">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="2f26d-123">Получение коллекции объектов Унифиедроледефинитион.</span><span class="sxs-lookup"><span data-stu-id="2f26d-123">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="2f26d-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f26d-124">Properties</span></span>

<span data-ttu-id="2f26d-125">Нет</span><span class="sxs-lookup"><span data-stu-id="2f26d-125">None</span></span>

## <a name="relationships"></a><span data-ttu-id="2f26d-126">Связи</span><span class="sxs-lookup"><span data-stu-id="2f26d-126">Relationships</span></span>

<span data-ttu-id="2f26d-127">Нет</span><span class="sxs-lookup"><span data-stu-id="2f26d-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f26d-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f26d-128">JSON representation</span></span>

<span data-ttu-id="2f26d-129">Нет</span><span class="sxs-lookup"><span data-stu-id="2f26d-129">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
