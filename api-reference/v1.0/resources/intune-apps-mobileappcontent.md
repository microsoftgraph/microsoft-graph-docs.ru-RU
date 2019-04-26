---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9cde82585bdbe4ca4c15102e6b343810f29fdae8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557826"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="097e7-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="097e7-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="097e7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="097e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="097e7-106">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="097e7-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="097e7-107">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="097e7-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="097e7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="097e7-108">Methods</span></span>
|<span data-ttu-id="097e7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="097e7-109">Method</span></span>|<span data-ttu-id="097e7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="097e7-110">Return Type</span></span>|<span data-ttu-id="097e7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="097e7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="097e7-112">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="097e7-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="097e7-113">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="097e7-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="097e7-114">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="097e7-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="097e7-115">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="097e7-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|<span data-ttu-id="097e7-116">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="097e7-116">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="097e7-117">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="097e7-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="097e7-118">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="097e7-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|<span data-ttu-id="097e7-119">[mobileAppContent](../resources/intune-apps-mobileappcontent.md);</span><span class="sxs-lookup"><span data-stu-id="097e7-119">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span></span>|<span data-ttu-id="097e7-120">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="097e7-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="097e7-121">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="097e7-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="097e7-122">Нет</span><span class="sxs-lookup"><span data-stu-id="097e7-122">None</span></span>|<span data-ttu-id="097e7-123">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="097e7-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="097e7-124">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="097e7-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="097e7-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="097e7-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="097e7-126">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="097e7-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="097e7-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="097e7-127">Properties</span></span>
|<span data-ttu-id="097e7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="097e7-128">Property</span></span>|<span data-ttu-id="097e7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="097e7-129">Type</span></span>|<span data-ttu-id="097e7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="097e7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="097e7-131">id</span><span class="sxs-lookup"><span data-stu-id="097e7-131">id</span></span>|<span data-ttu-id="097e7-132">String</span><span class="sxs-lookup"><span data-stu-id="097e7-132">String</span></span>|<span data-ttu-id="097e7-133">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="097e7-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="097e7-134">Связи</span><span class="sxs-lookup"><span data-stu-id="097e7-134">Relationships</span></span>
|<span data-ttu-id="097e7-135">Отношение</span><span class="sxs-lookup"><span data-stu-id="097e7-135">Relationship</span></span>|<span data-ttu-id="097e7-136">Тип</span><span class="sxs-lookup"><span data-stu-id="097e7-136">Type</span></span>|<span data-ttu-id="097e7-137">Описание</span><span class="sxs-lookup"><span data-stu-id="097e7-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="097e7-138">files</span><span class="sxs-lookup"><span data-stu-id="097e7-138">files</span></span>|<span data-ttu-id="097e7-139">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="097e7-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="097e7-140">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="097e7-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="097e7-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="097e7-141">JSON Representation</span></span>
<span data-ttu-id="097e7-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="097e7-142">Here is a JSON representation of the resource.</span></span>
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



