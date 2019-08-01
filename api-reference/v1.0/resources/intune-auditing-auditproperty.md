---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2a3e4ed10a756c4d1cb62bf98c1b6cb13d6f22c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032055"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="507f7-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="507f7-103">auditProperty resource type</span></span>

> <span data-ttu-id="507f7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="507f7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="507f7-105">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="507f7-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="507f7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="507f7-106">Properties</span></span>
|<span data-ttu-id="507f7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="507f7-107">Property</span></span>|<span data-ttu-id="507f7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="507f7-108">Type</span></span>|<span data-ttu-id="507f7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="507f7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="507f7-110">displayName</span><span class="sxs-lookup"><span data-stu-id="507f7-110">displayName</span></span>|<span data-ttu-id="507f7-111">String</span><span class="sxs-lookup"><span data-stu-id="507f7-111">String</span></span>|<span data-ttu-id="507f7-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="507f7-112">Display name.</span></span>|
|<span data-ttu-id="507f7-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="507f7-113">oldValue</span></span>|<span data-ttu-id="507f7-114">String</span><span class="sxs-lookup"><span data-stu-id="507f7-114">String</span></span>|<span data-ttu-id="507f7-115">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="507f7-115">Old value.</span></span>|
|<span data-ttu-id="507f7-116">newValue</span><span class="sxs-lookup"><span data-stu-id="507f7-116">newValue</span></span>|<span data-ttu-id="507f7-117">String</span><span class="sxs-lookup"><span data-stu-id="507f7-117">String</span></span>|<span data-ttu-id="507f7-118">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="507f7-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="507f7-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="507f7-119">Relationships</span></span>
<span data-ttu-id="507f7-120">Нет</span><span class="sxs-lookup"><span data-stu-id="507f7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="507f7-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="507f7-121">JSON Representation</span></span>
<span data-ttu-id="507f7-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="507f7-122">Here is a JSON representation of the resource.</span></span>
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



