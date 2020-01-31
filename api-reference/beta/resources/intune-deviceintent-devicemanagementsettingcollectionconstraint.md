---
title: Тип ресурса Девицеманажементсеттингколлектионконстраинт
description: Ограничение, которое устанавливает максимальное количество элементов в коллекции
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cfad548881f4466cce4c4015506a342610c03b35
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636744"
---
# <a name="devicemanagementsettingcollectionconstraint-resource-type"></a><span data-ttu-id="cfb9e-103">Тип ресурса Девицеманажементсеттингколлектионконстраинт</span><span class="sxs-lookup"><span data-stu-id="cfb9e-103">deviceManagementSettingCollectionConstraint resource type</span></span>

> <span data-ttu-id="cfb9e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfb9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfb9e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cfb9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfb9e-106">Ограничение, которое устанавливает максимальное количество элементов в коллекции</span><span class="sxs-lookup"><span data-stu-id="cfb9e-106">Constraint that enforces the maximum number of elements a collection</span></span>


<span data-ttu-id="cfb9e-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="cfb9e-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cfb9e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cfb9e-108">Properties</span></span>
|<span data-ttu-id="cfb9e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfb9e-109">Property</span></span>|<span data-ttu-id="cfb9e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cfb9e-110">Type</span></span>|<span data-ttu-id="cfb9e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cfb9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfb9e-112">минимумленгс</span><span class="sxs-lookup"><span data-stu-id="cfb9e-112">minimumLength</span></span>|<span data-ttu-id="cfb9e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="cfb9e-113">Int32</span></span>|<span data-ttu-id="cfb9e-114">Минимальное число элементов в коллекции</span><span class="sxs-lookup"><span data-stu-id="cfb9e-114">The minimum number of elements in the collection</span></span>|
|<span data-ttu-id="cfb9e-115">максимумленгс</span><span class="sxs-lookup"><span data-stu-id="cfb9e-115">maximumLength</span></span>|<span data-ttu-id="cfb9e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="cfb9e-116">Int32</span></span>|<span data-ttu-id="cfb9e-117">Максимальное число элементов в коллекции</span><span class="sxs-lookup"><span data-stu-id="cfb9e-117">The maximum number of elements in the collection</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfb9e-118">Связи</span><span class="sxs-lookup"><span data-stu-id="cfb9e-118">Relationships</span></span>
<span data-ttu-id="cfb9e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="cfb9e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfb9e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cfb9e-120">JSON Representation</span></span>
<span data-ttu-id="cfb9e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cfb9e-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingCollectionConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCollectionConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```



