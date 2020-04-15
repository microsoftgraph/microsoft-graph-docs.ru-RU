---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e25318e22007e202586e1c629c2d932a30bbab1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410949"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="e362a-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e362a-104">mobileAppContent resource type</span></span>

<span data-ttu-id="e362a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e362a-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e362a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e362a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e362a-107">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="e362a-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="e362a-108">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="e362a-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="e362a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="e362a-109">Methods</span></span>
|<span data-ttu-id="e362a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="e362a-110">Method</span></span>|<span data-ttu-id="e362a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e362a-111">Return Type</span></span>|<span data-ttu-id="e362a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e362a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e362a-113">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="e362a-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="e362a-114">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="e362a-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="e362a-115">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e362a-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="e362a-116">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e362a-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|<span data-ttu-id="e362a-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="e362a-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="e362a-118">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e362a-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="e362a-119">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e362a-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|<span data-ttu-id="e362a-120">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="e362a-120">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="e362a-121">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e362a-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="e362a-122">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e362a-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="e362a-123">Нет</span><span class="sxs-lookup"><span data-stu-id="e362a-123">None</span></span>|<span data-ttu-id="e362a-124">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e362a-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="e362a-125">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e362a-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="e362a-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e362a-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="e362a-127">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e362a-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e362a-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="e362a-128">Properties</span></span>
|<span data-ttu-id="e362a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e362a-129">Property</span></span>|<span data-ttu-id="e362a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e362a-130">Type</span></span>|<span data-ttu-id="e362a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e362a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e362a-132">id</span><span class="sxs-lookup"><span data-stu-id="e362a-132">id</span></span>|<span data-ttu-id="e362a-133">String</span><span class="sxs-lookup"><span data-stu-id="e362a-133">String</span></span>|<span data-ttu-id="e362a-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="e362a-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e362a-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="e362a-135">Relationships</span></span>
|<span data-ttu-id="e362a-136">Связь</span><span class="sxs-lookup"><span data-stu-id="e362a-136">Relationship</span></span>|<span data-ttu-id="e362a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="e362a-137">Type</span></span>|<span data-ttu-id="e362a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="e362a-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e362a-139">files</span><span class="sxs-lookup"><span data-stu-id="e362a-139">files</span></span>|<span data-ttu-id="e362a-140">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="e362a-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="e362a-141">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="e362a-141">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e362a-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e362a-142">JSON Representation</span></span>
<span data-ttu-id="e362a-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e362a-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```







