---
title: Тип ресурса linkedResource
description: Представляет источник объекта todoTask
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0a386cd8ed714a6f7127ea0a872a4170997bb8b9
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850081"
---
# <a name="linkedresource-resource-type"></a><span data-ttu-id="1f1cd-103">Тип ресурса linkedResource</span><span class="sxs-lookup"><span data-stu-id="1f1cd-103">linkedResource resource type</span></span>

<span data-ttu-id="1f1cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f1cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f1cd-105">Представляет элемент в партнерском приложении, связанном [с todoTask.](./todotask.md)</span><span class="sxs-lookup"><span data-stu-id="1f1cd-105">Represents an item in a partner application related to a [todoTask](./todotask.md).</span></span> <span data-ttu-id="1f1cd-106">В качестве примера можно приступить к созданию задачи.</span><span class="sxs-lookup"><span data-stu-id="1f1cd-106">An example is an email that created the task.</span></span> <span data-ttu-id="1f1cd-107">В **объекте linkedResource** хранятся сведения о исходном приложении и позволяет связывать его обратно с соответствующим элементом.</span><span class="sxs-lookup"><span data-stu-id="1f1cd-107">A **linkedResource** object stores information about that source application, and lets you link back to the related item.</span></span>

## <a name="methods"></a><span data-ttu-id="1f1cd-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1f1cd-108">Methods</span></span>
|<span data-ttu-id="1f1cd-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1f1cd-109">Method</span></span>|<span data-ttu-id="1f1cd-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="1f1cd-110">Return type</span></span>|<span data-ttu-id="1f1cd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1f1cd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1f1cd-112">Перечисление linkedResources</span><span class="sxs-lookup"><span data-stu-id="1f1cd-112">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="1f1cd-113">[Коллекция linkedResource](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="1f1cd-113">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="1f1cd-114">Получение linkedResources из свойства навигации linkedResources.</span><span class="sxs-lookup"><span data-stu-id="1f1cd-114">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="1f1cd-115">Создание linkedResource</span><span class="sxs-lookup"><span data-stu-id="1f1cd-115">Create linkedResource</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="1f1cd-116">linkedResource</span><span class="sxs-lookup"><span data-stu-id="1f1cd-116">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="1f1cd-117">Создание объекта linkedResources.</span><span class="sxs-lookup"><span data-stu-id="1f1cd-117">Create a new linkedResources object.</span></span>|
|[<span data-ttu-id="1f1cd-118">Получение linkedResource</span><span class="sxs-lookup"><span data-stu-id="1f1cd-118">Get linkedResource</span></span>](../api/linkedresource-get.md)|[<span data-ttu-id="1f1cd-119">linkedResource</span><span class="sxs-lookup"><span data-stu-id="1f1cd-119">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="1f1cd-120">Чтение свойств и связей [объекта linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="1f1cd-120">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="1f1cd-121">Обновление linkedResource</span><span class="sxs-lookup"><span data-stu-id="1f1cd-121">Update linkedResource</span></span>](../api/linkedresource-update.md)|[<span data-ttu-id="1f1cd-122">linkedResource</span><span class="sxs-lookup"><span data-stu-id="1f1cd-122">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="1f1cd-123">Обновление свойств объекта [linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="1f1cd-123">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="1f1cd-124">Удаление linkedResource</span><span class="sxs-lookup"><span data-stu-id="1f1cd-124">Delete linkedResource</span></span>](../api/linkedresource-delete.md)|<span data-ttu-id="1f1cd-125">Нет</span><span class="sxs-lookup"><span data-stu-id="1f1cd-125">None</span></span>|<span data-ttu-id="1f1cd-126">Удаляет объект [linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="1f1cd-126">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f1cd-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f1cd-127">Properties</span></span>
|<span data-ttu-id="1f1cd-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f1cd-128">Property</span></span>|<span data-ttu-id="1f1cd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1f1cd-129">Type</span></span>|<span data-ttu-id="1f1cd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1f1cd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f1cd-131">applicationName</span><span class="sxs-lookup"><span data-stu-id="1f1cd-131">applicationName</span></span>|<span data-ttu-id="1f1cd-132">String</span><span class="sxs-lookup"><span data-stu-id="1f1cd-132">String</span></span>|<span data-ttu-id="1f1cd-133">Поле, указывающее имя приложения источника, отправляющего **linkedResource.**</span><span class="sxs-lookup"><span data-stu-id="1f1cd-133">Field indicating the app name of the source that is sending the **linkedResource**.</span></span>|
|<span data-ttu-id="1f1cd-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1f1cd-134">displayName</span></span>|<span data-ttu-id="1f1cd-135">String</span><span class="sxs-lookup"><span data-stu-id="1f1cd-135">String</span></span>|<span data-ttu-id="1f1cd-136">Поле, обозначающее **заголовок связанного ресурса.**</span><span class="sxs-lookup"><span data-stu-id="1f1cd-136">Field indicating the title of the **linkedResource**.</span></span>|
|<span data-ttu-id="1f1cd-137">externalId</span><span class="sxs-lookup"><span data-stu-id="1f1cd-137">externalId</span></span>|<span data-ttu-id="1f1cd-138">String</span><span class="sxs-lookup"><span data-stu-id="1f1cd-138">String</span></span>|<span data-ttu-id="1f1cd-139">Идентификатор объекта, связанного с этой задачей в сторонней или партнерской системе.</span><span class="sxs-lookup"><span data-stu-id="1f1cd-139">Id of the object that is associated with this task on the third-party/partner system.</span></span>|
|<span data-ttu-id="1f1cd-140">id</span><span class="sxs-lookup"><span data-stu-id="1f1cd-140">id</span></span>|<span data-ttu-id="1f1cd-141">String</span><span class="sxs-lookup"><span data-stu-id="1f1cd-141">String</span></span>|<span data-ttu-id="1f1cd-142">Созданный сервером ИД **для linkedResource.**</span><span class="sxs-lookup"><span data-stu-id="1f1cd-142">Server generated ID for the **linkedResource**.</span></span> <span data-ttu-id="1f1cd-143">Наследуется от [объекта.](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="1f1cd-143">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="1f1cd-144">webUrl</span><span class="sxs-lookup"><span data-stu-id="1f1cd-144">webUrl</span></span>|<span data-ttu-id="1f1cd-145">String</span><span class="sxs-lookup"><span data-stu-id="1f1cd-145">String</span></span>|<span data-ttu-id="1f1cd-146">Глубокая ссылка **на связанныйресурс.**</span><span class="sxs-lookup"><span data-stu-id="1f1cd-146">Deep link to the **linkedResource**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f1cd-147">Связи</span><span class="sxs-lookup"><span data-stu-id="1f1cd-147">Relationships</span></span>
<span data-ttu-id="1f1cd-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1f1cd-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f1cd-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1f1cd-149">JSON representation</span></span>
<span data-ttu-id="1f1cd-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f1cd-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.linkedResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "String (identifier)",
  "webUrl": "String",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String"
}
```

