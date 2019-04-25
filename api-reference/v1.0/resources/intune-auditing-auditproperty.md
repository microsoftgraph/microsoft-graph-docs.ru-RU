---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e819234fd4ee7065378046f8ec977276a8c9f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565802"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="778d1-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="778d1-103">auditProperty resource type</span></span>

> <span data-ttu-id="778d1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="778d1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="778d1-105">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="778d1-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="778d1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="778d1-106">Properties</span></span>
|<span data-ttu-id="778d1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="778d1-107">Property</span></span>|<span data-ttu-id="778d1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="778d1-108">Type</span></span>|<span data-ttu-id="778d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="778d1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="778d1-110">displayName</span><span class="sxs-lookup"><span data-stu-id="778d1-110">displayName</span></span>|<span data-ttu-id="778d1-111">String</span><span class="sxs-lookup"><span data-stu-id="778d1-111">String</span></span>|<span data-ttu-id="778d1-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="778d1-112">Display name.</span></span>|
|<span data-ttu-id="778d1-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="778d1-113">oldValue</span></span>|<span data-ttu-id="778d1-114">String</span><span class="sxs-lookup"><span data-stu-id="778d1-114">String</span></span>|<span data-ttu-id="778d1-115">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="778d1-115">Old value.</span></span>|
|<span data-ttu-id="778d1-116">newValue</span><span class="sxs-lookup"><span data-stu-id="778d1-116">newValue</span></span>|<span data-ttu-id="778d1-117">String</span><span class="sxs-lookup"><span data-stu-id="778d1-117">String</span></span>|<span data-ttu-id="778d1-118">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="778d1-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="778d1-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="778d1-119">Relationships</span></span>
<span data-ttu-id="778d1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="778d1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="778d1-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="778d1-121">JSON Representation</span></span>
<span data-ttu-id="778d1-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="778d1-122">Here is a JSON representation of the resource.</span></span>
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



