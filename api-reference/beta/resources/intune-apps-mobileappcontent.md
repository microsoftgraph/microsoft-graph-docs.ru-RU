---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ceeb6cd4e989f4e020c885dde119c39d9659539c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418185"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="765a0-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="765a0-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="765a0-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="765a0-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="765a0-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="765a0-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="765a0-107">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="765a0-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="765a0-108">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="765a0-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="765a0-109">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="765a0-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="765a0-110">Методы</span><span class="sxs-lookup"><span data-stu-id="765a0-110">Methods</span></span>
|<span data-ttu-id="765a0-111">Метод</span><span class="sxs-lookup"><span data-stu-id="765a0-111">Method</span></span>|<span data-ttu-id="765a0-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="765a0-112">Return Type</span></span>|<span data-ttu-id="765a0-113">Описание</span><span class="sxs-lookup"><span data-stu-id="765a0-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="765a0-114">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="765a0-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="765a0-115">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="765a0-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="765a0-116">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="765a0-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="765a0-117">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="765a0-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="765a0-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="765a0-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="765a0-119">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="765a0-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="765a0-120">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="765a0-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="765a0-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="765a0-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="765a0-122">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="765a0-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="765a0-123">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="765a0-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="765a0-124">Нет</span><span class="sxs-lookup"><span data-stu-id="765a0-124">None</span></span>|<span data-ttu-id="765a0-125">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="765a0-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="765a0-126">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="765a0-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="765a0-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="765a0-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="765a0-128">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="765a0-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="765a0-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="765a0-129">Properties</span></span>
|<span data-ttu-id="765a0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="765a0-130">Property</span></span>|<span data-ttu-id="765a0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="765a0-131">Type</span></span>|<span data-ttu-id="765a0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="765a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="765a0-133">id</span><span class="sxs-lookup"><span data-stu-id="765a0-133">id</span></span>|<span data-ttu-id="765a0-134">String</span><span class="sxs-lookup"><span data-stu-id="765a0-134">String</span></span>|<span data-ttu-id="765a0-135">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="765a0-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="765a0-136">Связи</span><span class="sxs-lookup"><span data-stu-id="765a0-136">Relationships</span></span>
|<span data-ttu-id="765a0-137">Связь</span><span class="sxs-lookup"><span data-stu-id="765a0-137">Relationship</span></span>|<span data-ttu-id="765a0-138">Тип</span><span class="sxs-lookup"><span data-stu-id="765a0-138">Type</span></span>|<span data-ttu-id="765a0-139">Описание</span><span class="sxs-lookup"><span data-stu-id="765a0-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="765a0-140">files</span><span class="sxs-lookup"><span data-stu-id="765a0-140">files</span></span>|<span data-ttu-id="765a0-141">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="765a0-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="765a0-142">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="765a0-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="765a0-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="765a0-143">containedApps</span></span>|<span data-ttu-id="765a0-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="765a0-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="765a0-145">Коллекция автономные приложения в MobileLobApp, работающие в качестве пакета.</span><span class="sxs-lookup"><span data-stu-id="765a0-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="765a0-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="765a0-146">JSON Representation</span></span>
<span data-ttu-id="765a0-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="765a0-147">Here is a JSON representation of the resource.</span></span>
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




