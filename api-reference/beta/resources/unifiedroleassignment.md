---
title: Тип ресурса Унифиедролеассигнмент
description: Назначение роли — это связь между определением роли и участником в определенной области для предоставления доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cfc0c00add243b98c852a00f0a4ab990c3ca5173
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437792"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="a4d0f-103">Тип ресурса Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="a4d0f-103">unifiedRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4d0f-104">Унифиедролеассигнмент используется для предоставления доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-104">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="a4d0f-105">Он представляет определение роли, назначенное участнику (обычно пользователю) в определенной области.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-105">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

## <a name="methods"></a><span data-ttu-id="a4d0f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a4d0f-106">Methods</span></span>

| <span data-ttu-id="a4d0f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a4d0f-107">Method</span></span>       | <span data-ttu-id="a4d0f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a4d0f-108">Return Type</span></span> | <span data-ttu-id="a4d0f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a4d0f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a4d0f-110">Получение Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="a4d0f-110">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="a4d0f-111">унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="a4d0f-111">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="a4d0f-112">Чтение свойств и связей объекта Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-112">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="a4d0f-113">Создание Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="a4d0f-113">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="a4d0f-114">унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="a4d0f-114">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="a4d0f-115">Создание нового Унифиедролеассигнмент путем отправки в коллекцию roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-115">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="a4d0f-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="a4d0f-116">Delete</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="a4d0f-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a4d0f-117">None</span></span> | <span data-ttu-id="a4d0f-118">Удаление объекта Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-118">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a4d0f-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4d0f-119">Properties</span></span>

| <span data-ttu-id="a4d0f-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4d0f-120">Property</span></span>     | <span data-ttu-id="a4d0f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a4d0f-121">Type</span></span>        | <span data-ttu-id="a4d0f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a4d0f-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4d0f-123">id</span><span class="sxs-lookup"><span data-stu-id="a4d0f-123">id</span></span>|<span data-ttu-id="a4d0f-124">String</span><span class="sxs-lookup"><span data-stu-id="a4d0f-124">String</span></span>| <span data-ttu-id="a4d0f-125">Уникальный идентификатор для Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-125">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="a4d0f-126">Key, не допускающая значение null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-126">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="a4d0f-127">principalId</span><span class="sxs-lookup"><span data-stu-id="a4d0f-127">principalId</span></span>|<span data-ttu-id="a4d0f-128">String</span><span class="sxs-lookup"><span data-stu-id="a4d0f-128">String</span></span>| <span data-ttu-id="a4d0f-129">ObjectID субъекта, которому предоставляется назначение.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-129">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="a4d0f-130">ресаурцескопе</span><span class="sxs-lookup"><span data-stu-id="a4d0f-130">resourceScope</span></span>|<span data-ttu-id="a4d0f-131">String</span><span class="sxs-lookup"><span data-stu-id="a4d0f-131">String</span></span>| <span data-ttu-id="a4d0f-132">Область, в которой применяется Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-132">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="a4d0f-133">Это "/" для всей службы.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-133">This is "/" for service-wide.</span></span> |
|<span data-ttu-id="a4d0f-134">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="a4d0f-134">roleDefinitionId</span></span>|<span data-ttu-id="a4d0f-135">String</span><span class="sxs-lookup"><span data-stu-id="a4d0f-135">String</span></span>| <span data-ttu-id="a4d0f-136">Унифиедроледефинитион, для которого предназначено назначение.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-136">The unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="a4d0f-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-137">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a4d0f-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="a4d0f-138">Relationships</span></span>

<span data-ttu-id="a4d0f-139">Нет</span><span class="sxs-lookup"><span data-stu-id="a4d0f-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4d0f-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4d0f-140">JSON representation</span></span>

<span data-ttu-id="a4d0f-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4d0f-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "principalId": "String",
  "resourceScope": "String",
  "roleDefinitionId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
