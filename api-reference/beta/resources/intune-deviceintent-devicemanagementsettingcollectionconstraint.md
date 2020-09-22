---
title: Тип ресурса Девицеманажементсеттингколлектионконстраинт
description: Ограничение, которое устанавливает максимальное количество элементов в коллекции
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a6bd64e29e01858ce6f1b09ef822e2a3621d5720
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061268"
---
# <a name="devicemanagementsettingcollectionconstraint-resource-type"></a><span data-ttu-id="af064-103">Тип ресурса Девицеманажементсеттингколлектионконстраинт</span><span class="sxs-lookup"><span data-stu-id="af064-103">deviceManagementSettingCollectionConstraint resource type</span></span>

<span data-ttu-id="af064-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af064-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af064-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af064-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af064-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af064-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af064-107">Ограничение, которое устанавливает максимальное количество элементов в коллекции</span><span class="sxs-lookup"><span data-stu-id="af064-107">Constraint that enforces the maximum number of elements a collection</span></span>


<span data-ttu-id="af064-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="af064-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="af064-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="af064-109">Properties</span></span>
|<span data-ttu-id="af064-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="af064-110">Property</span></span>|<span data-ttu-id="af064-111">Тип</span><span class="sxs-lookup"><span data-stu-id="af064-111">Type</span></span>|<span data-ttu-id="af064-112">Описание</span><span class="sxs-lookup"><span data-stu-id="af064-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af064-113">минимумленгс</span><span class="sxs-lookup"><span data-stu-id="af064-113">minimumLength</span></span>|<span data-ttu-id="af064-114">Int32</span><span class="sxs-lookup"><span data-stu-id="af064-114">Int32</span></span>|<span data-ttu-id="af064-115">Минимальное число элементов в коллекции</span><span class="sxs-lookup"><span data-stu-id="af064-115">The minimum number of elements in the collection</span></span>|
|<span data-ttu-id="af064-116">максимумленгс</span><span class="sxs-lookup"><span data-stu-id="af064-116">maximumLength</span></span>|<span data-ttu-id="af064-117">Int32</span><span class="sxs-lookup"><span data-stu-id="af064-117">Int32</span></span>|<span data-ttu-id="af064-118">Максимальное число элементов в коллекции</span><span class="sxs-lookup"><span data-stu-id="af064-118">The maximum number of elements in the collection</span></span>|

## <a name="relationships"></a><span data-ttu-id="af064-119">Связи</span><span class="sxs-lookup"><span data-stu-id="af064-119">Relationships</span></span>
<span data-ttu-id="af064-120">Нет</span><span class="sxs-lookup"><span data-stu-id="af064-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af064-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af064-121">JSON Representation</span></span>
<span data-ttu-id="af064-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af064-122">Here is a JSON representation of the resource.</span></span>
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






