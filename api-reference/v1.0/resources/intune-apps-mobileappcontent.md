---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 76895e336b633da63d62a467a267f96b3f344132
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918877"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="ebfed-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebfed-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="ebfed-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ebfed-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebfed-106">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="ebfed-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="ebfed-107">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="ebfed-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="ebfed-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ebfed-108">Methods</span></span>
|<span data-ttu-id="ebfed-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ebfed-109">Method</span></span>|<span data-ttu-id="ebfed-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ebfed-110">Return Type</span></span>|<span data-ttu-id="ebfed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ebfed-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebfed-112">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="ebfed-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="ebfed-113">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="ebfed-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="ebfed-114">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ebfed-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="ebfed-115">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebfed-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="ebfed-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebfed-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="ebfed-117">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ebfed-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ebfed-118">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebfed-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="ebfed-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebfed-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="ebfed-120">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ebfed-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ebfed-121">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebfed-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="ebfed-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ebfed-122">None</span></span>|<span data-ttu-id="ebfed-123">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ebfed-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="ebfed-124">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebfed-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="ebfed-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ebfed-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="ebfed-126">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ebfed-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ebfed-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebfed-127">Properties</span></span>
|<span data-ttu-id="ebfed-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebfed-128">Property</span></span>|<span data-ttu-id="ebfed-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ebfed-129">Type</span></span>|<span data-ttu-id="ebfed-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ebfed-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebfed-131">id</span><span class="sxs-lookup"><span data-stu-id="ebfed-131">id</span></span>|<span data-ttu-id="ebfed-132">String</span><span class="sxs-lookup"><span data-stu-id="ebfed-132">String</span></span>|<span data-ttu-id="ebfed-133">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="ebfed-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebfed-134">Связи</span><span class="sxs-lookup"><span data-stu-id="ebfed-134">Relationships</span></span>
|<span data-ttu-id="ebfed-135">Связь</span><span class="sxs-lookup"><span data-stu-id="ebfed-135">Relationship</span></span>|<span data-ttu-id="ebfed-136">Тип</span><span class="sxs-lookup"><span data-stu-id="ebfed-136">Type</span></span>|<span data-ttu-id="ebfed-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ebfed-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebfed-138">files</span><span class="sxs-lookup"><span data-stu-id="ebfed-138">files</span></span>|<span data-ttu-id="ebfed-139">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="ebfed-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="ebfed-140">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="ebfed-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebfed-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebfed-141">JSON Representation</span></span>
<span data-ttu-id="ebfed-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebfed-142">Here is a JSON representation of the resource.</span></span>
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



