---
title: Тип ресурса Девицеманажементсеттингколлектионконстраинт
description: Ограничение, которое устанавливает максимальное количество элементов в коллекции
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c285a7cff806585cc9e54b05011c22f8b385036f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528809"
---
# <a name="devicemanagementsettingcollectionconstraint-resource-type"></a><span data-ttu-id="64ce5-103">Тип ресурса Девицеманажементсеттингколлектионконстраинт</span><span class="sxs-lookup"><span data-stu-id="64ce5-103">deviceManagementSettingCollectionConstraint resource type</span></span>

<span data-ttu-id="64ce5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="64ce5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64ce5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64ce5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64ce5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64ce5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64ce5-107">Ограничение, которое устанавливает максимальное количество элементов в коллекции</span><span class="sxs-lookup"><span data-stu-id="64ce5-107">Constraint that enforces the maximum number of elements a collection</span></span>


<span data-ttu-id="64ce5-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="64ce5-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64ce5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="64ce5-109">Properties</span></span>
|<span data-ttu-id="64ce5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="64ce5-110">Property</span></span>|<span data-ttu-id="64ce5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="64ce5-111">Type</span></span>|<span data-ttu-id="64ce5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="64ce5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64ce5-113">минимумленгс</span><span class="sxs-lookup"><span data-stu-id="64ce5-113">minimumLength</span></span>|<span data-ttu-id="64ce5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="64ce5-114">Int32</span></span>|<span data-ttu-id="64ce5-115">Минимальное число элементов в коллекции</span><span class="sxs-lookup"><span data-stu-id="64ce5-115">The minimum number of elements in the collection</span></span>|
|<span data-ttu-id="64ce5-116">максимумленгс</span><span class="sxs-lookup"><span data-stu-id="64ce5-116">maximumLength</span></span>|<span data-ttu-id="64ce5-117">Int32</span><span class="sxs-lookup"><span data-stu-id="64ce5-117">Int32</span></span>|<span data-ttu-id="64ce5-118">Максимальное число элементов в коллекции</span><span class="sxs-lookup"><span data-stu-id="64ce5-118">The maximum number of elements in the collection</span></span>|

## <a name="relationships"></a><span data-ttu-id="64ce5-119">Связи</span><span class="sxs-lookup"><span data-stu-id="64ce5-119">Relationships</span></span>
<span data-ttu-id="64ce5-120">Нет</span><span class="sxs-lookup"><span data-stu-id="64ce5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64ce5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64ce5-121">JSON Representation</span></span>
<span data-ttu-id="64ce5-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64ce5-122">Here is a JSON representation of the resource.</span></span>
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



