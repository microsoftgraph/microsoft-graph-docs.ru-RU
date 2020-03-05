---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 62effaf4c2f970e8c6dc5b88d0a677dd90b33e5a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491888"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="04fea-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="04fea-104">mobileAppContent resource type</span></span>

<span data-ttu-id="04fea-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="04fea-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04fea-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04fea-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04fea-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04fea-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04fea-108">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="04fea-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="04fea-109">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="04fea-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="04fea-110">Методы</span><span class="sxs-lookup"><span data-stu-id="04fea-110">Methods</span></span>
|<span data-ttu-id="04fea-111">Метод</span><span class="sxs-lookup"><span data-stu-id="04fea-111">Method</span></span>|<span data-ttu-id="04fea-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="04fea-112">Return Type</span></span>|<span data-ttu-id="04fea-113">Описание</span><span class="sxs-lookup"><span data-stu-id="04fea-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="04fea-114">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="04fea-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="04fea-115">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="04fea-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="04fea-116">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="04fea-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="04fea-117">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="04fea-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|<span data-ttu-id="04fea-118">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="04fea-118">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="04fea-119">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="04fea-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="04fea-120">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="04fea-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|<span data-ttu-id="04fea-121">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="04fea-121">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="04fea-122">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="04fea-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="04fea-123">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="04fea-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="04fea-124">Нет</span><span class="sxs-lookup"><span data-stu-id="04fea-124">None</span></span>|<span data-ttu-id="04fea-125">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="04fea-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="04fea-126">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="04fea-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="04fea-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="04fea-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="04fea-128">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="04fea-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="04fea-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="04fea-129">Properties</span></span>
|<span data-ttu-id="04fea-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="04fea-130">Property</span></span>|<span data-ttu-id="04fea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="04fea-131">Type</span></span>|<span data-ttu-id="04fea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="04fea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04fea-133">id</span><span class="sxs-lookup"><span data-stu-id="04fea-133">id</span></span>|<span data-ttu-id="04fea-134">String</span><span class="sxs-lookup"><span data-stu-id="04fea-134">String</span></span>|<span data-ttu-id="04fea-135">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="04fea-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04fea-136">Связи</span><span class="sxs-lookup"><span data-stu-id="04fea-136">Relationships</span></span>
|<span data-ttu-id="04fea-137">Связь</span><span class="sxs-lookup"><span data-stu-id="04fea-137">Relationship</span></span>|<span data-ttu-id="04fea-138">Тип</span><span class="sxs-lookup"><span data-stu-id="04fea-138">Type</span></span>|<span data-ttu-id="04fea-139">Описание</span><span class="sxs-lookup"><span data-stu-id="04fea-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04fea-140">files</span><span class="sxs-lookup"><span data-stu-id="04fea-140">files</span></span>|<span data-ttu-id="04fea-141">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="04fea-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="04fea-142">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="04fea-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="04fea-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="04fea-143">containedApps</span></span>|<span data-ttu-id="04fea-144">Коллекция [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="04fea-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="04fea-145">Коллекция вложенных приложений в MobileLobApp, действующая в виде пакета.</span><span class="sxs-lookup"><span data-stu-id="04fea-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04fea-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04fea-146">JSON Representation</span></span>
<span data-ttu-id="04fea-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04fea-147">Here is a JSON representation of the resource.</span></span>
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



