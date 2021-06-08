---
title: Тип ресурса mobileAppContent
description: Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c36a306e0b594ff84bffbc3e80fd393d20051371
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759011"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="a74d2-104">Тип ресурса mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a74d2-104">mobileAppContent resource type</span></span>

<span data-ttu-id="a74d2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a74d2-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a74d2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a74d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a74d2-107">Содержит свойства контента для определенной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="a74d2-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="a74d2-108">Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="a74d2-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="a74d2-109">Методы</span><span class="sxs-lookup"><span data-stu-id="a74d2-109">Methods</span></span>
|<span data-ttu-id="a74d2-110">Метод</span><span class="sxs-lookup"><span data-stu-id="a74d2-110">Method</span></span>|<span data-ttu-id="a74d2-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a74d2-111">Return Type</span></span>|<span data-ttu-id="a74d2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a74d2-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a74d2-113">Список объектов mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="a74d2-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="a74d2-114">Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="a74d2-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="a74d2-115">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a74d2-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="a74d2-116">Получение объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a74d2-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="a74d2-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a74d2-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="a74d2-118">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a74d2-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="a74d2-119">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a74d2-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="a74d2-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a74d2-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="a74d2-121">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a74d2-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="a74d2-122">Удаление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a74d2-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="a74d2-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a74d2-123">None</span></span>|<span data-ttu-id="a74d2-124">Удаляет объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a74d2-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="a74d2-125">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a74d2-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="a74d2-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a74d2-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="a74d2-127">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a74d2-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a74d2-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="a74d2-128">Properties</span></span>
|<span data-ttu-id="a74d2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a74d2-129">Property</span></span>|<span data-ttu-id="a74d2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a74d2-130">Type</span></span>|<span data-ttu-id="a74d2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a74d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a74d2-132">id</span><span class="sxs-lookup"><span data-stu-id="a74d2-132">id</span></span>|<span data-ttu-id="a74d2-133">String</span><span class="sxs-lookup"><span data-stu-id="a74d2-133">String</span></span>|<span data-ttu-id="a74d2-134">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="a74d2-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a74d2-135">Связи</span><span class="sxs-lookup"><span data-stu-id="a74d2-135">Relationships</span></span>
|<span data-ttu-id="a74d2-136">Связь</span><span class="sxs-lookup"><span data-stu-id="a74d2-136">Relationship</span></span>|<span data-ttu-id="a74d2-137">Тип</span><span class="sxs-lookup"><span data-stu-id="a74d2-137">Type</span></span>|<span data-ttu-id="a74d2-138">Описание</span><span class="sxs-lookup"><span data-stu-id="a74d2-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a74d2-139">files</span><span class="sxs-lookup"><span data-stu-id="a74d2-139">files</span></span>|<span data-ttu-id="a74d2-140">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="a74d2-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="a74d2-141">Список файлов для этой версии контента приложения.</span><span class="sxs-lookup"><span data-stu-id="a74d2-141">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a74d2-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a74d2-142">JSON Representation</span></span>
<span data-ttu-id="a74d2-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a74d2-143">Here is a JSON representation of the resource.</span></span>
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




