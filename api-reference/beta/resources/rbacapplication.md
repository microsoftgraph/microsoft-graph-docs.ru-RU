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
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="0eaeb-103">Тип ресурса Рбакаппликатион</span><span class="sxs-lookup"><span data-stu-id="0eaeb-103">rbacApplication resource type</span></span>

<span data-ttu-id="0eaeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eaeb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eaeb-105">Контейнер управления ролями для определения Объединенных ролей и назначений ролей для поставщиков Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="0eaeb-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="0eaeb-106">В настоящее время "каталог" является единственным поддерживаемым приложением RBAC.</span><span class="sxs-lookup"><span data-stu-id="0eaeb-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="methods"></a><span data-ttu-id="0eaeb-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0eaeb-107">Methods</span></span>

| <span data-ttu-id="0eaeb-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0eaeb-108">Method</span></span>       | <span data-ttu-id="0eaeb-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0eaeb-109">Return Type</span></span> | <span data-ttu-id="0eaeb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0eaeb-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0eaeb-111">Создание Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="0eaeb-111">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="0eaeb-112">унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="0eaeb-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="0eaeb-113">Создание нового Унифиедролеассигнмент путем отправки в коллекцию roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="0eaeb-113">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="0eaeb-114">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="0eaeb-114">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="0eaeb-115">Коллекция [унифиедролеассигнмент](unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0eaeb-115">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="0eaeb-116">Получение коллекции объектов Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="0eaeb-116">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="0eaeb-117">С помощью фильтрации на Унифиедроледефитионид или ПринЦипалид можно запрашивать только определенные экземпляры.</span><span class="sxs-lookup"><span data-stu-id="0eaeb-117">Only specific instances can be queried, by filtering on unifiedRoleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="0eaeb-118">Создание Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="0eaeb-118">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="0eaeb-119">унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="0eaeb-119">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="0eaeb-120">Создание нового Унифиедроледефинитион путем отправки в коллекцию перечисление roledefinition.</span><span class="sxs-lookup"><span data-stu-id="0eaeb-120">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="0eaeb-121">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="0eaeb-121">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="0eaeb-122">Коллекция [унифиедроледефинитион](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0eaeb-122">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="0eaeb-123">Получение коллекции объектов Унифиедроледефинитион.</span><span class="sxs-lookup"><span data-stu-id="0eaeb-123">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="0eaeb-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="0eaeb-124">Properties</span></span>

<span data-ttu-id="0eaeb-125">Нет</span><span class="sxs-lookup"><span data-stu-id="0eaeb-125">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0eaeb-126">Связи</span><span class="sxs-lookup"><span data-stu-id="0eaeb-126">Relationships</span></span>

<span data-ttu-id="0eaeb-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0eaeb-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0eaeb-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0eaeb-128">JSON representation</span></span>

<span data-ttu-id="0eaeb-129">Нет</span><span class="sxs-lookup"><span data-stu-id="0eaeb-129">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
