---
title: Тип ресурса Ситесаурце
description: Контейнер для сайта, связанного с хранитель.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 60b2d8fb3374dd4f97dcff802caf509e66ca6db1
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597825"
---
# <a name="sitesource-resource-type"></a><span data-ttu-id="42af3-103">Тип ресурса Ситесаурце</span><span class="sxs-lookup"><span data-stu-id="42af3-103">siteSource resource type</span></span>

<span data-ttu-id="42af3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42af3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42af3-105">Контейнер для сайта, связанного с [хранитель](custodian.md).</span><span class="sxs-lookup"><span data-stu-id="42af3-105">The container for a site associated with a [custodian](custodian.md).</span></span>

## <a name="methods"></a><span data-ttu-id="42af3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="42af3-106">Methods</span></span>

|<span data-ttu-id="42af3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="42af3-107">Method</span></span>|<span data-ttu-id="42af3-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="42af3-108">Return type</span></span>|<span data-ttu-id="42af3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="42af3-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42af3-110">Список Ситесаурцес</span><span class="sxs-lookup"><span data-stu-id="42af3-110">List siteSources</span></span>](../api/custodian-list-sitesources.md)|<span data-ttu-id="42af3-111">Коллекция [ситесаурце](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="42af3-111">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="42af3-112">Получение списка объектов **ситесаурце** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="42af3-112">Get a list of **siteSource** objects and their properties.</span></span>|
|[<span data-ttu-id="42af3-113">Создание Ситесаурце</span><span class="sxs-lookup"><span data-stu-id="42af3-113">Create siteSource</span></span>](../api/custodian-post-sitesources.md)|[<span data-ttu-id="42af3-114">ситесаурце</span><span class="sxs-lookup"><span data-stu-id="42af3-114">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="42af3-115">Создание нового объекта **ситесаурце** .</span><span class="sxs-lookup"><span data-stu-id="42af3-115">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="42af3-116">Получение Ситесаурце</span><span class="sxs-lookup"><span data-stu-id="42af3-116">Get siteSource</span></span>](../api/sitesource-get.md)|[<span data-ttu-id="42af3-117">ситесаурце</span><span class="sxs-lookup"><span data-stu-id="42af3-117">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="42af3-118">Чтение свойств и связей объекта **ситесаурце** .</span><span class="sxs-lookup"><span data-stu-id="42af3-118">Read the properties and relationships of a **siteSource** object.</span></span>|
|[<span data-ttu-id="42af3-119">Удаление Ситесаурце</span><span class="sxs-lookup"><span data-stu-id="42af3-119">Delete siteSource</span></span>](../api/sitesource-delete.md)|<span data-ttu-id="42af3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="42af3-120">None</span></span>|<span data-ttu-id="42af3-121">Удаление объекта **ситесаурце** .</span><span class="sxs-lookup"><span data-stu-id="42af3-121">Delete a **siteSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="42af3-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="42af3-122">Properties</span></span>

|<span data-ttu-id="42af3-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="42af3-123">Property</span></span>|<span data-ttu-id="42af3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="42af3-124">Type</span></span>|<span data-ttu-id="42af3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="42af3-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42af3-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="42af3-126">createdBy</span></span>|[<span data-ttu-id="42af3-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="42af3-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="42af3-128">Пользователь, создавший **ситесаурце**.</span><span class="sxs-lookup"><span data-stu-id="42af3-128">The user who created the **siteSource**.</span></span>|
|<span data-ttu-id="42af3-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42af3-129">createdDateTime</span></span>|<span data-ttu-id="42af3-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42af3-130">DateTimeOffset</span></span>|<span data-ttu-id="42af3-131">Дата и время создания **ситесаурце** .</span><span class="sxs-lookup"><span data-stu-id="42af3-131">The date and time the **siteSource** was created.</span></span>|
|<span data-ttu-id="42af3-132">displayName</span><span class="sxs-lookup"><span data-stu-id="42af3-132">displayName</span></span>|<span data-ttu-id="42af3-133">String</span><span class="sxs-lookup"><span data-stu-id="42af3-133">String</span></span>|<span data-ttu-id="42af3-134">Отображаемое имя **ситесаурце**.</span><span class="sxs-lookup"><span data-stu-id="42af3-134">The display name of the **siteSource**.</span></span> <span data-ttu-id="42af3-135">Это будет имя сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="42af3-135">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="42af3-136">id</span><span class="sxs-lookup"><span data-stu-id="42af3-136">id</span></span>|<span data-ttu-id="42af3-137">String</span><span class="sxs-lookup"><span data-stu-id="42af3-137">String</span></span>| <span data-ttu-id="42af3-138">Идентификатор **ситесаурце**.</span><span class="sxs-lookup"><span data-stu-id="42af3-138">The ID of the **siteSource**.</span></span> <span data-ttu-id="42af3-139">Это значение не является ИДЕНТИФИКАТОРом действительного сайта.</span><span class="sxs-lookup"><span data-stu-id="42af3-139">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42af3-140">Связи</span><span class="sxs-lookup"><span data-stu-id="42af3-140">Relationships</span></span>

|<span data-ttu-id="42af3-141">Связь</span><span class="sxs-lookup"><span data-stu-id="42af3-141">Relationship</span></span>|<span data-ttu-id="42af3-142">Тип</span><span class="sxs-lookup"><span data-stu-id="42af3-142">Type</span></span>|<span data-ttu-id="42af3-143">Описание</span><span class="sxs-lookup"><span data-stu-id="42af3-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42af3-144">site</span><span class="sxs-lookup"><span data-stu-id="42af3-144">site</span></span>|[<span data-ttu-id="42af3-145">site</span><span class="sxs-lookup"><span data-stu-id="42af3-145">site</span></span>](../resources/site.md)|<span data-ttu-id="42af3-146">Сайт SharePoint, связанный с **ситесаурце**.</span><span class="sxs-lookup"><span data-stu-id="42af3-146">The SharePoint site associated with the **siteSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42af3-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42af3-147">JSON representation</span></span>

<span data-ttu-id="42af3-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42af3-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.siteSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
