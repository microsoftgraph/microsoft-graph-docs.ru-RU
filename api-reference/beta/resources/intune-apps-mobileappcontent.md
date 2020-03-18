---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5cc1888288809812b0b2af533641fd61161cee08
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797848"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="a36de-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a36de-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="a36de-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a36de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a36de-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a36de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a36de-107">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="a36de-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="a36de-108">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="a36de-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="a36de-109">Методы</span><span class="sxs-lookup"><span data-stu-id="a36de-109">Methods</span></span>
|<span data-ttu-id="a36de-110">Метод</span><span class="sxs-lookup"><span data-stu-id="a36de-110">Method</span></span>|<span data-ttu-id="a36de-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a36de-111">Return Type</span></span>|<span data-ttu-id="a36de-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a36de-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a36de-113">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="a36de-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="a36de-114">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="a36de-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="a36de-115">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a36de-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="a36de-116">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a36de-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|<span data-ttu-id="a36de-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="a36de-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="a36de-118">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a36de-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="a36de-119">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a36de-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|<span data-ttu-id="a36de-120">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="a36de-120">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="a36de-121">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a36de-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="a36de-122">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a36de-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="a36de-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a36de-123">None</span></span>|<span data-ttu-id="a36de-124">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a36de-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="a36de-125">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a36de-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="a36de-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a36de-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="a36de-127">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a36de-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a36de-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="a36de-128">Properties</span></span>
|<span data-ttu-id="a36de-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a36de-129">Property</span></span>|<span data-ttu-id="a36de-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a36de-130">Type</span></span>|<span data-ttu-id="a36de-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a36de-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a36de-132">id</span><span class="sxs-lookup"><span data-stu-id="a36de-132">id</span></span>|<span data-ttu-id="a36de-133">String</span><span class="sxs-lookup"><span data-stu-id="a36de-133">String</span></span>|<span data-ttu-id="a36de-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="a36de-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a36de-135">Связи</span><span class="sxs-lookup"><span data-stu-id="a36de-135">Relationships</span></span>
|<span data-ttu-id="a36de-136">Связь</span><span class="sxs-lookup"><span data-stu-id="a36de-136">Relationship</span></span>|<span data-ttu-id="a36de-137">Тип</span><span class="sxs-lookup"><span data-stu-id="a36de-137">Type</span></span>|<span data-ttu-id="a36de-138">Описание</span><span class="sxs-lookup"><span data-stu-id="a36de-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a36de-139">files</span><span class="sxs-lookup"><span data-stu-id="a36de-139">files</span></span>|<span data-ttu-id="a36de-140">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="a36de-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="a36de-141">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="a36de-141">The list of files for this app content version.</span></span>|
|<span data-ttu-id="a36de-142">containedApps</span><span class="sxs-lookup"><span data-stu-id="a36de-142">containedApps</span></span>|<span data-ttu-id="a36de-143">Коллекция [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="a36de-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="a36de-144">Коллекция вложенных приложений в MobileLobApp, действующая в виде пакета.</span><span class="sxs-lookup"><span data-stu-id="a36de-144">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a36de-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a36de-145">JSON Representation</span></span>
<span data-ttu-id="a36de-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a36de-146">Here is a JSON representation of the resource.</span></span>
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



