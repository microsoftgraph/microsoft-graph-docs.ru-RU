---
title: Тип ресурса dataSourceContainer
description: Базовый класс для хранителей и источников данных без хранения.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e2d7d88a3d747817858853ebc6f2909b2edde65b
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080902"
---
# <a name="datasourcecontainer-resource-type"></a><span data-ttu-id="f2de9-103">Тип ресурса dataSourceContainer</span><span class="sxs-lookup"><span data-stu-id="f2de9-103">dataSourceContainer resource type</span></span>

<span data-ttu-id="f2de9-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f2de9-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2de9-105">Базовый класс [для хранителя](../resources/ediscovery-custodian.md) [и noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span><span class="sxs-lookup"><span data-stu-id="f2de9-105">Base class for [custodian](../resources/ediscovery-custodian.md) and [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>

<span data-ttu-id="f2de9-106">Наследует от [объекта](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="f2de9-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f2de9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f2de9-107">Methods</span></span>

<span data-ttu-id="f2de9-108">Нет</span><span class="sxs-lookup"><span data-stu-id="f2de9-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="f2de9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2de9-109">Properties</span></span>

|<span data-ttu-id="f2de9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2de9-110">Property</span></span>|<span data-ttu-id="f2de9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f2de9-111">Type</span></span>|<span data-ttu-id="f2de9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f2de9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2de9-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2de9-113">createdDateTime</span></span>|<span data-ttu-id="f2de9-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2de9-114">DateTimeOffset</span></span>|<span data-ttu-id="f2de9-115">Создана дата и время создания объекта dataSourceContainer.</span><span class="sxs-lookup"><span data-stu-id="f2de9-115">Created date and time of the dataSourceContainer entity.</span></span>|
|<span data-ttu-id="f2de9-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f2de9-116">displayName</span></span>|<span data-ttu-id="f2de9-117">String</span><span class="sxs-lookup"><span data-stu-id="f2de9-117">String</span></span>|<span data-ttu-id="f2de9-118">Отображение имени объекта dataSourceContainer.</span><span class="sxs-lookup"><span data-stu-id="f2de9-118">Display name of the dataSourceContainer entity.</span></span>|
|<span data-ttu-id="f2de9-119">id</span><span class="sxs-lookup"><span data-stu-id="f2de9-119">id</span></span>|<span data-ttu-id="f2de9-120">String</span><span class="sxs-lookup"><span data-stu-id="f2de9-120">String</span></span>|<span data-ttu-id="f2de9-121">Уникальный идентификатор dataSourceContainer.</span><span class="sxs-lookup"><span data-stu-id="f2de9-121">Unique identifier of the dataSourceContainer.</span></span> <span data-ttu-id="f2de9-122">Унаследованный от [сущности](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="f2de9-122">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="f2de9-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2de9-123">lastModifiedDateTime</span></span>|<span data-ttu-id="f2de9-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2de9-124">DateTimeOffset</span></span>|<span data-ttu-id="f2de9-125">Последняя измененная дата и время dataSourceContainer.</span><span class="sxs-lookup"><span data-stu-id="f2de9-125">Last modified date and time of the dataSourceContainer.</span></span>|
|<span data-ttu-id="f2de9-126">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2de9-126">releasedDateTime</span></span>|<span data-ttu-id="f2de9-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2de9-127">DateTimeOffset</span></span>|<span data-ttu-id="f2de9-128">Дата и время освобождения dataSourceContainer из дела.</span><span class="sxs-lookup"><span data-stu-id="f2de9-128">Date and time that the dataSourceContainer was released from the case.</span></span>|
|<span data-ttu-id="f2de9-129">status</span><span class="sxs-lookup"><span data-stu-id="f2de9-129">status</span></span>|<span data-ttu-id="f2de9-130">microsoft.graph.ediscovery.dataSourceContainerStatus</span><span class="sxs-lookup"><span data-stu-id="f2de9-130">microsoft.graph.ediscovery.dataSourceContainerStatus</span></span>|<span data-ttu-id="f2de9-131">Последнее состояние dataSourceContainer.</span><span class="sxs-lookup"><span data-stu-id="f2de9-131">Latest status of the dataSourceContainer.</span></span> <span data-ttu-id="f2de9-132">Возможные значения: `Active`, `Released`.</span><span class="sxs-lookup"><span data-stu-id="f2de9-132">Possible values are: `Active`, `Released`.</span></span>|

### <a name="datasourcecontainerstatus-values"></a><span data-ttu-id="f2de9-133">значения dataSourceContainerStatus</span><span class="sxs-lookup"><span data-stu-id="f2de9-133">dataSourceContainerStatus values</span></span>

|<span data-ttu-id="f2de9-134">Member</span><span class="sxs-lookup"><span data-stu-id="f2de9-134">Member</span></span>|<span data-ttu-id="f2de9-135">Описание</span><span class="sxs-lookup"><span data-stu-id="f2de9-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2de9-136">Активное</span><span class="sxs-lookup"><span data-stu-id="f2de9-136">Active</span></span>|<span data-ttu-id="f2de9-137">В этом случае dataSourceContainer находится на удержании.</span><span class="sxs-lookup"><span data-stu-id="f2de9-137">The dataSourceContainer is on hold in the case.</span></span>|
|<span data-ttu-id="f2de9-138">Выпущено</span><span class="sxs-lookup"><span data-stu-id="f2de9-138">Released</span></span>|<span data-ttu-id="f2de9-139">В этом случае dataSourceContainer был освобожден из удержания.</span><span class="sxs-lookup"><span data-stu-id="f2de9-139">The dataSourceContainer was released from hold in the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2de9-140">Связи</span><span class="sxs-lookup"><span data-stu-id="f2de9-140">Relationships</span></span>

<span data-ttu-id="f2de9-141">Нет</span><span class="sxs-lookup"><span data-stu-id="f2de9-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2de9-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2de9-142">JSON representation</span></span>

<span data-ttu-id="f2de9-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2de9-143">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.dataSourceContainer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.dataSourceContainer",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
