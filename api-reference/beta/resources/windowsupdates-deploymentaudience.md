---
title: тип ресурса deploymentAudience
description: Набор updatableAsset ресурсов, к которым может применяться развертывание.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 98d295183f69012da6ea9fc5803bc440465854c8
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067526"
---
# <a name="deploymentaudience-resource-type"></a><span data-ttu-id="bda6b-103">тип ресурса deploymentAudience</span><span class="sxs-lookup"><span data-stu-id="bda6b-103">deploymentAudience resource type</span></span>

<span data-ttu-id="bda6b-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="bda6b-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bda6b-105">Набор [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсов, к которым [может применяться](../resources/windowsupdates-deployment.md) развертывание.</span><span class="sxs-lookup"><span data-stu-id="bda6b-105">The set of [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to which a [deployment](../resources/windowsupdates-deployment.md) can apply.</span></span>

<span data-ttu-id="bda6b-106">Если один и тот же ресурс **updatableAsset** включен в отношения исключений и участников, развертывание не будет применяться к ним.  </span><span class="sxs-lookup"><span data-stu-id="bda6b-106">If the same **updatableAsset** resource is included in the **exclusions** and **members** relationships, deployment will not apply to it.</span></span>

## <a name="methods"></a><span data-ttu-id="bda6b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bda6b-107">Methods</span></span>
|<span data-ttu-id="bda6b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bda6b-108">Method</span></span>|<span data-ttu-id="bda6b-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="bda6b-109">Return type</span></span>|<span data-ttu-id="bda6b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bda6b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bda6b-111">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="bda6b-111">List members</span></span>](../api/windowsupdates-deploymentaudience-list-members.md)|<span data-ttu-id="bda6b-112">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="bda6b-112">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="bda6b-113">Список участников [развертыванияAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="bda6b-113">List members of the [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>|
|[<span data-ttu-id="bda6b-114">Исключения списка</span><span class="sxs-lookup"><span data-stu-id="bda6b-114">List exclusions</span></span>](../api/windowsupdates-deploymentaudience-list-exclusions.md)|<span data-ttu-id="bda6b-115">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="bda6b-115">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="bda6b-116">Список исключений [развертыванияAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="bda6b-116">List exclusions of the [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>|
|[<span data-ttu-id="bda6b-117">Обновление участников и исключений</span><span class="sxs-lookup"><span data-stu-id="bda6b-117">Update members and exclusions</span></span>](../api/windowsupdates-deploymentaudience-updateaudience.md)|<span data-ttu-id="bda6b-118">Нет</span><span class="sxs-lookup"><span data-stu-id="bda6b-118">None</span></span>|<span data-ttu-id="bda6b-119">Добавление или удаление участников и исключений.</span><span class="sxs-lookup"><span data-stu-id="bda6b-119">Add or remove members and exclusions.</span></span>|
|[<span data-ttu-id="bda6b-120">Обновление участников и исключений (по ID)</span><span class="sxs-lookup"><span data-stu-id="bda6b-120">Update members and exclusions (by ID)</span></span>](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)|<span data-ttu-id="bda6b-121">Нет</span><span class="sxs-lookup"><span data-stu-id="bda6b-121">None</span></span>|<span data-ttu-id="bda6b-122">Добавление или удаление участников и исключений одного типа.</span><span class="sxs-lookup"><span data-stu-id="bda6b-122">Add or remove members and exclusions of the same type.</span></span>|

## <a name="properties"></a><span data-ttu-id="bda6b-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="bda6b-123">Properties</span></span>
|<span data-ttu-id="bda6b-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="bda6b-124">Property</span></span>|<span data-ttu-id="bda6b-125">Тип</span><span class="sxs-lookup"><span data-stu-id="bda6b-125">Type</span></span>|<span data-ttu-id="bda6b-126">Описание</span><span class="sxs-lookup"><span data-stu-id="bda6b-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bda6b-127">id</span><span class="sxs-lookup"><span data-stu-id="bda6b-127">id</span></span>|<span data-ttu-id="bda6b-128">String</span><span class="sxs-lookup"><span data-stu-id="bda6b-128">String</span></span>|<span data-ttu-id="bda6b-129">Уникальный идентификатор для аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="bda6b-129">The unique identifier for the deployment audience.</span></span> <span data-ttu-id="bda6b-130">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bda6b-130">Returned by default.</span></span> <span data-ttu-id="bda6b-131">Ключ.</span><span class="sxs-lookup"><span data-stu-id="bda6b-131">Key.</span></span> <span data-ttu-id="bda6b-132">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="bda6b-132">Not nullable.</span></span> <span data-ttu-id="bda6b-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bda6b-133">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bda6b-134">Связи</span><span class="sxs-lookup"><span data-stu-id="bda6b-134">Relationships</span></span>
|<span data-ttu-id="bda6b-135">Связь</span><span class="sxs-lookup"><span data-stu-id="bda6b-135">Relationship</span></span>|<span data-ttu-id="bda6b-136">Тип</span><span class="sxs-lookup"><span data-stu-id="bda6b-136">Type</span></span>|<span data-ttu-id="bda6b-137">Описание</span><span class="sxs-lookup"><span data-stu-id="bda6b-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bda6b-138">исключения</span><span class="sxs-lookup"><span data-stu-id="bda6b-138">exclusions</span></span>|<span data-ttu-id="bda6b-139">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="bda6b-139">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="bda6b-140">Указывает ресурсы, которые необходимо исключить из аудитории.</span><span class="sxs-lookup"><span data-stu-id="bda6b-140">Specifies the assets to exclude from the audience.</span></span>|
|<span data-ttu-id="bda6b-141">members</span><span class="sxs-lookup"><span data-stu-id="bda6b-141">members</span></span>|<span data-ttu-id="bda6b-142">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="bda6b-142">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="bda6b-143">Указывает активы, которые необходимо включить в аудиторию.</span><span class="sxs-lookup"><span data-stu-id="bda6b-143">Specifies the assets to include in the audience.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bda6b-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bda6b-144">JSON representation</span></span>
<span data-ttu-id="bda6b-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bda6b-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentAudience",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentAudience",
  "id": "String (identifier)"
}
```

