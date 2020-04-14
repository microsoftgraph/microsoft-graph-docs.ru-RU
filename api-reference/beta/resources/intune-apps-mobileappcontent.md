---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 96058f7af6bdf375ffdc2a6df4558afd96145627
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458585"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="e4541-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e4541-104">mobileAppContent resource type</span></span>

<span data-ttu-id="e4541-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4541-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4541-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4541-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4541-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4541-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4541-108">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="e4541-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="e4541-109">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="e4541-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="e4541-110">Методы</span><span class="sxs-lookup"><span data-stu-id="e4541-110">Methods</span></span>
|<span data-ttu-id="e4541-111">Метод</span><span class="sxs-lookup"><span data-stu-id="e4541-111">Method</span></span>|<span data-ttu-id="e4541-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e4541-112">Return Type</span></span>|<span data-ttu-id="e4541-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e4541-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4541-114">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="e4541-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="e4541-115">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="e4541-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="e4541-116">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e4541-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="e4541-117">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e4541-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|<span data-ttu-id="e4541-118">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="e4541-118">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="e4541-119">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e4541-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="e4541-120">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e4541-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|<span data-ttu-id="e4541-121">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="e4541-121">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="e4541-122">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e4541-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="e4541-123">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e4541-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="e4541-124">Нет</span><span class="sxs-lookup"><span data-stu-id="e4541-124">None</span></span>|<span data-ttu-id="e4541-125">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e4541-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="e4541-126">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e4541-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="e4541-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e4541-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="e4541-128">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="e4541-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4541-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4541-129">Properties</span></span>
|<span data-ttu-id="e4541-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4541-130">Property</span></span>|<span data-ttu-id="e4541-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e4541-131">Type</span></span>|<span data-ttu-id="e4541-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e4541-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4541-133">id</span><span class="sxs-lookup"><span data-stu-id="e4541-133">id</span></span>|<span data-ttu-id="e4541-134">String</span><span class="sxs-lookup"><span data-stu-id="e4541-134">String</span></span>|<span data-ttu-id="e4541-135">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="e4541-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4541-136">Связи</span><span class="sxs-lookup"><span data-stu-id="e4541-136">Relationships</span></span>
|<span data-ttu-id="e4541-137">Связь</span><span class="sxs-lookup"><span data-stu-id="e4541-137">Relationship</span></span>|<span data-ttu-id="e4541-138">Тип</span><span class="sxs-lookup"><span data-stu-id="e4541-138">Type</span></span>|<span data-ttu-id="e4541-139">Описание</span><span class="sxs-lookup"><span data-stu-id="e4541-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4541-140">files</span><span class="sxs-lookup"><span data-stu-id="e4541-140">files</span></span>|<span data-ttu-id="e4541-141">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="e4541-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="e4541-142">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="e4541-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="e4541-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="e4541-143">containedApps</span></span>|<span data-ttu-id="e4541-144">Коллекция [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4541-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="e4541-145">Коллекция вложенных приложений в MobileLobApp, действующая в виде пакета.</span><span class="sxs-lookup"><span data-stu-id="e4541-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4541-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4541-146">JSON Representation</span></span>
<span data-ttu-id="e4541-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4541-147">Here is a JSON representation of the resource.</span></span>
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



