---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4d0a97affa024a5a38e034b53a66b9c1c629cc96
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354072"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="bba33-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="bba33-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="bba33-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bba33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bba33-106">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="bba33-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="bba33-107">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="bba33-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="bba33-108">Методы</span><span class="sxs-lookup"><span data-stu-id="bba33-108">Methods</span></span>
|<span data-ttu-id="bba33-109">Метод</span><span class="sxs-lookup"><span data-stu-id="bba33-109">Method</span></span>|<span data-ttu-id="bba33-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bba33-110">Return Type</span></span>|<span data-ttu-id="bba33-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bba33-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bba33-112">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="bba33-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="bba33-113">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="bba33-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="bba33-114">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="bba33-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="bba33-115">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="bba33-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|<span data-ttu-id="bba33-116">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="bba33-116">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="bba33-117">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="bba33-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="bba33-118">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="bba33-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|<span data-ttu-id="bba33-119">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="bba33-119">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="bba33-120">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="bba33-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="bba33-121">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="bba33-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="bba33-122">Нет</span><span class="sxs-lookup"><span data-stu-id="bba33-122">None</span></span>|<span data-ttu-id="bba33-123">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="bba33-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="bba33-124">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="bba33-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="bba33-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="bba33-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="bba33-126">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="bba33-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bba33-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="bba33-127">Properties</span></span>
|<span data-ttu-id="bba33-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bba33-128">Property</span></span>|<span data-ttu-id="bba33-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bba33-129">Type</span></span>|<span data-ttu-id="bba33-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bba33-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bba33-131">id</span><span class="sxs-lookup"><span data-stu-id="bba33-131">id</span></span>|<span data-ttu-id="bba33-132">String</span><span class="sxs-lookup"><span data-stu-id="bba33-132">String</span></span>|<span data-ttu-id="bba33-133">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="bba33-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bba33-134">Связи</span><span class="sxs-lookup"><span data-stu-id="bba33-134">Relationships</span></span>
|<span data-ttu-id="bba33-135">Связь</span><span class="sxs-lookup"><span data-stu-id="bba33-135">Relationship</span></span>|<span data-ttu-id="bba33-136">Тип</span><span class="sxs-lookup"><span data-stu-id="bba33-136">Type</span></span>|<span data-ttu-id="bba33-137">Описание</span><span class="sxs-lookup"><span data-stu-id="bba33-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bba33-138">files</span><span class="sxs-lookup"><span data-stu-id="bba33-138">files</span></span>|<span data-ttu-id="bba33-139">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="bba33-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="bba33-140">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="bba33-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bba33-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bba33-141">JSON Representation</span></span>
<span data-ttu-id="bba33-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bba33-142">Here is a JSON representation of the resource.</span></span>
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




