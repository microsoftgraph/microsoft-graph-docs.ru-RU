---
title: тип ресурса windowsUpdateCatalogItem
description: Сущность элемента каталога обновления Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6faffa482a2fc79e653eedf8a70a041f264d7d49
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863613"
---
# <a name="windowsupdatecatalogitem-resource-type"></a><span data-ttu-id="f7021-103">тип ресурса windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="f7021-103">windowsUpdateCatalogItem resource type</span></span>

<span data-ttu-id="f7021-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7021-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7021-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7021-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7021-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7021-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7021-107">Сущность элемента каталога обновления Windows</span><span class="sxs-lookup"><span data-stu-id="f7021-107">Windows update catalog item entity</span></span>

## <a name="methods"></a><span data-ttu-id="f7021-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f7021-108">Methods</span></span>
|<span data-ttu-id="f7021-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f7021-109">Method</span></span>|<span data-ttu-id="f7021-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f7021-110">Return Type</span></span>|<span data-ttu-id="f7021-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f7021-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f7021-112">Список windowsUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="f7021-112">List windowsUpdateCatalogItems</span></span>](../api/intune-softwareupdate-windowsupdatecatalogitem-list.md)|<span data-ttu-id="f7021-113">[коллекция windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="f7021-113">[windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) collection</span></span>|<span data-ttu-id="f7021-114">Список свойств и связей [объектов WindowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="f7021-114">List properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) objects.</span></span>|
|[<span data-ttu-id="f7021-115">Get windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="f7021-115">Get windowsUpdateCatalogItem</span></span>](../api/intune-softwareupdate-windowsupdatecatalogitem-get.md)|[<span data-ttu-id="f7021-116">windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="f7021-116">windowsUpdateCatalogItem</span></span>](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|<span data-ttu-id="f7021-117">Чтение свойств и связей [объекта WindowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="f7021-117">Read properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7021-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7021-118">Properties</span></span>
|<span data-ttu-id="f7021-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7021-119">Property</span></span>|<span data-ttu-id="f7021-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f7021-120">Type</span></span>|<span data-ttu-id="f7021-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f7021-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7021-122">id</span><span class="sxs-lookup"><span data-stu-id="f7021-122">id</span></span>|<span data-ttu-id="f7021-123">String</span><span class="sxs-lookup"><span data-stu-id="f7021-123">String</span></span>|<span data-ttu-id="f7021-124">ID элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="f7021-124">The catalog item id.</span></span>|
|<span data-ttu-id="f7021-125">displayName</span><span class="sxs-lookup"><span data-stu-id="f7021-125">displayName</span></span>|<span data-ttu-id="f7021-126">String</span><span class="sxs-lookup"><span data-stu-id="f7021-126">String</span></span>|<span data-ttu-id="f7021-127">Имя отображения элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="f7021-127">The display name for the catalog item.</span></span>|
|<span data-ttu-id="f7021-128">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="f7021-128">releaseDateTime</span></span>|<span data-ttu-id="f7021-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7021-129">DateTimeOffset</span></span>|<span data-ttu-id="f7021-130">Дата выпуска элемента каталога</span><span class="sxs-lookup"><span data-stu-id="f7021-130">The date the catalog item was released</span></span>|
|<span data-ttu-id="f7021-131">endOfSupportDate</span><span class="sxs-lookup"><span data-stu-id="f7021-131">endOfSupportDate</span></span>|<span data-ttu-id="f7021-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7021-132">DateTimeOffset</span></span>|<span data-ttu-id="f7021-133">Последняя поддерживаемая дата элемента каталога</span><span class="sxs-lookup"><span data-stu-id="f7021-133">The last supported date for a catalog item</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7021-134">Связи</span><span class="sxs-lookup"><span data-stu-id="f7021-134">Relationships</span></span>
<span data-ttu-id="f7021-135">Нет</span><span class="sxs-lookup"><span data-stu-id="f7021-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7021-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7021-136">JSON Representation</span></span>
<span data-ttu-id="f7021-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7021-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "endOfSupportDate": "String (timestamp)"
}
```




