---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 090a55e73ac823101386c23b18811163131099a6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327516"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="d4fa8-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="d4fa8-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="d4fa8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4fa8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4fa8-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4fa8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4fa8-107">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="d4fa8-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="d4fa8-108">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="d4fa8-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="d4fa8-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d4fa8-109">Methods</span></span>
|<span data-ttu-id="d4fa8-110">Метод</span><span class="sxs-lookup"><span data-stu-id="d4fa8-110">Method</span></span>|<span data-ttu-id="d4fa8-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d4fa8-111">Return Type</span></span>|<span data-ttu-id="d4fa8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d4fa8-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4fa8-113">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="d4fa8-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="d4fa8-114">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="d4fa8-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="d4fa8-115">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="d4fa8-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="d4fa8-116">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="d4fa8-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|<span data-ttu-id="d4fa8-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="d4fa8-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="d4fa8-118">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="d4fa8-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="d4fa8-119">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="d4fa8-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|<span data-ttu-id="d4fa8-120">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="d4fa8-120">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="d4fa8-121">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="d4fa8-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="d4fa8-122">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="d4fa8-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="d4fa8-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d4fa8-123">None</span></span>|<span data-ttu-id="d4fa8-124">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="d4fa8-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="d4fa8-125">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="d4fa8-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="d4fa8-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="d4fa8-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="d4fa8-127">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="d4fa8-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4fa8-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4fa8-128">Properties</span></span>
|<span data-ttu-id="d4fa8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4fa8-129">Property</span></span>|<span data-ttu-id="d4fa8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d4fa8-130">Type</span></span>|<span data-ttu-id="d4fa8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d4fa8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4fa8-132">id</span><span class="sxs-lookup"><span data-stu-id="d4fa8-132">id</span></span>|<span data-ttu-id="d4fa8-133">String</span><span class="sxs-lookup"><span data-stu-id="d4fa8-133">String</span></span>|<span data-ttu-id="d4fa8-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="d4fa8-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4fa8-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="d4fa8-135">Relationships</span></span>
|<span data-ttu-id="d4fa8-136">Отношение</span><span class="sxs-lookup"><span data-stu-id="d4fa8-136">Relationship</span></span>|<span data-ttu-id="d4fa8-137">Тип</span><span class="sxs-lookup"><span data-stu-id="d4fa8-137">Type</span></span>|<span data-ttu-id="d4fa8-138">Описание</span><span class="sxs-lookup"><span data-stu-id="d4fa8-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4fa8-139">files</span><span class="sxs-lookup"><span data-stu-id="d4fa8-139">files</span></span>|<span data-ttu-id="d4fa8-140">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="d4fa8-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="d4fa8-141">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="d4fa8-141">The list of files for this app content version.</span></span>|
|<span data-ttu-id="d4fa8-142">containedApps</span><span class="sxs-lookup"><span data-stu-id="d4fa8-142">containedApps</span></span>|<span data-ttu-id="d4fa8-143">Коллекция [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4fa8-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="d4fa8-144">Коллекция вложенных приложений в MobileLobApp, действующая в виде пакета.</span><span class="sxs-lookup"><span data-stu-id="d4fa8-144">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4fa8-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4fa8-145">JSON Representation</span></span>
<span data-ttu-id="d4fa8-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4fa8-146">Here is a JSON representation of the resource.</span></span>
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



