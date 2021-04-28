---
title: тип ресурсов updatableAssetGroup
description: Группа ресурсов azureADDevice, которые могут получать обновления.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a3aca42b69a906f167393cfd284d6756b3c4bb52
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067495"
---
# <a name="updatableassetgroup-resource-type"></a><span data-ttu-id="d0946-103">тип ресурсов updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="d0946-103">updatableAssetGroup resource type</span></span>

<span data-ttu-id="d0946-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="d0946-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0946-105">Группа ресурсов [azureADDevice,](../resources/windowsupdates-azureaddevice.md) которые могут получать обновления.</span><span class="sxs-lookup"><span data-stu-id="d0946-105">A group of [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources that can receive updates.</span></span>

<span data-ttu-id="d0946-106">Участники — это тип [ресурса azureADDevice.](../resources/windowsupdates-azureADDevice.md)</span><span class="sxs-lookup"><span data-stu-id="d0946-106">Members are of the [azureADDevice](../resources/windowsupdates-azureADDevice.md) resource type.</span></span> <span data-ttu-id="d0946-107">Ресурс **updatableAssetGroup** не может быть членом другой **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="d0946-107">An **updatableAssetGroup** resource cannot be a member of another **updatableAssetGroup**.</span></span>

<span data-ttu-id="d0946-108">Наследует [от updatableAsset](../resources/windowsupdates-updatableasset.md).</span><span class="sxs-lookup"><span data-stu-id="d0946-108">Inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d0946-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d0946-109">Methods</span></span>
|<span data-ttu-id="d0946-110">Метод</span><span class="sxs-lookup"><span data-stu-id="d0946-110">Method</span></span>|<span data-ttu-id="d0946-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="d0946-111">Return type</span></span>|<span data-ttu-id="d0946-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d0946-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d0946-113">Список ресурсов updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="d0946-113">List updatableAssetGroup resources</span></span>](../api/windowsupdates-updates-list-updatableassets-updatableassetgroup.md)|<span data-ttu-id="d0946-114">[коллекция microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="d0946-114">[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) collection</span></span>|<span data-ttu-id="d0946-115">Получите список объектов [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="d0946-115">Get a list of the [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) objects and their properties.</span></span>|
|[<span data-ttu-id="d0946-116">Создание updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="d0946-116">Create updatableAssetGroup</span></span>](../api/windowsupdates-updates-post-updatableassets-updatableassetgroup.md)|[<span data-ttu-id="d0946-117">microsoft.graph.windowsUpdates.updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="d0946-117">microsoft.graph.windowsUpdates.updatableAssetGroup</span></span>](../resources/windowsupdates-updatableassetgroup.md)|<span data-ttu-id="d0946-118">Создание нового [объекта updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="d0946-118">Create a new [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>|
|[<span data-ttu-id="d0946-119">Get updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="d0946-119">Get updatableAssetGroup</span></span>](../api/windowsupdates-updatableassetgroup-get.md)|[<span data-ttu-id="d0946-120">microsoft.graph.windowsUpdates.updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="d0946-120">microsoft.graph.windowsUpdates.updatableAssetGroup</span></span>](../resources/windowsupdates-updatableassetgroup.md)|<span data-ttu-id="d0946-121">Ознакомьтесь с свойствами и отношениями объекта [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="d0946-121">Read the properties and relationships of an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>|
|[<span data-ttu-id="d0946-122">Удаление updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="d0946-122">Delete updatableAssetGroup</span></span>](../api/windowsupdates-updatableassetgroup-delete.md)|<span data-ttu-id="d0946-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d0946-123">None</span></span>|<span data-ttu-id="d0946-124">Удаляет объект [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="d0946-124">Deletes an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>|
|[<span data-ttu-id="d0946-125">Добавление участников</span><span class="sxs-lookup"><span data-stu-id="d0946-125">Add members</span></span>](../api/windowsupdates-updatableassetgroup-addmembers.md)|<span data-ttu-id="d0946-126">Нет</span><span class="sxs-lookup"><span data-stu-id="d0946-126">None</span></span>|<span data-ttu-id="d0946-127">Добавление участников в [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="d0946-127">Add members to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="d0946-128">Добавление участников (по ID)</span><span class="sxs-lookup"><span data-stu-id="d0946-128">Add members (by ID)</span></span>](../api/windowsupdates-updatableassetgroup-addmembers.md)|<span data-ttu-id="d0946-129">Нет</span><span class="sxs-lookup"><span data-stu-id="d0946-129">None</span></span>|<span data-ttu-id="d0946-130">Добавление участников в [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="d0946-130">Add members to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="d0946-131">Удаление участников</span><span class="sxs-lookup"><span data-stu-id="d0946-131">Remove members</span></span>](../api/windowsupdates-updatableassetgroup-removemembers.md)|<span data-ttu-id="d0946-132">Нет</span><span class="sxs-lookup"><span data-stu-id="d0946-132">None</span></span>|<span data-ttu-id="d0946-133">Удаление участников [из updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="d0946-133">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="d0946-134">Удаление участников (по ID)</span><span class="sxs-lookup"><span data-stu-id="d0946-134">Remove members (by ID)</span></span>](../api/windowsupdates-updatableassetgroup-removemembers.md)|<span data-ttu-id="d0946-135">Нет</span><span class="sxs-lookup"><span data-stu-id="d0946-135">None</span></span>|<span data-ttu-id="d0946-136">Удаление участников [из updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="d0946-136">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="d0946-137">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="d0946-137">List members</span></span>](../api/windowsupdates-updatableassetgroup-list-members.md)|<span data-ttu-id="d0946-138">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="d0946-138">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="d0946-139">Получите [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсы из свойства навигации членов.</span><span class="sxs-lookup"><span data-stu-id="d0946-139">Get the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources from the members navigation property.</span></span>|

## <a name="properties"></a><span data-ttu-id="d0946-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0946-140">Properties</span></span>
|<span data-ttu-id="d0946-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0946-141">Property</span></span>|<span data-ttu-id="d0946-142">Тип</span><span class="sxs-lookup"><span data-stu-id="d0946-142">Type</span></span>|<span data-ttu-id="d0946-143">Описание</span><span class="sxs-lookup"><span data-stu-id="d0946-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0946-144">id</span><span class="sxs-lookup"><span data-stu-id="d0946-144">id</span></span>|<span data-ttu-id="d0946-145">String</span><span class="sxs-lookup"><span data-stu-id="d0946-145">String</span></span>|<span data-ttu-id="d0946-146">Идентификатор для группы.</span><span class="sxs-lookup"><span data-stu-id="d0946-146">An identifier for the group.</span></span> <span data-ttu-id="d0946-147">Ключ.</span><span class="sxs-lookup"><span data-stu-id="d0946-147">Key.</span></span> <span data-ttu-id="d0946-148">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="d0946-148">Not nullable.</span></span> <span data-ttu-id="d0946-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0946-149">Read-only.</span></span> <span data-ttu-id="d0946-150">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d0946-150">Returned by default.</span></span> <span data-ttu-id="d0946-151">Унаследовано от [updatableAsset](../resources/windowsupdates-updatableasset.md).</span><span class="sxs-lookup"><span data-stu-id="d0946-151">Inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0946-152">Связи</span><span class="sxs-lookup"><span data-stu-id="d0946-152">Relationships</span></span>
|<span data-ttu-id="d0946-153">Связь</span><span class="sxs-lookup"><span data-stu-id="d0946-153">Relationship</span></span>|<span data-ttu-id="d0946-154">Тип</span><span class="sxs-lookup"><span data-stu-id="d0946-154">Type</span></span>|<span data-ttu-id="d0946-155">Описание</span><span class="sxs-lookup"><span data-stu-id="d0946-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0946-156">members</span><span class="sxs-lookup"><span data-stu-id="d0946-156">members</span></span>|<span data-ttu-id="d0946-157">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="d0946-157">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="d0946-158">Члены группы.</span><span class="sxs-lookup"><span data-stu-id="d0946-158">Members of the group.</span></span> <span data-ttu-id="d0946-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0946-159">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0946-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0946-160">JSON representation</span></span>
<span data-ttu-id="d0946-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0946-161">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup",
  "baseType": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
  "id": "String (identifier)"
}
```

