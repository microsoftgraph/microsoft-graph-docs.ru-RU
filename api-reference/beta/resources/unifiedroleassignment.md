---
title: Тип ресурса Унифиедролеассигнмент
description: Назначение роли — это связь между определением роли и участником в определенной области для предоставления доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c51c3cd7c706cf154db8c1de21c04aaa098c3efb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519619"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="155af-103">Тип ресурса Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="155af-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="155af-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="155af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="155af-105">Унифиедролеассигнмент используется для предоставления доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="155af-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="155af-106">Он представляет определение роли, назначенное участнику (обычно пользователю) в определенной области.</span><span class="sxs-lookup"><span data-stu-id="155af-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

## <a name="methods"></a><span data-ttu-id="155af-107">Методы</span><span class="sxs-lookup"><span data-stu-id="155af-107">Methods</span></span>

| <span data-ttu-id="155af-108">Метод</span><span class="sxs-lookup"><span data-stu-id="155af-108">Method</span></span>       | <span data-ttu-id="155af-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="155af-109">Return Type</span></span> | <span data-ttu-id="155af-110">Описание</span><span class="sxs-lookup"><span data-stu-id="155af-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="155af-111">Получение Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="155af-111">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="155af-112">унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="155af-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="155af-113">Чтение свойств и связей объекта Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="155af-113">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="155af-114">Создание Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="155af-114">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="155af-115">унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="155af-115">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="155af-116">Создание нового Унифиедролеассигнмент путем отправки в коллекцию roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="155af-116">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| <span data-ttu-id="155af-117">[удаление](../api/unifiedroleassignment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="155af-117">[Delete](../api/unifiedroleassignment-delete.md)</span></span> | <span data-ttu-id="155af-118">Нет</span><span class="sxs-lookup"><span data-stu-id="155af-118">None</span></span> | <span data-ttu-id="155af-119">Удаление объекта Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="155af-119">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="155af-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="155af-120">Properties</span></span>

| <span data-ttu-id="155af-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="155af-121">Property</span></span>     | <span data-ttu-id="155af-122">Тип</span><span class="sxs-lookup"><span data-stu-id="155af-122">Type</span></span>        | <span data-ttu-id="155af-123">Описание</span><span class="sxs-lookup"><span data-stu-id="155af-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="155af-124">id</span><span class="sxs-lookup"><span data-stu-id="155af-124">id</span></span>|<span data-ttu-id="155af-125">String</span><span class="sxs-lookup"><span data-stu-id="155af-125">String</span></span>| <span data-ttu-id="155af-126">Уникальный идентификатор для Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="155af-126">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="155af-127">Key, не допускающая значение null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="155af-127">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="155af-128">principalId</span><span class="sxs-lookup"><span data-stu-id="155af-128">principalId</span></span>|<span data-ttu-id="155af-129">String</span><span class="sxs-lookup"><span data-stu-id="155af-129">String</span></span>| <span data-ttu-id="155af-130">ObjectID субъекта, которому предоставляется назначение.</span><span class="sxs-lookup"><span data-stu-id="155af-130">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="155af-131">ресаурцескопе</span><span class="sxs-lookup"><span data-stu-id="155af-131">resourceScope</span></span>|<span data-ttu-id="155af-132">String</span><span class="sxs-lookup"><span data-stu-id="155af-132">String</span></span>| <span data-ttu-id="155af-133">Область, в которой применяется Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="155af-133">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="155af-134">Это "/" для всей службы.</span><span class="sxs-lookup"><span data-stu-id="155af-134">This is "/" for service-wide.</span></span> |
|<span data-ttu-id="155af-135">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="155af-135">roleDefinitionId</span></span>|<span data-ttu-id="155af-136">String</span><span class="sxs-lookup"><span data-stu-id="155af-136">String</span></span>| <span data-ttu-id="155af-137">Унифиедроледефинитион, для которого предназначено назначение.</span><span class="sxs-lookup"><span data-stu-id="155af-137">The unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="155af-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="155af-138">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="155af-139">Связи</span><span class="sxs-lookup"><span data-stu-id="155af-139">Relationships</span></span>

<span data-ttu-id="155af-140">Нет</span><span class="sxs-lookup"><span data-stu-id="155af-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="155af-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="155af-141">JSON representation</span></span>

<span data-ttu-id="155af-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="155af-142">The following is a JSON representation of the resource.</span></span>

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
