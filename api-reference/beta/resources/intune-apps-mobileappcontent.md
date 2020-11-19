---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd09faa187f6621f07d2811a90ca706a6da24db6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281070"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="cb970-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="cb970-104">mobileAppContent resource type</span></span>

<span data-ttu-id="cb970-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb970-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb970-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb970-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb970-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb970-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb970-108">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="cb970-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="cb970-109">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="cb970-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="cb970-110">Методы</span><span class="sxs-lookup"><span data-stu-id="cb970-110">Methods</span></span>
|<span data-ttu-id="cb970-111">Метод</span><span class="sxs-lookup"><span data-stu-id="cb970-111">Method</span></span>|<span data-ttu-id="cb970-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cb970-112">Return Type</span></span>|<span data-ttu-id="cb970-113">Описание</span><span class="sxs-lookup"><span data-stu-id="cb970-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb970-114">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="cb970-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="cb970-115">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="cb970-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="cb970-116">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="cb970-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="cb970-117">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="cb970-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="cb970-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="cb970-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="cb970-119">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="cb970-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="cb970-120">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="cb970-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="cb970-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="cb970-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="cb970-122">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="cb970-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="cb970-123">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="cb970-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="cb970-124">Нет</span><span class="sxs-lookup"><span data-stu-id="cb970-124">None</span></span>|<span data-ttu-id="cb970-125">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="cb970-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="cb970-126">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="cb970-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="cb970-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="cb970-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="cb970-128">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="cb970-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb970-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb970-129">Properties</span></span>
|<span data-ttu-id="cb970-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb970-130">Property</span></span>|<span data-ttu-id="cb970-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cb970-131">Type</span></span>|<span data-ttu-id="cb970-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cb970-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb970-133">id</span><span class="sxs-lookup"><span data-stu-id="cb970-133">id</span></span>|<span data-ttu-id="cb970-134">String</span><span class="sxs-lookup"><span data-stu-id="cb970-134">String</span></span>|<span data-ttu-id="cb970-135">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="cb970-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb970-136">Связи</span><span class="sxs-lookup"><span data-stu-id="cb970-136">Relationships</span></span>
|<span data-ttu-id="cb970-137">Связь</span><span class="sxs-lookup"><span data-stu-id="cb970-137">Relationship</span></span>|<span data-ttu-id="cb970-138">Тип</span><span class="sxs-lookup"><span data-stu-id="cb970-138">Type</span></span>|<span data-ttu-id="cb970-139">Описание</span><span class="sxs-lookup"><span data-stu-id="cb970-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb970-140">files</span><span class="sxs-lookup"><span data-stu-id="cb970-140">files</span></span>|<span data-ttu-id="cb970-141">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="cb970-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="cb970-142">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="cb970-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="cb970-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="cb970-143">containedApps</span></span>|<span data-ttu-id="cb970-144">Коллекция [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb970-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="cb970-145">Коллекция вложенных приложений в MobileLobApp, действующая в виде пакета.</span><span class="sxs-lookup"><span data-stu-id="cb970-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb970-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb970-146">JSON Representation</span></span>
<span data-ttu-id="cb970-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb970-147">Here is a JSON representation of the resource.</span></span>
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




