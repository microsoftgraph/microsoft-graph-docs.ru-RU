---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a3ed4b5d1e05b3d1f8621cecf875a6fbbe9d740
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990311"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="3d56b-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="3d56b-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="3d56b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d56b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d56b-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d56b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d56b-107">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="3d56b-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="3d56b-108">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="3d56b-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="3d56b-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3d56b-109">Methods</span></span>
|<span data-ttu-id="3d56b-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3d56b-110">Method</span></span>|<span data-ttu-id="3d56b-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3d56b-111">Return Type</span></span>|<span data-ttu-id="3d56b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3d56b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3d56b-113">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="3d56b-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="3d56b-114">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="3d56b-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="3d56b-115">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="3d56b-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="3d56b-116">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="3d56b-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|<span data-ttu-id="3d56b-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="3d56b-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="3d56b-118">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="3d56b-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="3d56b-119">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="3d56b-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|<span data-ttu-id="3d56b-120">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="3d56b-120">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="3d56b-121">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="3d56b-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="3d56b-122">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="3d56b-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="3d56b-123">Нет</span><span class="sxs-lookup"><span data-stu-id="3d56b-123">None</span></span>|<span data-ttu-id="3d56b-124">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="3d56b-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="3d56b-125">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="3d56b-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="3d56b-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="3d56b-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="3d56b-127">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="3d56b-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3d56b-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d56b-128">Properties</span></span>
|<span data-ttu-id="3d56b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d56b-129">Property</span></span>|<span data-ttu-id="3d56b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3d56b-130">Type</span></span>|<span data-ttu-id="3d56b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3d56b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d56b-132">id</span><span class="sxs-lookup"><span data-stu-id="3d56b-132">id</span></span>|<span data-ttu-id="3d56b-133">String</span><span class="sxs-lookup"><span data-stu-id="3d56b-133">String</span></span>|<span data-ttu-id="3d56b-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="3d56b-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d56b-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="3d56b-135">Relationships</span></span>
|<span data-ttu-id="3d56b-136">Отношение</span><span class="sxs-lookup"><span data-stu-id="3d56b-136">Relationship</span></span>|<span data-ttu-id="3d56b-137">Тип</span><span class="sxs-lookup"><span data-stu-id="3d56b-137">Type</span></span>|<span data-ttu-id="3d56b-138">Описание</span><span class="sxs-lookup"><span data-stu-id="3d56b-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d56b-139">files</span><span class="sxs-lookup"><span data-stu-id="3d56b-139">files</span></span>|<span data-ttu-id="3d56b-140">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="3d56b-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="3d56b-141">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="3d56b-141">The list of files for this app content version.</span></span>|
|<span data-ttu-id="3d56b-142">containedApps</span><span class="sxs-lookup"><span data-stu-id="3d56b-142">containedApps</span></span>|<span data-ttu-id="3d56b-143">Коллекция [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d56b-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="3d56b-144">Коллекция вложенных приложений в MobileLobApp, действующая в виде пакета.</span><span class="sxs-lookup"><span data-stu-id="3d56b-144">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d56b-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d56b-145">JSON Representation</span></span>
<span data-ttu-id="3d56b-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d56b-146">Here is a JSON representation of the resource.</span></span>
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





