---
title: Тип ресурса Рбакаппликатион
description: Свойство навигации по управлению ролями
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: afcef3766e4df80a3856ab59684ba826c3a78d14
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437827"
---
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="badd6-103">Тип ресурса Рбакаппликатион</span><span class="sxs-lookup"><span data-stu-id="badd6-103">rbacApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="badd6-104">Контейнер управления ролями для определения Объединенных ролей и назначений ролей для поставщиков Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="badd6-104">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="badd6-105">В настоящее время "каталог" является единственным поддерживаемым приложением RBAC.</span><span class="sxs-lookup"><span data-stu-id="badd6-105">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="methods"></a><span data-ttu-id="badd6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="badd6-106">Methods</span></span>

| <span data-ttu-id="badd6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="badd6-107">Method</span></span>       | <span data-ttu-id="badd6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="badd6-108">Return Type</span></span> | <span data-ttu-id="badd6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="badd6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="badd6-110">Создание Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="badd6-110">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="badd6-111">унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="badd6-111">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="badd6-112">Создание нового Унифиедролеассигнмент путем отправки в коллекцию roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="badd6-112">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="badd6-113">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="badd6-113">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="badd6-114">Коллекция [унифиедролеассигнмент](unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="badd6-114">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="badd6-115">Получение коллекции объектов Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="badd6-115">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="badd6-116">С помощью фильтрации на Унифиедроледефитионид или ПринЦипалид можно запрашивать только определенные экземпляры.</span><span class="sxs-lookup"><span data-stu-id="badd6-116">Only specific instances can be queried, by filtering on unifiedRoleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="badd6-117">Создание Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="badd6-117">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="badd6-118">унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="badd6-118">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="badd6-119">Создание нового Унифиедроледефинитион путем отправки в коллекцию перечисление roledefinition.</span><span class="sxs-lookup"><span data-stu-id="badd6-119">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="badd6-120">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="badd6-120">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="badd6-121">Коллекция [унифиедроледефинитион](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="badd6-121">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="badd6-122">Получение коллекции объектов Унифиедроледефинитион.</span><span class="sxs-lookup"><span data-stu-id="badd6-122">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="badd6-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="badd6-123">Properties</span></span>

<span data-ttu-id="badd6-124">Нет</span><span class="sxs-lookup"><span data-stu-id="badd6-124">None</span></span>

## <a name="relationships"></a><span data-ttu-id="badd6-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="badd6-125">Relationships</span></span>

<span data-ttu-id="badd6-126">Нет</span><span class="sxs-lookup"><span data-stu-id="badd6-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="badd6-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="badd6-127">JSON representation</span></span>

<span data-ttu-id="badd6-128">Нет</span><span class="sxs-lookup"><span data-stu-id="badd6-128">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
