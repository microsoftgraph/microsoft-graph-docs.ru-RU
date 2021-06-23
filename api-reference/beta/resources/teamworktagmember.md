---
title: тип ресурса teamworkTagMember
description: Представляет пользователя в команде с тегом, примененным к ним.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 73666dd19720e6d8882bb16fd90c612097e41d10
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059885"
---
# <a name="teamworktagmember-resource-type"></a><span data-ttu-id="6da31-103">тип ресурса teamworkTagMember</span><span class="sxs-lookup"><span data-stu-id="6da31-103">teamworkTagMember resource type</span></span>

<span data-ttu-id="6da31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6da31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6da31-105">Представляет пользователя в команде, к которой применяется тег.</span><span class="sxs-lookup"><span data-stu-id="6da31-105">Represents a user in a team to whom a tag is applied.</span></span>

## <a name="methods"></a><span data-ttu-id="6da31-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6da31-106">Methods</span></span>
|<span data-ttu-id="6da31-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6da31-107">Method</span></span>|<span data-ttu-id="6da31-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="6da31-108">Return type</span></span>|<span data-ttu-id="6da31-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6da31-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6da31-110">Список командной работыTagMembers</span><span class="sxs-lookup"><span data-stu-id="6da31-110">List teamworkTagMembers</span></span>](../api/teamworktagmember-list.md)|<span data-ttu-id="6da31-111">**коллекция teamworkTagMember**</span><span class="sxs-lookup"><span data-stu-id="6da31-111">**teamworkTagMember** collection</span></span>|<span data-ttu-id="6da31-112">Получите список участников стандартного тега в команде и их свойства.</span><span class="sxs-lookup"><span data-stu-id="6da31-112">Get a list of the members of a standard tag in a team and their properties.</span></span>|
|[<span data-ttu-id="6da31-113">Получить командную работуTagMember</span><span class="sxs-lookup"><span data-stu-id="6da31-113">Get teamworkTagMember</span></span>](../api/teamworktagmember-get.md)|<span data-ttu-id="6da31-114">**teamworkTagMember**</span><span class="sxs-lookup"><span data-stu-id="6da31-114">**teamworkTagMember**</span></span>|<span data-ttu-id="6da31-115">Получите свойства и отношения участника стандартного тега в команде.</span><span class="sxs-lookup"><span data-stu-id="6da31-115">Get the properties and relationships of a member of a standard tag in a team.</span></span>|
|[<span data-ttu-id="6da31-116">Удаление командной работыTagMember</span><span class="sxs-lookup"><span data-stu-id="6da31-116">Delete teamworkTagMember</span></span>](../api/teamworktagmember-delete.md)|<span data-ttu-id="6da31-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="6da31-117">None</span></span>|<span data-ttu-id="6da31-118">Удаление участника из стандартного тега в команде.</span><span class="sxs-lookup"><span data-stu-id="6da31-118">Delete a member from a standard tag in the team.</span></span>|

## <a name="properties"></a><span data-ttu-id="6da31-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="6da31-119">Properties</span></span>
|<span data-ttu-id="6da31-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="6da31-120">Property</span></span>|<span data-ttu-id="6da31-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6da31-121">Type</span></span>|<span data-ttu-id="6da31-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6da31-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6da31-123">displayName</span><span class="sxs-lookup"><span data-stu-id="6da31-123">displayName</span></span>|<span data-ttu-id="6da31-124">Строка</span><span class="sxs-lookup"><span data-stu-id="6da31-124">String</span></span>|<span data-ttu-id="6da31-125">Имя отображения участника.</span><span class="sxs-lookup"><span data-stu-id="6da31-125">The member's display name.</span></span>|
|<span data-ttu-id="6da31-126">ID</span><span class="sxs-lookup"><span data-stu-id="6da31-126">ID</span></span>|<span data-ttu-id="6da31-127">Строка</span><span class="sxs-lookup"><span data-stu-id="6da31-127">String</span></span>|<span data-ttu-id="6da31-128">ID участника.</span><span class="sxs-lookup"><span data-stu-id="6da31-128">ID of the member.</span></span>|
|<span data-ttu-id="6da31-129">tenantID</span><span class="sxs-lookup"><span data-stu-id="6da31-129">tenantID</span></span>|<span data-ttu-id="6da31-130">Строка</span><span class="sxs-lookup"><span data-stu-id="6da31-130">String</span></span>|<span data-ttu-id="6da31-131">ID клиента, в который входит член тега.</span><span class="sxs-lookup"><span data-stu-id="6da31-131">The ID of the tenant that the tag member is a part of.</span></span>|
|<span data-ttu-id="6da31-132">userID</span><span class="sxs-lookup"><span data-stu-id="6da31-132">userID</span></span>|<span data-ttu-id="6da31-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6da31-133">String</span></span>|<span data-ttu-id="6da31-134">Пользовательский ID участника.</span><span class="sxs-lookup"><span data-stu-id="6da31-134">The user ID of the member.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6da31-135">Связи</span><span class="sxs-lookup"><span data-stu-id="6da31-135">Relationships</span></span>
<span data-ttu-id="6da31-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6da31-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6da31-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6da31-137">JSON representation</span></span>
<span data-ttu-id="6da31-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6da31-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "ID",
  "@odata.type": "microsoft.graph.teamworkTagMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagMember",
  "ID": "String (Identifier)",
  "displayName": "String",
  "tenantID": "String",
  "userID": "String"
}
```

