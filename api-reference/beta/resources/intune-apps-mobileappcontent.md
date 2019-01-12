---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 57266335608e97924edbddc056d931725a633e4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939121"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="5bc4c-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="5bc4c-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="5bc4c-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5bc4c-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bc4c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bc4c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5bc4c-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5bc4c-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5bc4c-108">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="5bc4c-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="5bc4c-109">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="5bc4c-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="5bc4c-110">Методы</span><span class="sxs-lookup"><span data-stu-id="5bc4c-110">Methods</span></span>
|<span data-ttu-id="5bc4c-111">Метод</span><span class="sxs-lookup"><span data-stu-id="5bc4c-111">Method</span></span>|<span data-ttu-id="5bc4c-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5bc4c-112">Return Type</span></span>|<span data-ttu-id="5bc4c-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5bc4c-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5bc4c-114">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="5bc4c-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="5bc4c-115">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="5bc4c-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="5bc4c-116">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="5bc4c-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="5bc4c-117">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="5bc4c-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="5bc4c-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="5bc4c-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="5bc4c-119">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="5bc4c-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="5bc4c-120">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="5bc4c-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="5bc4c-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="5bc4c-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="5bc4c-122">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="5bc4c-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="5bc4c-123">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="5bc4c-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="5bc4c-124">Нет</span><span class="sxs-lookup"><span data-stu-id="5bc4c-124">None</span></span>|<span data-ttu-id="5bc4c-125">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="5bc4c-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="5bc4c-126">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="5bc4c-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="5bc4c-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="5bc4c-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="5bc4c-128">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="5bc4c-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5bc4c-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="5bc4c-129">Properties</span></span>
|<span data-ttu-id="5bc4c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bc4c-130">Property</span></span>|<span data-ttu-id="5bc4c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5bc4c-131">Type</span></span>|<span data-ttu-id="5bc4c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5bc4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bc4c-133">id</span><span class="sxs-lookup"><span data-stu-id="5bc4c-133">id</span></span>|<span data-ttu-id="5bc4c-134">String</span><span class="sxs-lookup"><span data-stu-id="5bc4c-134">String</span></span>|<span data-ttu-id="5bc4c-135">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="5bc4c-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5bc4c-136">Связи</span><span class="sxs-lookup"><span data-stu-id="5bc4c-136">Relationships</span></span>
|<span data-ttu-id="5bc4c-137">Связь</span><span class="sxs-lookup"><span data-stu-id="5bc4c-137">Relationship</span></span>|<span data-ttu-id="5bc4c-138">Тип</span><span class="sxs-lookup"><span data-stu-id="5bc4c-138">Type</span></span>|<span data-ttu-id="5bc4c-139">Описание</span><span class="sxs-lookup"><span data-stu-id="5bc4c-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bc4c-140">files</span><span class="sxs-lookup"><span data-stu-id="5bc4c-140">files</span></span>|<span data-ttu-id="5bc4c-141">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="5bc4c-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="5bc4c-142">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="5bc4c-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="5bc4c-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="5bc4c-143">containedApps</span></span>|<span data-ttu-id="5bc4c-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5bc4c-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="5bc4c-145">Коллекция автономные приложения в MobileLobApp, работающие в качестве пакета.</span><span class="sxs-lookup"><span data-stu-id="5bc4c-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bc4c-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5bc4c-146">JSON Representation</span></span>
<span data-ttu-id="5bc4c-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bc4c-147">Here is a JSON representation of the resource.</span></span>
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





