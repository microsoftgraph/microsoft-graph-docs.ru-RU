---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 08b2cba09a8b9dadc1d86e1d430b93440de21681
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094388"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="4fcef-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcef-104">mobileAppContent resource type</span></span>

<span data-ttu-id="4fcef-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fcef-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fcef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fcef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fcef-107">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="4fcef-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="4fcef-108">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="4fcef-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="4fcef-109">Методы</span><span class="sxs-lookup"><span data-stu-id="4fcef-109">Methods</span></span>
|<span data-ttu-id="4fcef-110">Метод</span><span class="sxs-lookup"><span data-stu-id="4fcef-110">Method</span></span>|<span data-ttu-id="4fcef-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4fcef-111">Return Type</span></span>|<span data-ttu-id="4fcef-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4fcef-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4fcef-113">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="4fcef-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="4fcef-114">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="4fcef-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="4fcef-115">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="4fcef-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="4fcef-116">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcef-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="4fcef-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcef-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="4fcef-118">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="4fcef-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="4fcef-119">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcef-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="4fcef-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcef-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="4fcef-121">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="4fcef-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="4fcef-122">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcef-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="4fcef-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4fcef-123">None</span></span>|<span data-ttu-id="4fcef-124">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="4fcef-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="4fcef-125">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcef-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="4fcef-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4fcef-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="4fcef-127">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="4fcef-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4fcef-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fcef-128">Properties</span></span>
|<span data-ttu-id="4fcef-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fcef-129">Property</span></span>|<span data-ttu-id="4fcef-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4fcef-130">Type</span></span>|<span data-ttu-id="4fcef-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4fcef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fcef-132">id</span><span class="sxs-lookup"><span data-stu-id="4fcef-132">id</span></span>|<span data-ttu-id="4fcef-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4fcef-133">String</span></span>|<span data-ttu-id="4fcef-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="4fcef-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fcef-135">Связи</span><span class="sxs-lookup"><span data-stu-id="4fcef-135">Relationships</span></span>
|<span data-ttu-id="4fcef-136">Связь</span><span class="sxs-lookup"><span data-stu-id="4fcef-136">Relationship</span></span>|<span data-ttu-id="4fcef-137">Тип</span><span class="sxs-lookup"><span data-stu-id="4fcef-137">Type</span></span>|<span data-ttu-id="4fcef-138">Описание</span><span class="sxs-lookup"><span data-stu-id="4fcef-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fcef-139">files</span><span class="sxs-lookup"><span data-stu-id="4fcef-139">files</span></span>|<span data-ttu-id="4fcef-140">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="4fcef-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="4fcef-141">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="4fcef-141">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4fcef-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4fcef-142">JSON Representation</span></span>
<span data-ttu-id="4fcef-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fcef-143">Here is a JSON representation of the resource.</span></span>
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









