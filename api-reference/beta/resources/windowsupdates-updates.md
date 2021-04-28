---
title: обновляет тип ресурса
description: Объект, который выступает в качестве контейнера для всех функций Windows обновления для службы развертывания бизнеса.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 0306dbadd815bdd8ff0ffde5719a950bcdff4683
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067484"
---
# <a name="updates-resource-type"></a><span data-ttu-id="b82b2-103">обновляет тип ресурса</span><span class="sxs-lookup"><span data-stu-id="b82b2-103">updates resource type</span></span>

<span data-ttu-id="b82b2-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="b82b2-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b82b2-105">Объект, который выступает в качестве контейнера для всех функций Windows обновления для службы развертывания бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b82b2-105">Entity that acts as a container for all Windows Update for Business deployment service functionality.</span></span>

## <a name="properties"></a><span data-ttu-id="b82b2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b82b2-106">Properties</span></span>
|<span data-ttu-id="b82b2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b82b2-107">Property</span></span>|<span data-ttu-id="b82b2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b82b2-108">Type</span></span>|<span data-ttu-id="b82b2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b82b2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b82b2-110">id</span><span class="sxs-lookup"><span data-stu-id="b82b2-110">id</span></span>|<span data-ttu-id="b82b2-111">String</span><span class="sxs-lookup"><span data-stu-id="b82b2-111">String</span></span>|<span data-ttu-id="b82b2-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b82b2-112">Read-only.</span></span> <span data-ttu-id="b82b2-113">Унаследованный от [сущности](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="b82b2-113">Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b82b2-114">Связи</span><span class="sxs-lookup"><span data-stu-id="b82b2-114">Relationships</span></span>
|<span data-ttu-id="b82b2-115">Связь</span><span class="sxs-lookup"><span data-stu-id="b82b2-115">Relationship</span></span>|<span data-ttu-id="b82b2-116">Тип</span><span class="sxs-lookup"><span data-stu-id="b82b2-116">Type</span></span>|<span data-ttu-id="b82b2-117">Описание</span><span class="sxs-lookup"><span data-stu-id="b82b2-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b82b2-118">каталог</span><span class="sxs-lookup"><span data-stu-id="b82b2-118">catalog</span></span>|[<span data-ttu-id="b82b2-119">microsoft.graph.windowsUpdates.catalog</span><span class="sxs-lookup"><span data-stu-id="b82b2-119">microsoft.graph.windowsUpdates.catalog</span></span>](../resources/windowsupdates-catalog.md)|<span data-ttu-id="b82b2-120">Каталог контента, который может быть утвержден для развертывания службой развертывания.</span><span class="sxs-lookup"><span data-stu-id="b82b2-120">Catalog of content that can be approved for deployment by the deployment service.</span></span> <span data-ttu-id="b82b2-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b82b2-121">Read-only.</span></span>|
|<span data-ttu-id="b82b2-122">развертывания</span><span class="sxs-lookup"><span data-stu-id="b82b2-122">deployments</span></span>|<span data-ttu-id="b82b2-123">[коллекция microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="b82b2-123">[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md) collection</span></span>|<span data-ttu-id="b82b2-124">Развертывания, созданные с помощью службы развертывания.</span><span class="sxs-lookup"><span data-stu-id="b82b2-124">Deployments created using the deployment service.</span></span> <span data-ttu-id="b82b2-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b82b2-125">Read-only.</span></span>|
|<span data-ttu-id="b82b2-126">updatableAssets</span><span class="sxs-lookup"><span data-stu-id="b82b2-126">updatableAssets</span></span>|<span data-ttu-id="b82b2-127">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="b82b2-127">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="b82b2-128">Активы, зарегистрированные в службе развертывания, которые могут получать обновления.</span><span class="sxs-lookup"><span data-stu-id="b82b2-128">Assets registered with the deployment service that can receive updates.</span></span> <span data-ttu-id="b82b2-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b82b2-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b82b2-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b82b2-130">JSON representation</span></span>
<span data-ttu-id="b82b2-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b82b2-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updates",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updates",
  "id": "String (identifier)"
}
```

