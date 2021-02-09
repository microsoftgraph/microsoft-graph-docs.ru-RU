---
title: Тип ресурса windowsUpdateCatalogItem
description: Сущность элемента каталога обновлений Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5de85dde2c9f2b5bc68e9644b96852bdbe880de
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162447"
---
# <a name="windowsupdatecatalogitem-resource-type"></a><span data-ttu-id="b18f6-103">Тип ресурса windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="b18f6-103">windowsUpdateCatalogItem resource type</span></span>

<span data-ttu-id="b18f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b18f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b18f6-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b18f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b18f6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b18f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b18f6-107">Сущность элемента каталога обновлений Windows</span><span class="sxs-lookup"><span data-stu-id="b18f6-107">Windows update catalog item entity</span></span>

## <a name="methods"></a><span data-ttu-id="b18f6-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b18f6-108">Methods</span></span>
|<span data-ttu-id="b18f6-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b18f6-109">Method</span></span>|<span data-ttu-id="b18f6-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b18f6-110">Return Type</span></span>|<span data-ttu-id="b18f6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b18f6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b18f6-112">Список windowsUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="b18f6-112">List windowsUpdateCatalogItems</span></span>](../api/intune-softwareupdate-windowsupdatecatalogitem-list.md)|<span data-ttu-id="b18f6-113">[Коллекция windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b18f6-113">[windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) collection</span></span>|<span data-ttu-id="b18f6-114">Список свойств и связей объектов [windowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b18f6-114">List properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) objects.</span></span>|
|[<span data-ttu-id="b18f6-115">Get windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="b18f6-115">Get windowsUpdateCatalogItem</span></span>](../api/intune-softwareupdate-windowsupdatecatalogitem-get.md)|[<span data-ttu-id="b18f6-116">windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="b18f6-116">windowsUpdateCatalogItem</span></span>](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|<span data-ttu-id="b18f6-117">Чтение свойств и связей объекта [windowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="b18f6-117">Read properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b18f6-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="b18f6-118">Properties</span></span>
|<span data-ttu-id="b18f6-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="b18f6-119">Property</span></span>|<span data-ttu-id="b18f6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b18f6-120">Type</span></span>|<span data-ttu-id="b18f6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b18f6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b18f6-122">id</span><span class="sxs-lookup"><span data-stu-id="b18f6-122">id</span></span>|<span data-ttu-id="b18f6-123">String</span><span class="sxs-lookup"><span data-stu-id="b18f6-123">String</span></span>|<span data-ttu-id="b18f6-124">ИД элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="b18f6-124">The catalog item id.</span></span>|
|<span data-ttu-id="b18f6-125">displayName</span><span class="sxs-lookup"><span data-stu-id="b18f6-125">displayName</span></span>|<span data-ttu-id="b18f6-126">String</span><span class="sxs-lookup"><span data-stu-id="b18f6-126">String</span></span>|<span data-ttu-id="b18f6-127">Отображаемого имени элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="b18f6-127">The display name for the catalog item.</span></span>|
|<span data-ttu-id="b18f6-128">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="b18f6-128">releaseDateTime</span></span>|<span data-ttu-id="b18f6-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b18f6-129">DateTimeOffset</span></span>|<span data-ttu-id="b18f6-130">Дата выпуска элемента каталога</span><span class="sxs-lookup"><span data-stu-id="b18f6-130">The date the catalog item was released</span></span>|

## <a name="relationships"></a><span data-ttu-id="b18f6-131">Связи</span><span class="sxs-lookup"><span data-stu-id="b18f6-131">Relationships</span></span>
<span data-ttu-id="b18f6-132">Нет</span><span class="sxs-lookup"><span data-stu-id="b18f6-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b18f6-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b18f6-133">JSON Representation</span></span>
<span data-ttu-id="b18f6-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b18f6-134">Here is a JSON representation of the resource.</span></span>
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
  "releaseDateTime": "String (timestamp)"
}
```




