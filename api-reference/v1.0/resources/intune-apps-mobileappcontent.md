---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 64e012c25d1674bf3d4ce365aa13ac6a5600b755
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531093"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="69c19-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="69c19-104">mobileAppContent resource type</span></span>

<span data-ttu-id="69c19-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69c19-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69c19-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69c19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69c19-107">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="69c19-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="69c19-108">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="69c19-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="69c19-109">Методы</span><span class="sxs-lookup"><span data-stu-id="69c19-109">Methods</span></span>
|<span data-ttu-id="69c19-110">Метод</span><span class="sxs-lookup"><span data-stu-id="69c19-110">Method</span></span>|<span data-ttu-id="69c19-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="69c19-111">Return Type</span></span>|<span data-ttu-id="69c19-112">Описание</span><span class="sxs-lookup"><span data-stu-id="69c19-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69c19-113">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="69c19-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="69c19-114">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="69c19-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="69c19-115">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="69c19-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="69c19-116">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="69c19-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|<span data-ttu-id="69c19-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="69c19-117">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="69c19-118">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="69c19-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="69c19-119">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="69c19-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|<span data-ttu-id="69c19-120">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="69c19-120">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="69c19-121">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="69c19-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="69c19-122">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="69c19-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="69c19-123">Нет</span><span class="sxs-lookup"><span data-stu-id="69c19-123">None</span></span>|<span data-ttu-id="69c19-124">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="69c19-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="69c19-125">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="69c19-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="69c19-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="69c19-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="69c19-127">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="69c19-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="69c19-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="69c19-128">Properties</span></span>
|<span data-ttu-id="69c19-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="69c19-129">Property</span></span>|<span data-ttu-id="69c19-130">Тип</span><span class="sxs-lookup"><span data-stu-id="69c19-130">Type</span></span>|<span data-ttu-id="69c19-131">Описание</span><span class="sxs-lookup"><span data-stu-id="69c19-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69c19-132">id</span><span class="sxs-lookup"><span data-stu-id="69c19-132">id</span></span>|<span data-ttu-id="69c19-133">Строка</span><span class="sxs-lookup"><span data-stu-id="69c19-133">String</span></span>|<span data-ttu-id="69c19-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="69c19-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69c19-135">Связи</span><span class="sxs-lookup"><span data-stu-id="69c19-135">Relationships</span></span>
|<span data-ttu-id="69c19-136">Связь</span><span class="sxs-lookup"><span data-stu-id="69c19-136">Relationship</span></span>|<span data-ttu-id="69c19-137">Тип</span><span class="sxs-lookup"><span data-stu-id="69c19-137">Type</span></span>|<span data-ttu-id="69c19-138">Описание</span><span class="sxs-lookup"><span data-stu-id="69c19-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69c19-139">files</span><span class="sxs-lookup"><span data-stu-id="69c19-139">files</span></span>|<span data-ttu-id="69c19-140">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="69c19-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="69c19-141">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="69c19-141">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69c19-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69c19-142">JSON Representation</span></span>
<span data-ttu-id="69c19-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69c19-143">Here is a JSON representation of the resource.</span></span>
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




