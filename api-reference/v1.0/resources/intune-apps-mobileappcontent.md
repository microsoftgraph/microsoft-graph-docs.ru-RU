---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9cde82585bdbe4ca4c15102e6b343810f29fdae8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261301"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="ccf9b-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccf9b-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="ccf9b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccf9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccf9b-106">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="ccf9b-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="ccf9b-107">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="ccf9b-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="ccf9b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ccf9b-108">Methods</span></span>
|<span data-ttu-id="ccf9b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ccf9b-109">Method</span></span>|<span data-ttu-id="ccf9b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ccf9b-110">Return Type</span></span>|<span data-ttu-id="ccf9b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ccf9b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ccf9b-112">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="ccf9b-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="ccf9b-113">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="ccf9b-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="ccf9b-114">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ccf9b-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="ccf9b-115">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccf9b-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|<span data-ttu-id="ccf9b-116">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="ccf9b-116">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="ccf9b-117">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ccf9b-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ccf9b-118">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccf9b-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|<span data-ttu-id="ccf9b-119">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="ccf9b-119">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="ccf9b-120">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ccf9b-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ccf9b-121">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccf9b-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="ccf9b-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ccf9b-122">None</span></span>|<span data-ttu-id="ccf9b-123">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ccf9b-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="ccf9b-124">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccf9b-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="ccf9b-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ccf9b-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="ccf9b-126">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ccf9b-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ccf9b-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="ccf9b-127">Properties</span></span>
|<span data-ttu-id="ccf9b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccf9b-128">Property</span></span>|<span data-ttu-id="ccf9b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ccf9b-129">Type</span></span>|<span data-ttu-id="ccf9b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ccf9b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccf9b-131">id</span><span class="sxs-lookup"><span data-stu-id="ccf9b-131">id</span></span>|<span data-ttu-id="ccf9b-132">String</span><span class="sxs-lookup"><span data-stu-id="ccf9b-132">String</span></span>|<span data-ttu-id="ccf9b-133">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="ccf9b-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccf9b-134">Связи</span><span class="sxs-lookup"><span data-stu-id="ccf9b-134">Relationships</span></span>
|<span data-ttu-id="ccf9b-135">Отношение</span><span class="sxs-lookup"><span data-stu-id="ccf9b-135">Relationship</span></span>|<span data-ttu-id="ccf9b-136">Тип</span><span class="sxs-lookup"><span data-stu-id="ccf9b-136">Type</span></span>|<span data-ttu-id="ccf9b-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ccf9b-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccf9b-138">files</span><span class="sxs-lookup"><span data-stu-id="ccf9b-138">files</span></span>|<span data-ttu-id="ccf9b-139">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="ccf9b-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="ccf9b-140">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="ccf9b-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ccf9b-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ccf9b-141">JSON Representation</span></span>
<span data-ttu-id="ccf9b-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccf9b-142">Here is a JSON representation of the resource.</span></span>
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



