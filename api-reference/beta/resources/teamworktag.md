---
title: тип ресурса teamworkTag
description: Представляет тег, связанный с командой.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: fc732ce340f8ab8a3460c16900c4aff2d381744e
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059891"
---
# <a name="teamworktag-resource-type"></a><span data-ttu-id="be5e2-103">тип ресурса teamworkTag</span><span class="sxs-lookup"><span data-stu-id="be5e2-103">teamworkTag resource type</span></span>

<span data-ttu-id="be5e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be5e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be5e2-105">Представляет тег, связанный с командой.</span><span class="sxs-lookup"><span data-stu-id="be5e2-105">Represents a tag associated with a team.</span></span> 

<span data-ttu-id="be5e2-106">Теги предоставляют пользователям гибкий способ классификации пользователей или групп на основе общего атрибута в команде.</span><span class="sxs-lookup"><span data-stu-id="be5e2-106">Tags provide a flexible way for customers to classify users or groups based on a common attribute within a team.</span></span> <span data-ttu-id="be5e2-107">Например, тег Nurse, Manager или Designer позволит пользователям достигать групп людей в Teams без необходимости ввести каждое имя.</span><span class="sxs-lookup"><span data-stu-id="be5e2-107">For example, a Nurse or Manager or Designer tag will enable users to reach groups of people in Teams without having to type every single name.</span></span>

<span data-ttu-id="be5e2-108">При добавлении тега пользователи могут @mention его в канале.</span><span class="sxs-lookup"><span data-stu-id="be5e2-108">When a tag is added, users can @mention it in a channel.</span></span> <span data-ttu-id="be5e2-109">Каждый, кому назначен этот тег, получит уведомление точно так же, как если бы он @mentioned по отдельности.</span><span class="sxs-lookup"><span data-stu-id="be5e2-109">Everyone who has been assigned that tag will receive a notification just as they would if they were @mentioned individually.</span></span> <span data-ttu-id="be5e2-110">Пользователи также могут использовать тег для запуска нового чата с участниками этого тега.</span><span class="sxs-lookup"><span data-stu-id="be5e2-110">Users can also use a tag is to start a new chat with the members of that tag.</span></span>

## <a name="methods"></a><span data-ttu-id="be5e2-111">Методы</span><span class="sxs-lookup"><span data-stu-id="be5e2-111">Methods</span></span>
|<span data-ttu-id="be5e2-112">Метод</span><span class="sxs-lookup"><span data-stu-id="be5e2-112">Method</span></span>|<span data-ttu-id="be5e2-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="be5e2-113">Return type</span></span>|<span data-ttu-id="be5e2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="be5e2-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be5e2-115">Список teamworkTags</span><span class="sxs-lookup"><span data-stu-id="be5e2-115">List teamworkTags</span></span>](../api/teamworktag-list.md)|<span data-ttu-id="be5e2-116">**коллекция teamworkTag**</span><span class="sxs-lookup"><span data-stu-id="be5e2-116">**teamworkTag** collection</span></span>|<span data-ttu-id="be5e2-117">Получите список объектов **teamworkTag** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="be5e2-117">Get a list of the **teamworkTag** objects and their properties.</span></span>|
|[<span data-ttu-id="be5e2-118">Создание командной работы</span><span class="sxs-lookup"><span data-stu-id="be5e2-118">Create teamworkTag</span></span>](../api/teamworktag-post.md)|<span data-ttu-id="be5e2-119">**teamworkTag**</span><span class="sxs-lookup"><span data-stu-id="be5e2-119">**teamworkTag**</span></span>|<span data-ttu-id="be5e2-120">Создание нового **объекта teamworkTag.**</span><span class="sxs-lookup"><span data-stu-id="be5e2-120">Create a new **teamworkTag** object.</span></span>|
|[<span data-ttu-id="be5e2-121">Командная работа</span><span class="sxs-lookup"><span data-stu-id="be5e2-121">Get teamworkTag</span></span>](../api/teamworktag-get.md)|<span data-ttu-id="be5e2-122">**teamworkTag**</span><span class="sxs-lookup"><span data-stu-id="be5e2-122">**teamworkTag**</span></span>|<span data-ttu-id="be5e2-123">Ознакомьтесь с свойствами и отношениями объекта **teamworkTag.**</span><span class="sxs-lookup"><span data-stu-id="be5e2-123">Read the properties and relationships of a **teamworkTag** object.</span></span>|
|[<span data-ttu-id="be5e2-124">Обновление командной работы</span><span class="sxs-lookup"><span data-stu-id="be5e2-124">Update teamworkTag</span></span>](../api/teamworktag-update.md)|<span data-ttu-id="be5e2-125">**teamworkTag**</span><span class="sxs-lookup"><span data-stu-id="be5e2-125">**teamworkTag**</span></span>|<span data-ttu-id="be5e2-126">Обновление свойств объекта **teamworkTag.**</span><span class="sxs-lookup"><span data-stu-id="be5e2-126">Update the properties of a **teamworkTag** object.</span></span>|
|[<span data-ttu-id="be5e2-127">Удаление командной работы</span><span class="sxs-lookup"><span data-stu-id="be5e2-127">Delete teamworkTag</span></span>](../api/teamworktag-delete.md)|<span data-ttu-id="be5e2-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="be5e2-128">None</span></span>|<span data-ttu-id="be5e2-129">Удаление **объекта teamworkTag.**</span><span class="sxs-lookup"><span data-stu-id="be5e2-129">Delete a **teamworkTag** object.</span></span>|
|[<span data-ttu-id="be5e2-130">Список командной работыTagMembers</span><span class="sxs-lookup"><span data-stu-id="be5e2-130">List teamworkTagMembers</span></span>](../api/teamworktagmember-list.md)|<span data-ttu-id="be5e2-131">**коллекция teamworkTagMember**</span><span class="sxs-lookup"><span data-stu-id="be5e2-131">**teamworkTagMember** collection</span></span>|<span data-ttu-id="be5e2-132">Получите список участников стандартного тега в команде и их свойства.</span><span class="sxs-lookup"><span data-stu-id="be5e2-132">Get a list of the members of a standard tag in a team and their properties.</span></span>|
|[<span data-ttu-id="be5e2-133">Получить командную работуTagMember</span><span class="sxs-lookup"><span data-stu-id="be5e2-133">Get teamworkTagMember</span></span>](../api/teamworktagmember-get.md)|<span data-ttu-id="be5e2-134">**teamworkTagMember**</span><span class="sxs-lookup"><span data-stu-id="be5e2-134">**teamworkTagMember**</span></span>|<span data-ttu-id="be5e2-135">Получите свойства и отношения участника стандартного тега в команде.</span><span class="sxs-lookup"><span data-stu-id="be5e2-135">Get the properties and relationships of a member of a standard tag in a team.</span></span>|
|[<span data-ttu-id="be5e2-136">Удаление командной работыTagMember</span><span class="sxs-lookup"><span data-stu-id="be5e2-136">Delete teamworkTagMember</span></span>](../api/teamworktagmember-delete.md)|<span data-ttu-id="be5e2-137">Нет.</span><span class="sxs-lookup"><span data-stu-id="be5e2-137">None</span></span>|<span data-ttu-id="be5e2-138">Удаление участника из стандартного тега в команде.</span><span class="sxs-lookup"><span data-stu-id="be5e2-138">Delete a member from a standard tag in the team.</span></span>|

## <a name="properties"></a><span data-ttu-id="be5e2-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="be5e2-139">Properties</span></span>
|<span data-ttu-id="be5e2-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="be5e2-140">Property</span></span>|<span data-ttu-id="be5e2-141">Тип</span><span class="sxs-lookup"><span data-stu-id="be5e2-141">Type</span></span>|<span data-ttu-id="be5e2-142">Описание</span><span class="sxs-lookup"><span data-stu-id="be5e2-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be5e2-143">description</span><span class="sxs-lookup"><span data-stu-id="be5e2-143">description</span></span>|<span data-ttu-id="be5e2-144">Строка</span><span class="sxs-lookup"><span data-stu-id="be5e2-144">String</span></span>|<span data-ttu-id="be5e2-145">Описание тега, как оно будет отображаться пользователю в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="be5e2-145">Tag description as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="be5e2-146">displayName</span><span class="sxs-lookup"><span data-stu-id="be5e2-146">displayName</span></span>|<span data-ttu-id="be5e2-147">Строка</span><span class="sxs-lookup"><span data-stu-id="be5e2-147">String</span></span>|<span data-ttu-id="be5e2-148">Тег имя, как это будет отображаться пользователю в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="be5e2-148">Tag name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="be5e2-149">id</span><span class="sxs-lookup"><span data-stu-id="be5e2-149">id</span></span>|<span data-ttu-id="be5e2-150">Строка</span><span class="sxs-lookup"><span data-stu-id="be5e2-150">String</span></span>|<span data-ttu-id="be5e2-151">ID тега.</span><span class="sxs-lookup"><span data-stu-id="be5e2-151">ID of the tag.</span></span>|
|<span data-ttu-id="be5e2-152">memberCount</span><span class="sxs-lookup"><span data-stu-id="be5e2-152">memberCount</span></span>|<span data-ttu-id="be5e2-153">Int32</span><span class="sxs-lookup"><span data-stu-id="be5e2-153">Int32</span></span>|<span data-ttu-id="be5e2-154">Количество пользователей, назначенных тегу.</span><span class="sxs-lookup"><span data-stu-id="be5e2-154">The number of users assigned to the tag.</span></span>|
|<span data-ttu-id="be5e2-155">tagType</span><span class="sxs-lookup"><span data-stu-id="be5e2-155">tagType</span></span>|<span data-ttu-id="be5e2-156">teamworkTagType</span><span class="sxs-lookup"><span data-stu-id="be5e2-156">teamworkTagType</span></span>|<span data-ttu-id="be5e2-157">Тип тега.</span><span class="sxs-lookup"><span data-stu-id="be5e2-157">The type of tag.</span></span> <span data-ttu-id="be5e2-158">По умолчанию это стандарт.</span><span class="sxs-lookup"><span data-stu-id="be5e2-158">Default is standard.</span></span>|
|<span data-ttu-id="be5e2-159">teamId</span><span class="sxs-lookup"><span data-stu-id="be5e2-159">teamId</span></span>|<span data-ttu-id="be5e2-160">Строка</span><span class="sxs-lookup"><span data-stu-id="be5e2-160">String</span></span>|<span data-ttu-id="be5e2-161">ID команды, в которой определен тег.</span><span class="sxs-lookup"><span data-stu-id="be5e2-161">ID of the team in which the tag is defined.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be5e2-162">Связи</span><span class="sxs-lookup"><span data-stu-id="be5e2-162">Relationships</span></span>
|<span data-ttu-id="be5e2-163">Связь</span><span class="sxs-lookup"><span data-stu-id="be5e2-163">Relationship</span></span>|<span data-ttu-id="be5e2-164">Тип</span><span class="sxs-lookup"><span data-stu-id="be5e2-164">Type</span></span>|<span data-ttu-id="be5e2-165">Описание</span><span class="sxs-lookup"><span data-stu-id="be5e2-165">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be5e2-166">members</span><span class="sxs-lookup"><span data-stu-id="be5e2-166">members</span></span>|<span data-ttu-id="be5e2-167">[коллекция teamworkTagMember](../resources/teamworktagmember.md)</span><span class="sxs-lookup"><span data-stu-id="be5e2-167">[teamworkTagMember](../resources/teamworktagmember.md) collection</span></span>|<span data-ttu-id="be5e2-168">Пользователи, назначенные тегу.</span><span class="sxs-lookup"><span data-stu-id="be5e2-168">Users assigned to the tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be5e2-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be5e2-169">JSON representation</span></span>
<span data-ttu-id="be5e2-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be5e2-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkTag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "String (identifier)",
  "teamId": "String",
  "displayName": "String",
  "memberCount": "Integer",
  "tagType": "String"
}
```

