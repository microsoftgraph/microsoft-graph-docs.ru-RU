---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e819234fd4ee7065378046f8ec977276a8c9f2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260615"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="b96dd-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="b96dd-103">auditProperty resource type</span></span>

> <span data-ttu-id="b96dd-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b96dd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b96dd-105">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="b96dd-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="b96dd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b96dd-106">Properties</span></span>
|<span data-ttu-id="b96dd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b96dd-107">Property</span></span>|<span data-ttu-id="b96dd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b96dd-108">Type</span></span>|<span data-ttu-id="b96dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b96dd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b96dd-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b96dd-110">displayName</span></span>|<span data-ttu-id="b96dd-111">String</span><span class="sxs-lookup"><span data-stu-id="b96dd-111">String</span></span>|<span data-ttu-id="b96dd-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="b96dd-112">Display name.</span></span>|
|<span data-ttu-id="b96dd-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="b96dd-113">oldValue</span></span>|<span data-ttu-id="b96dd-114">String</span><span class="sxs-lookup"><span data-stu-id="b96dd-114">String</span></span>|<span data-ttu-id="b96dd-115">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="b96dd-115">Old value.</span></span>|
|<span data-ttu-id="b96dd-116">newValue</span><span class="sxs-lookup"><span data-stu-id="b96dd-116">newValue</span></span>|<span data-ttu-id="b96dd-117">String</span><span class="sxs-lookup"><span data-stu-id="b96dd-117">String</span></span>|<span data-ttu-id="b96dd-118">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="b96dd-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b96dd-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b96dd-119">Relationships</span></span>
<span data-ttu-id="b96dd-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b96dd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b96dd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b96dd-121">JSON Representation</span></span>
<span data-ttu-id="b96dd-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b96dd-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



